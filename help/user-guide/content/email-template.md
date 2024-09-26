---
title: Een e-mailsjabloon voorbereiden voor Adobe GenStudio voor prestatieverkopers
description: Leer hoe u een aangepaste e-mailsjabloon maakt voor Adobe GenStudio voor prestatieverkopers.
level: Intermediate
feature: Templates, Content
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 58833ed0c8e28061ab2584b7949f2a0cbd3d10cc
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# E-mailsjabloon voorbereiden voor Adobe GenStudio voor prestatieverkopers

Doorgaans maakt een ontwerper het visuele ontwerp van een sjabloon in een ontwerpprogramma zoals Adobe XD. Nadat een e-mailsjabloon is ontworpen, gecodeerd en getest, kunt u het voorbereiden voor uploaden en gebruiken in GenStudio for Performance Marketers.

Zie [ elementen van het Malplaatje ](use-templates.md#template-elements).

## Richtlijnen toevoegen

Alvorens u een Meta en malplaatje voorbereidt, zorg ervoor dat u [ richtlijnen ](/help/user-guide/guidelines/overview.md) aan uw GenStudio voor de Marketers van Prestaties hebt toegevoegd en hen met uitvoerige info voor relevante merken bevolkt. De [ merkrichtlijnen ](/help/user-guide/guidelines/brands.md) beïnvloeden direct geproduceerde inhoud.

**Voorbeeld**: Als u het lichaam van een e-mailmalplaatje niet groter wilt zijn dan 500 karakters, voeg dat vereiste aan de [ kanaalrichtlijnen ](/help/user-guide/guidelines/brands.md#channel-guidelines) voor het &quot;lichaam&quot;gebied toe.

Als er geen richtlijnen worden toegevoegd aan GenStudio for Performance Marketers, worden standaardwaarden gebruikt.

## Een e-mailsjabloon coderen

Nadat een sjabloon is ontworpen, wordt deze gecodeerd met HTML en inline CSS. De code moet schoon zijn en reageren op verschillende apparaten.

Zie [ voorbeelden van het Malplaatje ](/help/user-guide/content/customize-template.md#template-examples).

### E-mails met meerdere secties

U kunt [ gestructureerde herinneringen ](/help/user-guide/effective-prompts.md#structured-prompts) tijdens inhoudsgeneratie gebruiken om GenStudio for Performance Marketing op te dragen om variërende inhoud per sectie van een e-mail te produceren.

Bijvoorbeeld, als de secties in uw e-mailmalplaatje met `Pod` `Pod1` en `Pod2` vooraf worden bepaald, kan de gestructureerde herinnering voor inhoudsgeneratie specifieke richtlijnen voor die e-mailsecties omvatten. GenStudio for Performance Marketing komt overeen met de sectiespecifieke instructie in uw vraag naar de bijbehorende e-mailsectie en genereert inhoud die is uitgelijnd met de instructies.

Zie [ Gestructureerde herinneringen ](/help/user-guide/effective-prompts.md#structured-prompts).

## Een e-mailsjabloon testen

Test uw e-mailadres of testplatform om te controleren of deze correct wordt weergegeven op verschillende e-mailclients en apparaten.

Test of uw e-mailsjabloon voldoet aan het volgende:

* Layout past andere schermgrootten aan met CSS-mediaquery&#39;s
* U kunt op de knoppen klikken en naar de gewenste plaats navigeren
* De e-mailsjabloon is leesbaar en kan op mobiele apparaten worden gebruikt

## Gegenereerde inhoudsgebieden definiëren

Definieer de gebieden in uw e-mailsjabloon die dynamisch moeten worden gevuld met inhoud van GenStudio for Performance Marketers.

gegenereerde inhoudsgebieden definiëren:

* Identificeer de tekstelementen in het malplaatje dat GenStudio for Performance Marketers zou moeten auto-produceren, zoals de titel of CTA.
* Pas de HTML-sjabloon aan door er plaatsaanduidingen in op te nemen met behulp van de syntaxis Handlebars.

Zie [ placeholders van de Inhoud ](/help/user-guide/content/customize-template.md#content-placeholders).

## Een voorbeeld van de sjabloon bekijken

De zichtbaarheid van specifieke inhoudsgebieden bepalen met ingebouwde hulp. U kunt bijvoorbeeld parameters voor het bijhouden van koppelingen opnemen in een geëxporteerde sjabloon terwijl er geen voorvertoningskoppelingen zijn.

Zie [ de voorproef van het Malplaatje ](/help/user-guide/content/customize-template.md#template-preview).

## Sjabloon uploaden en gebruiken

Nadat uw sjabloon is ontworpen, gecodeerd, getest en bekeken, kunt u deze uploaden naar GenStudio for Performance Marketers voor gebruik bij het genereren van gloednieuwe marketinginhoud.

Zie [ Werkend met malplaatjes ](use-templates.md).
