---
title: Sjablonen aanpassen
description: Leer hoe u een aangepaste sjabloon voor GenStudio maakt.
level: Intermediate
feature: Templates, Content
source-git-commit: 423956d6fdbf5b31041d44eb434f90d55a87d7c0
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---


# Sjablonen aanpassen

U kunt uw malplaatjes van HTML voor GenStudio aanpassen door de _het malplaatjetaal te gebruiken 0} Handlebars {._ De syntaxis Handlebars gebruikt regelmatige tekst met dubbele steunen als inhoudplaceholders. Zie [`What is Handlebars?` ](https://handlebarsjs.com/guide/#what-is-handlebars) in de _de taalgids van Handlebars_ leren hoe te om uw malplaatje voor te bereiden.

## Sjabloonstructuur

<!-- This is for email. In the future, maybe use tabs to provide guidance for other template types.
-->

Als u geen HTML-sjabloon klaar hebt voor gebruik in GenStudio, kunt u eerst de structuur van uw e-mail definiëren met behulp van HTML-tags: `DOCTYPE`, `html`, `head` en `body` . U kunt CSS-stijlen opnemen om de weergave van uw e-mail aan te passen.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Title</title>
    <style>
    </style>
</head>
<body>
</body>
</html>
```

>[!TIP]
>
>Voeg in de volgende secties plaatsaanduidingen voor inhoud toe voor e-mailvelden, verberg overbodige elementen uit de voorvertoning en beheer koppelingen naar statische inhoud. Zodra uw malplaatje klaar is, kunt u het [ uploaden aan GenStudio ](use-templates.md#upload-a-template) en beginnen gepersonaliseerde e-mails te produceren die op uw douanemalplaatje worden gebaseerd.

## Plaatsaanduidingen voor inhoud

In de kop of het hoofdgedeelte van de sjabloon kunt u met de syntaxis Handlebars tijdelijke aanduidingen voor inhoud invoegen op plaatsen waar u GenStudio nodig hebt om het e-mailbericht te vullen met werkelijke inhoud. GenStudio herkent en interpreteert automatisch de plaatsaanduidingen voor inhoud op basis van de veldnaam.

Met `{{ headline }}` kunt u bijvoorbeeld aangeven waar de kop van het e-mailbericht moet worden geplaatst:

```handlebars
<div>{{ headline }}</div>
```

Het maximumaantal velden dat in een aangepaste sjabloon is toegestaan, is twintig.

**Erkende gebiedsnamen**:

| Veld | Rol | Kanaalsjabloon |
| -------------- | ---------------------- | -------------------- |
| `pre_header` | Pre-header | email |
| `headline` | Titel | email<br> sociale advertentie |
| `body` | Platte kopie | email<br> sociale advertentie |
| `cta` | Oproep tot actie | email<br> sociale advertentie |
| `on_image_text` | Op afbeeldingstekst | sociaal en |
| `image` | Afbeelding | email<br> sociale advertentie |
| `brand_logo` | Logo van het geselecteerde merk | sociaal en |

>[!IMPORTANT]
>
>Tijdens het [!DNL Create] -proces verschaft GenStudio automatisch een `subject` -veld voor de e-mailsjabloon. Het is dus niet nodig het onderwerpveld op te nemen in uw e-mailsjabloon.

+++Voorbeeld: standaardsjabloon

Hier volgt een eenvoudig voorbeeld van een HTML-sjabloon voor e-mail. De kop bevat eenvoudige inline CSS voor opmaak. De hoofdtekst bevat een tijdelijke aanduiding `pre-header` , `headline` en `image` die door GenStudio kan worden gebruikt om inhoud te injecteren tijdens het genereren van e-mail.

```handlebars {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

### Achtergrondafbeelding

Bij het ontwerpen van een advertentie voor Meta is het belangrijk om een achtergrondafbeelding te gebruiken die wordt aangevuld met tekst en een merklogo-overlay. Voor een correcte schaling van de afbeelding moet u voor Meta-sjablonen een `aspect ratio` opgeven. In deze context kunt u slechts één afbeeldingsveld opgeven.

## Secties of groepen

_de Secties_ verstrekken een manier om GenStudio mee te delen dat de gebieden die tot een sectie behoren een hoge graad van coherentie vereisen. Als u deze relatie instelt, kan de AI inhoud genereren die overeenkomt met de creatieve elementen in de sectie. Een sjabloon kan maximaal drie secties bevatten.

Gebruik een voorvoegsel van uw keuze in de veldnaam om aan te geven dat dit veld deel uitmaakt van een sectie of groep. U kunt bijvoorbeeld de inhoud die in een gemarkeerd gebied wordt weergegeven, als spotlight instellen. U kunt de inhoud voor dit gebied identificeren met een algemeen voorvoegsel:

- `spotlight_headline`
- `spotlight_body`

Elke sectie kan slechts één veldtype hebben. De voorbeeldgroep met het voorvoegsel `spotlight` kan bijvoorbeeld slechts één veld `spotlight_headline` hebben.

Wanneer u meerdere secties hebt (maximaal drie):

- `headline`
- `body`
- `spotlight_headline`
- `spotlight_body`
- `news_headline`
- `news_body`

GenStudio begrijpt dat `spotlight_headline` nauwer verwant is aan `spotlight_body` dan aan `news_body` .

+++Voorbeeld: sjabloon met meerdere secties

In het bovenstaande voorbeeld ziet u dezelfde HTML-sjabloon, maar met nog twee secties. De kop bevat inline CSS voor het opmaken van een pod. De hoofdtekst gebruikt twee pods met plaatsaanduidingen voor inhoud met een voorvoegsel.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
        .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
        }
        .pod h2 {
            color: #333;
        }
        .pod p {
            color: #666;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
        <div class="pod">
            <h2>{{ pod1_headline }}</h2>
            <p>This is Pod 1 content.</p>
        </div>
        <div class="pod">
            <h2>{{ pod2_headline }}</h2>
            <p>This is Pod 2 content.</p>
        </div>
    </div>
</body>
</html>
```

+++

## Sjabloonvoorbeeld

E-mailsjablonen bevatten soms speciale inhoud die niet nodig is voor een voorvertoning in GenStudio. U kunt de zichtbaarheid van deze inhoud bepalen met ingebouwde helpers. Dit zijn speciale expressies in de sjabloontaal Handlebars die u helpen bepaalde handelingen uit te voeren.

De waarde `_genStudio.browser` wordt ingesteld bij het renderen van een sjabloon en de waarde `genStudio.export` wordt ingesteld bij het exporteren van een sjabloon. U kunt bepaalde inhoud boven aan de e-mails plaatsen met een voorwaardelijke wrapper, bijvoorbeeld wanneer de sjabloon wordt gebruikt voor exporteren:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Een ander voorbeeld kan zijn om het gebruik van volgcodes te verhinderen wanneer het previewing van een e-mailmalplaatje in GenStudio. In dit voorbeeld wordt getoond hoe u volgparameters kunt toevoegen aan koppelingen in de geëxporteerde sjabloon, terwijl de voorbeeldkoppelingen schoon blijven:

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Statische inhoud

E-mail- en metasjablonen zijn vaak gekoppeld aan afbeeldingen en CSS-bestanden die buiten GenStudio worden gehost. Wanneer GenStudio miniaturen voor deze sjablonen of de ervaringen die hiervan zijn afgeleid genereert, kunnen deze externe bronnen worden genegeerd als ze niet de juiste koppen CORS (Cross-Origin Resource Sharing) hebben.

Houd rekening met twee opties om ervoor te zorgen dat deze bronnen beschikbaar zijn tijdens het genereren van miniaturen:

1. **de Kopballen van CORS van het Gebruik**: De gastheerserver moet reacties met een `Access-Control-Allow-Origin` kopbal verzenden die aan `https://experience.adobe.com` waarde voor productiemilieu&#39;s wordt geplaatst. Met deze methode kan GenStudio toegang krijgen tot de bronnen en deze opnemen.
1. **Gegevens URLs van het Gebruik**: Sluit direct de externe middelen in het malplaatje in gebruikend Gegevens URLs. Deze methode omzeilt de beperkingen van CORS en zorgt ervoor dat de middelen tijdens duimnagelgeneratie beschikbaar zijn.
