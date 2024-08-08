---
title: Een e-mailsjabloon voorbereiden voor GenStudio
description: Leer hoe u een aangepaste e-mailsjabloon voor GenStudio maakt.
level: Intermediate
feature: Templates, Content
source-git-commit: 31f02218e02b1400ca9f32472acdecae03dbd304
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---


# E-mailsjabloon voorbereiden voor GenStudio

Doorgaans maakt een ontwerper het visuele ontwerp van een sjabloon in een ontwerpprogramma zoals Adobe XD. Nadat een e-mailsjabloon is ontworpen, gecodeerd en getest, kunt u het voorbereiden voor uploaden en gebruiken in GenStudio.

Zie [ Anatomie van een malplaatje ](/help/user-guide/content/use-templates.md#anatomy-of-a-template).

## Richtlijnen toevoegen

Alvorens u een Meta en malplaatje voorbereidt, zorg ervoor dat u [ richtlijnen ](/help/user-guide/guidelines/overview.md) aan uw GenStudio hebt toegevoegd en hen met uitvoerige info voor relevante merken bevolkt. De [ merkrichtlijnen ](/help/user-guide/guidelines/brands.md) beïnvloeden direct geproduceerde inhoud.

**Voorbeeld**: Als u het lichaam van een e-mailmalplaatje niet groter wilt zijn dan 500 karakters, voeg dat vereiste aan de [ kanaalrichtlijnen ](/help/user-guide/guidelines/brands.md#channel-guidelines) voor het &quot;lichaam&quot;gebied toe.

Als er geen richtlijnen aan GenStudio worden toegevoegd, worden standaardwaarden gebruikt.

## Een e-mailsjabloon coderen

Nadat een sjabloon is ontworpen, wordt deze gecodeerd met HTML en inline CSS. De code moet schoon zijn en reageren op verschillende apparaten.

Zie [ voorbeelden van het Malplaatje ](/help/user-guide/content/customize-template.md#template-examples).

## Een e-mailsjabloon testen

Test uw e-mailadres of testplatform om te controleren of deze correct wordt weergegeven op verschillende e-mailclients en apparaten.

Test of uw e-mailsjabloon voldoet aan het volgende:

* Layout past andere schermgrootten aan met CSS-mediaquery&#39;s
* U kunt op de knoppen klikken en naar de gewenste plaats navigeren
* De e-mailsjabloon is leesbaar en kan op mobiele apparaten worden gebruikt

## Gegenereerde inhoudsgebieden definiëren

Definieer de gebieden in uw e-mailsjabloon die dynamisch moeten worden gevuld met inhoud uit GenStudio.

gegenereerde inhoudsgebieden definiëren:

* Identificeer de tekstelementen in de sjabloon die GenStudio automatisch moet genereren, zoals de kop of CTA.
* Pas de HTML-sjabloon aan door er plaatsaanduidingen in op te nemen met behulp van de syntaxis Handblebars.

Zie [ placeholders van de Inhoud ](/help/user-guide/content/customize-template.md#content-placeholders).

## Een voorbeeld van de sjabloon bekijken

U kunt de zichtbaarheid van bepaalde inhoudsgebieden bepalen met behulp van ingebouwde hulpmiddelen. U kunt bijvoorbeeld parameters voor het bijhouden van koppelingen opnemen in een geëxporteerde sjabloon terwijl er geen voorvertoningskoppelingen zijn.

Zie [ de voorproef van het Malplaatje ](/help/user-guide/content/customize-template.md#template-preview).

## Sjabloon uploaden en gebruiken

Nadat uw sjabloon is ontworpen, gecodeerd, getest en bekeken, kunt u deze uploaden naar GenStudio voor gebruik bij het genereren van gloednieuwe marketinginhoud.

Zie [ Werkend met malplaatjes ](use-templates.md).
