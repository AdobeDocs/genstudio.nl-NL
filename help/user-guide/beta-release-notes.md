---
title: Opmerkingen bij de release Adobe GenStudio voor Performance Marketers Beta
description: Meer informatie over de nieuwste functies en verbeteringen in de Adobe GenStudio voor Performance Marketers.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 62793ab56b635f17e037b63beb56c09ff2d45621
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---

# Opmerkingen bij de release Adobe GenStudio voor Performance Marketers Beta

Deze nota&#39;s benadrukken significante Adobe GenStudio voor de fixes en de verhogingen van de Marketers van Prestaties voor de week die 6 september beëindigt.

## Nieuwe functies

* GenStudio biedt nu ondersteuning voor de optie om een voorvertoning van media-elementen weer te geven in tabel- en galerieweergaven van [!DNL Insights] . De videoduimnagels omvatten a **Spel** knoop met een dempingsoptie. <!-- GS-4398 -->

## Bekende problemen

De volgende bekende problemen zullen worden opgelost in de GenStudio for Performance Marketers GA-release.

* Editors krijgen soms een foutbericht &#39;Er is iets fout gegaan&#39; op de [!DNL Create Canvas] tijdens het genereren van de afbeelding. **Oplossing**: Als de fout zich herhaalt, kan de gebruiker logout, dan login aan GenStudio en regenerate het beeld.  <!-- GS-4813 -->

* De [!DNL Create Canvas] rendert afbeeldingen in Meta-advertenties onjuist. <!-- GS-4864 -->

* Assets zonder campagnes kan worden geüpload naar [!DNL Content] , maar is mogelijk niet zichtbaar voor gebruikers. <!-- GS-4815 -->

* Er is een verschil tussen voorvertoningen van MetaAds Canvas en geëxporteerde weergaven. <!-- GS-4492 4401 -->

* Campagneminiaturen ontbreken in [!DNL Insights] . <!-- GS-4648 -->

* Gebruikers kunnen momenteel kleine elementen selecteren waarvan het formaat moet worden gewijzigd, maar het vergroten van deze elementen wordt niet ondersteund. <!-- GS-3131 -->

* Gebruikers moeten zich twee keer aanmelden bij een kanaal voor Meta Ads-account wanneer zij zich ook bij Facebook hebben aangemeld. **Oplossing**: Logout van Facebook alvorens het programma te openen in een rekening van de Advertentie van het kanaal Meta.

* Geüploade afbeeldingen bevatten niet altijd de verwachte slimme tags. <!-- GS-4856 -->

### Extra verbeteringen en vaste problemen

* _voeg Assets_ popup toe wordt nu gelokaliseerd zoals verwacht. <!-- GS-3834 -->

* Problemen met het schalen van de ervaringssjabloon Meta-advertenties zijn opgelost. <!-- GS-4174 -->

* Inhoudsfragmentmodellen die voor sjablonen zijn gemaakt, kunnen nu op de juiste wijze in AEM worden weergegeven. <!-- GS-4716 -->

* De tekstvelden in het CSV-exportbestand voor e-mails met meerdere onderdelen worden nu op de verwachte manier geordend. <!-- GS-4013 -->

* Het [!DNL Content] onderzoeksgebied verdwijnt niet meer wanneer een gebruiker herhaaldelijk op de **Backspace** sleutel duwt om de tekst van het onderzoeksgebied te wissen.  <!-- GS-4543 -->

* GenStudio laadt nu gebruikers zoals verwacht wanneer een medewerker een @-vermelding toevoegt aan een opmerking. Eerder heeft GenStudio geen gebruikers geladen en deze fout weergegeven: `Unable to load users. Refresh the page` . <!-- GS-4113 -->

* GenStudio toont niet meer het **Iets ging fout** bericht wanneer een redacteur **Uitgezochte inhoud** tijdens e-mailverwezenlijking in het snelle gebied klikt. <!-- GS-4879 -->

## Vorige Beta-releases

In vorige Beta-releases waren de volgende markeringen en oplossingen opgenomen.

### Hooglichten

* De richtlijnen voor instagram en Facebook Channel zijn gecombineerd tot de merkrichtlijnen voor Meta.

* [!DNL Create] Canvasnavigatie-elementen zijn gestroomlijnd. Op de landingspagina van [!DNL Create] wordt het navigatievenster links weergegeven, maar gebruikers gebruiken nu een **[!UICONTROL Back]** -knop om vanuit andere [!DNL Create] werkgebieden naar deze ruimte te navigeren.

* Navigatie-elementen zijn verbeterd om de aandacht van de gebruiker te ondersteunen bij het uitvoeren van taken in het gehele product, waaronder de volgende productgebieden:

   * Informatie over middelen, ervaring en sjablonen in [!DNL Content]
   * Ervaring, element, kenmerkdetails in [!DNL Insights]
   * Merk details in [!DNL Brands]
   * Productgegevens en persoonlijke gegevens in producten en personen

* Gebruikers hoeven niet meer op de knop **[!UICONTROL Refresh]** te klikken om updates van Ervaringen in [!DNL Content] weer te geven.

* De _pagina van de Details van de Ervaring_ geeft nu externe activaduimnagels als HTML terug.

* De vertraging van de gebruikersinterface na het toevoegen of verwijderen van Assets en Ervaringen is verbeterd.

* Sjabloonvoorvertoningen bevatten nu beschrijvende standaardtekst. Zie [ een malplaatje ](https://experienceleague.adobe.com/en/docs/genstudio/user-guide/content/templates/customize-template#template-preview) aanpassen.

* **op percentage-gebaseerde bevestigingsscore**: De bevestiging van het merk toont nu de score van de brandbevestiging als percentage eerder dan een pas/ontbreekt waarde. (vaste 8/16)

* **bijgewerkte de extractieinterface van het Merk**: De extractie van het merk toont nu voltooiing van het extractieproces als percentage. (vaste 8/16)

* **Incrementele merklading tijdens extractie**: De richtlijnen van het merk worden nu incrementeel geladen in het gebruikersinterface. (vaste 8/16)

* **Multi-section e-mailverwezenlijking**: De gebruikers kunnen e-mails nu tot stand brengen die uit afzonderlijke titel, beeld, lichaam, en de elementen van CTA worden samengesteld. (vaste 8/16)

* **Meta Adds Resize**: De redacteurs kunnen Meta en aspectverhoudingen resize. (vaste 8/16)

* **Beperkte [!DNL Insights] login rekeningen**: [!DNL Insights] login steunt nu slechts één rekening per klant. (vaste 8/16)

### Extra verbeteringen en vaste problemen

* De _naam van de de paginadebietplaatsing van het Detail van de Ervaring_ specificeert nu de voer van Facebook of van Instagram. (vaste 8/16)

* Het snijden van grotere beelden en video is nu verenigbaar wanneer de gebruiker van de _mening van het Overzicht van het Middel 0} {aan de_ mening van het Detail van Activa _navigeert._ (vaste 8/16)

* Het aantal zoekresultaten op het scherm Kenmerken wordt niet langer weergegeven `0 of` voordat een gebruiker zich aanmeldt. (vast 8/16) <!-- GS-3665 -->

* Wanneer u op het veld **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Asset]** aantal klikt, worden de zoek- en filterinstellingen niet meer gewist. (vast 8/16) <!-- GS-3476 -->

### Bekende problemen opgelost in eerdere Beta-releases

* GenStudio geeft een fout weer wanneer een gebruiker referenties probeert in te voeren in de weergave [!DNL Insights] . (vast 8/29) <!-- GS-4689 -->

* Het uploaden van merkrichtlijnen mislukt vanwege problemen met het ACS-opslagplatform. (vast 8/22) <!-- GS-4369 -->

* In het vervolgkeuzemenu Vragen [!DNL Brands] wordt een spinner aan het einde van de lijst in [!DNL Brands] weergegeven tijdens het maken van e-mail. (vast 8/22) <!-- GS-4077 -->
