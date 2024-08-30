---
title: Een sjabloon aanpassen
description: Leer hoe u uw sjabloon kunt aanpassen en optimaliseren voor Adobe GenStudio voor Performance Marketers.
level: Intermediate
feature: Templates, Content
source-git-commit: 909ac53580e672df1adf0c73e67a32f2c045dc35
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---


# Een sjabloon aanpassen

Pas uw malplaatjes van HTML voor Adobe GenStudio voor de Marketers van Prestaties aan door de _het malplaatjetaal te gebruiken 0} Handlebars {._ In de syntaxis van [!DNL Handlebars] wordt gewone tekst met dubbele accolades gebruikt als plaatsaanduidingen voor inhoud. Zie [`What is [!DNL Handlebars]?` ](https://handlebarsjs.com/guide/#what-is-handlebars) in de _de taalgids van Handlebars_ leren hoe te om uw malplaatje voor te bereiden.

In de volgende secties wordt uitgelegd hoe u plaatsaanduidingen voor inhoud toevoegt, overbodige elementen uit de voorvertoning verbergt en koppelingen naar statische inhoud beheert. Zodra uw malplaatje klaar is, kunt u het [ uploaden aan GenStudio voor de Marketers van Prestaties ](use-templates.md#upload-a-template) en beginnen gepersonaliseerde e-mails te produceren die op uw douanemalplaatje worden gebaseerd.

## Plaatsaanduidingen voor inhoud

GenStudio voor de Marketers van Prestaties erkent bepaalde [ elementen ](use-templates.md#template-elements) binnen een malplaatje, maar slechts als u hen met een erkende gebiedsnaam identificeert.

In de kop of de hoofdtekst van een sjabloon kunt u de syntaxis van [!DNL Handlebars] gebruiken als plaatsaanduiding voor inhoud, waarbij u GenStudio for Performance Marketers nodig hebt om de sjabloon te vullen met werkelijke inhoud. GenStudio voor de Marketers van Prestaties herkent en interpreteert de inhoudsplaceholders die op [ worden gebaseerd herkende _gebied_ naam ](#recognized-field-names).

U kunt `{{ headline }}` bijvoorbeeld met de syntaxis van [!DNL Handlebars] gebruiken om aan te geven waar de kop van de e-mail moet worden geplaatst:

```handlebars
<div>{{headline}}</div>
```

### Erkende veldnamen

In de volgende tabel worden de veldnamen weergegeven die door GenStudio for Performance Marketers voor populaties worden herkend in sjablonen. Voeg deze veldnamen met de syntaxis [!DNL Handlebars] toe aan uw sjabloon waar u GenStudio for Performance Marketers nodig hebt om inhoud te genereren.

| Veld | Rol | Kanaalsjabloon |
| -------------- | ---------------------- | ------------------------------ |
| `pre_header` | Pre-header | email |
| `headline` | Titel | email <br> Meta-advertentie |
| `body` | Platte kopie | email <br> Meta-advertentie |
| `cta` | Oproep tot actie | email <br> Meta-advertentie |
| `on_image_text` | Op afbeeldingstekst | Meta en |
| `image` | Afbeelding | email <br> Meta-advertentie |
| `brand_logo` | Logo van geselecteerd merk <br> zie [ het merklogo gebiedsnaam ](#brand-logo-field-name) voor geadviseerd gebruik. | e-mail <br> Meta-advertentie |

GenStudio for Performance Marketers vult bepaalde velden automatisch in de volgende sjablonen in:

- **E-mailmalplaatje** vereist u niet om het `subject` gebied te identificeren
- **malplaatje van Advertenties van Meta** vereist u niet om `headline` te identificeren, `body`, en `CTA` gebieden

<!--
- **Display Ads template** does not require you to idenitify the `CTA` field
-->

>[!WARNING]
>
>Voor Instagram-advertenties wordt de gegenereerde kop niet weergegeven in de uiteindelijke ervaring.

Er geldt een limiet van 20 velden wanneer u een sjabloon uploadt naar GenStudio for Performance Marketers. Aangezien het veld `subject` automatisch wordt gegenereerd in een e-mail, telt het als één veld. Dit betekent dat er 19 velden zijn toegestaan in een e-mailsjabloon.

>[!TIP]
>
>U kunt uw malplaatje verifiëren gebruikend de [ malplaatjevoorproef ](#template-preview) in GenStudio voor de Marketers van Prestaties.

#### Naam merklogo

Op dit moment kunt u het merklogo voor het uploaden van de sjabloon niet selecteren. In de volgende voorbeelden worden twee methoden getoond die het merklogo voorwaardelijk weergeven. Elke methode verifieert de bron, biedt een standaard- of alternatieve afbeelding voor het geval het merklogo niet beschikbaar is en past een stijl toe:

**Voorbeeld 1**: Het gebruiken van [!DNL Handlebars] Ingebouwde voorwaarde van Helpers direct in het HTML `img src` attribuut:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Voorbeeld 2**: Het gebruiken van [!DNL Handlebars] Ingebouwde voorwaardelverklaring om de HTML `img` markering te verpakken:

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### Handmatige veldnamen

Alle andere veldnamen worden behandeld als handmatig gevulde velden.

Als u een bewerkbare sectie wilt maken, voegt u dubbele haakjes toe rond de sectienaam:

```handlebars
{{customVariable}}
```

### Secties of groepen

_secties_ informeren GenStudio voor de Marketers van Prestaties dat de gebieden in deze sectie een hoge graad van coherentie vereisen. Als u deze relatie instelt, kan de AI inhoud genereren die overeenkomt met de creatieve elementen in de sectie.

Gebruik een voorvoegsel van uw keuze in de veldnaam om aan te geven dat een veld deel uitmaakt van een sectie of groep. U kunt bijvoorbeeld de inhoud van een gemarkeerd gebied als spotlight instellen:

- `spotlight_headline`
- `spotlight_body`

Elke sectie kan slechts één van elk gebiedstype gebruiken. In het bovenstaande voorbeeld kan de sectie `spotlight` slechts één `spotlight_headline` -veld gebruiken.

Een sjabloon kan maximaal drie secties bevatten:

- `headline`
- `body`
- `spotlight_headline`
- `spotlight_body`
- `news_headline`
- `news_body`

GenStudio for Performance Marketers begrijpt dat `spotlight_headline` nauwer verwant is aan `spotlight_body` dan aan `news_body` .

## Sjabloonvoorbeeld

Wanneer u [ een malplaatje ](use-templates.md#upload-a-template) uploadt, scant GenStudio voor de Marketers van Prestaties het dossier van de HTML voor erkende gebieden. Gebruik de voorproef om uw [ malplaatjeelementen ](use-templates.md#template-elements) te herzien en te bevestigen dat u hen behoorlijk met [ erkende gebiedsnamen ](#recognized-field-names) identificeerde.

Voorbeeld van een e-mailsjabloon:

![ ontdekte gebieden van de Voorproef ](../../assets/template-detected-fields.png){width="650"}

### Voorvertoning besturen

U kunt de zichtbaarheid van speciale inhoud bepalen met behulp van ingebouwde hulpmiddelen (speciale expressies in de sjabloontaal [!DNL Handlebars] die bepaalde handelingen uitvoeren). U kunt bijvoorbeeld een voorwaardelijke instructie toevoegen waarmee trackingparameters worden toegevoegd aan koppelingen in de geëxporteerde sjabloon terwijl de voorbeeldkoppelingen schoon blijven.

De waarde `_genStudio.browser` wordt ingesteld bij het renderen van een sjabloon en de waarde `genStudio.export` wordt ingesteld bij het exporteren van een sjabloon. U kunt besluiten om bepaalde inhoud bij de bovenkant van een e-mail te omvatten gebruikend een voorwaardelijke omslag, bijvoorbeeld wanneer het malplaatje voor de uitvoer wordt gebruikt:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Een ander voorbeeld kan zijn om het gebruik van volgcodes te verhinderen wanneer het voorvertonen van een malplaatje in GenStudio for Performance Marketers. In het volgende voorbeeld ziet u hoe u volgparameters toevoegt aan koppelingen in de geëxporteerde sjabloon, terwijl de voorbeeldkoppelingen ongewijzigd blijven:

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Statische inhoud

E-mailsjablonen en meta-sjablonen zijn vaak gekoppeld aan afbeeldingen en CSS-bestanden die buiten GenStudio for Performance Marketers worden gehost. Wanneer GenStudio for Performance Marketers miniaturen voor deze sjablonen of de ervaringen die hiervan zijn afgeleid, genereert, kunnen deze externe bronnen worden genegeerd als ze niet de juiste koppen CORS (Cross-Origin Resource Sharing) hebben.

Houd rekening met twee opties om ervoor te zorgen dat deze bronnen beschikbaar zijn tijdens het genereren van miniaturen:

1. **de Kopballen van CORS van het Gebruik**: De gastheerserver moet reacties met een `Access-Control-Allow-Origin` kopbal verzenden die aan `https://experience.adobe.com` waarde voor productiemilieu&#39;s wordt geplaatst. Met deze methode kunnen GenStudio for Performance Marketers toegang krijgen tot de bronnen en deze opnemen.

1. **Gegevens URLs van het Gebruik**: Sluit direct de externe middelen in het malplaatje in gebruikend Gegevens URLs. Deze methode omzeilt de beperkingen van CORS en zorgt ervoor dat de middelen tijdens duimnagelgeneratie beschikbaar zijn.

## Sjabloonvoorbeelden

+++Voorbeeld: E-mailsjabloon met één sectie

Hier volgt een eenvoudig voorbeeld van een HTML-sjabloon voor een e-mailbericht dat één sectie bevat. De kop bevat eenvoudige inline CSS voor opmaak. Het lichaam bevat a `pre-header`, `headline`, en `image` [ placeholder ](#content-placeholders) voor gebruik door GenStudio voor de Marketers van Prestaties om inhoud tijdens het e-mailgeneratieproces te injecteren.

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

