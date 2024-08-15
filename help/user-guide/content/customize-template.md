---
title: Sjablonen aanpassen
description: Leer hoe u een aangepaste sjabloon voor GenStudio maakt.
level: Intermediate
feature: Templates, Content
source-git-commit: c9cf7da078e84cf7696f32ca2278aa71b7b1b7cc
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---


# Sjablonen aanpassen

Pas uw malplaatjes van HTML voor GenStudio aan door de _het malplaatjetaal te gebruiken 0} Handlebars {._ De syntaxis Handlebars gebruikt regelmatige tekst met dubbele steunen als inhoudplaceholders. Zie [`What is Handlebars?` ](https://handlebarsjs.com/guide/#what-is-handlebars) in de _de taalgids van Handlebars_ leren hoe te om uw malplaatje voor te bereiden.

<!-- This is for email. In the future, maybe use tabs to provide guidance for other template types.
-->If you do not have an HTML template ready to use in GenStudio, you can start by defining the structure of your email using HTML tags: `DOCTYPE`, `html`, `head`, and `body`. You can include CSS styles to customize the appearance of your email.

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

Zie [ voorbeelden van het Malplaatje ](#template-examples).

>[!TIP]
>
>Voeg in de volgende secties plaatsaanduidingen voor inhoud toe voor e-mailvelden, zie voorbeeldsjablonen, verberg overbodige elementen uit de voorvertoning en beheer koppelingen naar statische inhoud. Zodra uw malplaatje klaar is, kunt u het [ uploaden aan GenStudio ](use-templates.md#upload-a-template) en beginnen gepersonaliseerde e-mails te produceren die op uw douanemalplaatje worden gebaseerd.

## Plaatsaanduidingen voor inhoud

Binnen de kop of de hoofdtekst van een sjabloon kunt u de syntaxis Handlebars gebruiken om plaatsaanduidingen voor inhoud in te voegen op plaatsen waar GenStudio de sjabloon moet vullen met werkelijke inhoud. GenStudio herkent en interpreteert automatisch de plaatsaanduidingen voor inhoud op basis van de veldnaam.

Met `{{ headline }}` kunt u bijvoorbeeld aangeven waar de kop van het e-mailbericht moet worden geplaatst:

```handlebars
<div>{{ headline }}</div>
```

### Veldnamen

Het maximumaantal velden dat in een aangepaste sjabloon is toegestaan, is twintig.

#### Erkende veldnamen

De volgende tabel bevat een lijst met de veldnamen die door GenStudio worden herkend voor populatie in sjablonen.

| Veld | Rol | Kanaalsjabloon |
| -------------- | ---------------------- | -------------------- |
| `pre_header` | Pre-header | e-mail (aanbevolen) |
| `headline` | Titel | e-mail (geadviseerd) <br> Meta ad |
| `body` | Platte kopie | e-mail (geadviseerd) <br> Meta ad |
| `cta` | Oproep tot actie | e-mail (geadviseerd) <br> Meta ad |
| `on_image_text` | Op afbeeldingstekst | Meta-advertentie (aanbevolen) |
| `image` | Afbeelding | e-mail (geadviseerd) <br> Meta en (geadviseerd) |
| `brand_logo` | Logo van het geselecteerde merk | e-mail <br> Meta-advertentie |

GenStudio vult bepaalde velden automatisch in sjablonen in. Deze velden hoeven dus niet in uw sjabloonontwerpen te worden opgenomen:

* `subject` (e-mailsjabloon)
* `headline` -, `body` - en `CTA` -velden (metagegevens en sjabloon)

>[!WARNING]
>
>Voor Instagram-advertenties wordt de gegenereerde kop niet weergegeven in de uiteindelijke ervaring.

#### Naam merklogo

Als u een merklogo aan uw sjabloon wilt toevoegen, gebruikt u een van de volgende methoden om het standaardlogo te renderen.

_Voorbeeld_:

```bash
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default image>{{/if}}" alt="WKND" style="max-width: 88px; margin: 10px auto; display: block;"> 
```

_Voorbeeld_:

```bash
{{#if brand_logo}}

                    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">

                {{else}}

                    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">

                {{/if}}
```

#### Handmatige veldnamen

Alle andere veldnamen worden behandeld als handmatig gevulde velden. Als u een sectie bewerkbaar wilt maken, voegt u dubbele haakjes toe rond de sectie die u wilt bewerken.

_Voorbeeld_: ``{{customVariable}}`` (`customVariable` is de manueel editable sectie)

## Secties of groepen

_Secties_ informeren GenStudio dat de gebieden in deze sectie een hoge graad van coherentie vereisen. Als u deze relatie instelt, kan de AI inhoud genereren die overeenkomt met de creatieve elementen in de sectie.

Gebruik een voorvoegsel van uw keuze in de veldnaam om aan te geven dat een veld deel uitmaakt van een sectie of groep.

U kunt bijvoorbeeld de inhoud van een gemarkeerd gebied als spotlight instellen:

* `spotlight_headline`
* `spotlight_body`

Elke sectie kan slechts één van elk gebiedstype hebben. In het bovenstaande voorbeeld kan het voorvoegsel `spotlight` slechts één veld `spotlight_headline` hebben.

Een sjabloon kan maximaal drie secties bevatten:

* `headline`
* `body`
* `spotlight_headline`
* `spotlight_body`
* `news_headline`
* `news_body`

GenStudio begrijpt dat `spotlight_headline` nauwer verwant is aan `spotlight_body` dan aan `news_body` .

## Sjabloonvoorbeelden

+++Voorbeeld: E-mailsjabloon met één sectie

Hier volgt een eenvoudig voorbeeld van een HTML-sjabloon voor een e-mailbericht dat één sectie bevat. De kop bevat eenvoudige inline CSS voor opmaak. Het lichaam bevat a `pre-header`, `headline`, en `image` [ placeholder ](#content-placeholders) voor gebruik door GenStudio om inhoud tijdens het proces van de e-mailgeneratie te injecteren.

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

+++Voorbeeld: E-mailsjabloon met meerdere secties

In het bovenstaande voorbeeld ziet u dezelfde HTML-sjabloon, maar met nog twee secties. De kop bevat inline CSS voor het opmaken van een groep. Het lichaam gebruikt twee groepen met [ inhoudplaceholders ](#content-placeholders) gebruikend een prefix.

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

+++Voorbeeld: Meta-advertentiesjabloon

Hier volgt een eenvoudig voorbeeld van een advertentiesjabloon van Meta. De kop bevat inline CSS voor opmaak. Het lichaam gebruikt [ inhoudplaceholders ](#content-placeholders) gebruikend een prefix.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>

</body>
</html>
```

+++

## Sjabloonvoorbeeld

Bepaal de zichtbaarheid van speciale inhoud met behulp van ingebouwde hulpmiddelen (speciale expressies in de sjabloontaal Handlebars die bepaalde handelingen uitvoeren). U kunt bijvoorbeeld parameters voor het bijhouden van koppelingen toevoegen aan de koppelingen in de geëxporteerde sjabloon terwijl de koppelingen voor de voorvertoning ongewijzigd blijven.

De waarde `_genStudio.browser` wordt ingesteld bij het renderen van een sjabloon en de waarde `genStudio.export` wordt ingesteld bij het exporteren van een sjabloon. U kunt besluiten om bepaalde inhoud bij de bovenkant van een e-mail te omvatten gebruikend een voorwaardelijke omslag, bijvoorbeeld wanneer het malplaatje voor de uitvoer wordt gebruikt:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Een ander voorbeeld kan zijn om het gebruik van volgcodes te verhinderen wanneer het previewing van een malplaatje in GenStudio. In dit voorbeeld wordt getoond hoe u volgparameters kunt toevoegen aan koppelingen in de geëxporteerde sjabloon, terwijl de voorbeeldkoppelingen schoon blijven:

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
