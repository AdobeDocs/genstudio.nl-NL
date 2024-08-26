---
title: Toegankelijke sjablonen maken
description: Bouw malplaatjes die alle publiek voor gebruik in Adobe GenStudio voor de Marketers van Prestaties kunnen bereiken.
feature: Templates, Content
source-git-commit: 26d1b9c7b392e93e87ffcd9444f391c2980d1c3c
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---


# Toegankelijke sjablonen maken

Adobe streeft ernaar een optimale ervaring voor alle doelgroepen te bieden. Zie [ Initiatieven van de Toegankelijkheid bij Adobe ](https://www.adobe.com/trust/accessibility/initiatives.html) voor verdere lezing.

In GenStudio for Performance Marketers kunt u elementen en sjablonen uploaden waarmee u inhoud kunt maken voor verschillende ervaringen. Door de toegankelijkheidsstandaarden te respecteren, bereikt u uw inhoud het maximale doelpubliek.

Gebruik de volgende aanbevelingen om uw sjablonen voor te bereiden met behulp van optimale toegankelijkheidsstandaarden.

## Alternatieve tekst

Maak tekstalternatieven voor niet-tekstuele inhoud, zoals afbeeldingen.

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![ Collage van ideeën, boeken, man die reuzenpotlood, computer ](../../assets/card-create-assets.png){width="400"} houden

## Koppelingsdoel (alleen koppeling)

Maak duidelijke koppelingstekst die het doel en de locatie van de koppeling beschrijft.

Als u bijvoorbeeld koppelingstekst gebruikt zoals &quot;Klik hier&quot; of &quot;Meer lezen&quot;, wordt het doel van de koppeling niet duidelijk beschreven:

```html
<a href="product-site.html">Click here</a>
```

Als beste praktijken, zou u tekst moeten gebruiken die duidelijk beschrijft waar de verbinding gaat. Een beter voorbeeld zou de titel van de verbindingsbron en het doel kunnen gebruiken:

```html
<a href="product-site.html">Explore Product Site</a>
```

## Taal

Veel producten en services gebruiken taal op een creatieve of unieke manier. Vermijd jargon, lange zinnen en complexe zinnen. Gebruik een heldere, beknopte en goed leesbare taal die compatibel is met het doelpubliek.

- Gebruik waar mogelijk duidelijke beschrijvingen, inlinedefinities of verwante voorbeelden. Het kan moeilijk zijn om een uniek verticaal te vertalen.

- Spel uit of verbind met een definitie voor de eerste instanties van een acroniem of een afkorting. Het kan moeilijk zijn om afkortingen te vertalen.

- Gebruik waar mogelijk visuele elementen als aanvulling op tekst of complexe ideeën.
