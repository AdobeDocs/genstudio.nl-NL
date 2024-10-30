---
title: Opmerkingen bij de release van Adobe GenStudio for Performance Marketing Beta
description: Meer informatie over de nieuwste functies en verbeteringen voor Adobe GenStudio voor prestatiemarketing.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: bd3c5c9ff12c962d4123ac992fb74cd94e184172
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 2%

---

# Opmerkingen bij de release van Adobe GenStudio for Performance Marketing Beta

Deze nota&#39;s benadrukken significante correcties en verbeteringen van Adobe GenStudio for Performance Marketing voor de week die 4 oktober beëindigt.

## Nieuwe en verbeterde functies

* Filtermogelijkheden in het hele product zijn verbeterd. Problemen met filteren op leeftijd en geslacht in [!DNL Insights] zijn opgelost.  <!-- GS-1198 -->

* U kunt afbeeldingselementen (JPG of PNG) rechtstreeks bewerken met Adobe Express. Inhoudeditors kunnen het canvas van _[!UICONTROL Powered by Adobe Express]_gebruiken om achtergronden te verwijderen, generatieve vullingen toe te passen, effecten aan te passen en afbeeldingen uit te snijden zonder GenStudio for Performance Marketing te verlaten. <!-- GS-4615 -->

* Verbeterde ervaring met progressief laden voor gegenereerde varianten, gegenereerde e-mail en contextafhankelijke berichten. <!-- GS-4651 3062-->

* Inhoudeditors kunnen nu de functie Uitsnijden aanpassen gebruiken om gerenderde afbeeldingen in varianten uit te snijden. <!-- GS-2342 -->

* Problemen met vergroten/verkleinen en dupliceren van sjablonen zijn opgelost. <!-- GS-4895 -->

* Merkvalidatie verklaart nu de oorzaak van fouten die optreden tijdens validatie.

* Sjabloonvoorvertoningen geven nu de verwachte tekst op de afbeelding weer. <!-- GS-5917 -->

## Aanvullende verbeteringen en opgeloste problemen

* Met het canvas van [!DNL Create] worden nu aangepaste lettertypen op basis van sjablonen weergegeven zoals u had verwacht. <!-- GS-3415 -->

* Het juiste lettertype wordt nu toegepast tijdens het exporteren naar Meta. <!-- GS-5875 -->

* Problemen met het uploaden van een sjabloon die tot een succesvol uploaden hebben geleid, maar die niet zichtbaar zijn in de interface van het product, zijn opgelost. <!-- GS-4815 5650-->

* Gebruikers kunnen Meta-advertenties nu handmatig uitsnijden nadat ze zijn vergroot of verkleind. <!-- GS-5871 -->

* Gebruikers hoeven zich niet meer twee keer aan te melden bij een kanaal voor Meta-advertenties wanneer zij zich ook bij Facebook hebben aangemeld. <!-- GS-3009 -->

* De Canvasweergave van elementen en ervaringen blijft nu consistent tijdens het maken, beoordelen en goedkeuren van inhoud. <!-- GS-5877 -->

* Op het canvas worden nu slechts vier varianten weergegeven wanneer het canvas opnieuw wordt gegenereerd na een formaatbewerking. <!-- GS-5869 -->

* Op browsers gebaseerde spellingcontrole werkt nu zoals verwacht op het [!DNL Create] canvas. <!-- GS-5760 -->

* Weergaveadvertenties worden nu geëxporteerd als PNG-bestanden als **[!UICONTROL Export as PNG]** is geselecteerd. Eerder werden weergaveadvertenties als JPEG geëxporteerd toen de PNG-indeling werd geselecteerd. <!-- GS-5545 -->

* De opvulling is verhoogd tussen de knop **[!UICONTROL Manual crop]** en de knop **[!UICONTROL Generate]** . Eerder was de knop **[!UICONTROL Manual crop]** gedeeltelijk verborgen. <!-- GS-6084 -->

* In sjabloonvoorvertoningen worden nu naar behoren Google-lettertypen weergegeven. <!-- GS-5946 -->

* Geïmporteerde TypeKit- en Google-lettertypen worden nu volgens de verwachtingen geladen tijdens het exporteren. <!-- GS-5948 -->

* Oplossing voor problemen met het genereren van inhoud met aangepaste sjablonen. Eerder, toen een inhoudsredacteur probeerde om activa te produceren die een douanemalplaatje gebruiken, werd popup van de generatie niet getoond, en de console toonde fouten. <!-- GS-5262 -->

* Het DisplayAds-conceptcanvas behoudt nu zijn positie wanneer een gebruiker met de rechtermuisknop op het canvas klikt voordat hij of zij uit het contextmenu klikt. Eerder, verschoven het Canvas toen de gebruiker verlaten-klikte, die de ontwerp inhoud gedeeltelijk ontoegankelijk maakte.  <!-- GS-5687 -->

* Schimmereffecten blijven nu laden totdat de afbeelding opnieuw is gemaakt.  <!-- GS-5811 -->

* Merkvalidatiescore worden niet meer ongeldig nadat een gebruiker wijzigingen heeft aangebracht in gegenereerde e-mail, metaadvertenties of weergaveadvertenties. Eerder was deze score verborgen. <!-- GS-5379 -->

* Sjablonen waaraan CSS-stijlen zijn gekoppeld aan hun `body` -element, worden nu gebruikt zoals u had verwacht tijdens het exporteren van ervaringen. <!-- GS-5947 -->

* Correctie van problemen met het handmatig uitsnijden van afbeeldingen met grote afmetingen. <!-- GS-6039 -->

* Er wordt nu slechts één pop-upbericht weergegeven wanneer een gebruiker een nieuw element toevoegt in [!DNL Content] . <!-- GS-5020 -->

* Verbeterde Canvasprestaties tijdens het bewerken van tekst.  <!-- GS-5118 -->

* Ontbrekende spaties toegevoegd tussen tekenreeksen op het [!DNL Create] -e-mailadres of het Meta-canvas. <!-- GS-5019 -->

* Editors kunnen nu een bestand met namen die speciale tekens bevatten, opslaan na bewerking in Express. <!-- GS-6131 -->

### Lokalisatie

Deze release bevat verbeteringen voor lokalisatie in de hele productinterface, waaronder de volgende interfacegebieden:

* De URL voor het doel van de optie **[!UICONTROL Learn more]** in het [!DNL Create] prompt menu. <!-- GS-5029 -->

* Nummernotaties naast [!DNL Insights] > [!DNL Experience] Invoervelden zoeken. <!-- GS-4494 -->

## Bekend probleem

* Geregenereerde e-mailfragmenten verschijnen niet in de variant na selectie. (Varianten worden echter weergegeven nadat het concept opnieuw is geopend.) <!-- GS-5913 -->