---
title: Opmerkingen bij de release Adobe GenStudio voor Performance Marketers Beta
description: Meer informatie over de nieuwste functies en verbeteringen in de Adobe GenStudio voor Performance Marketers.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 5f729070a3a4c162ebac0fde9814c649c9984b4d
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 0%

---

# Opmerkingen bij de release Adobe GenStudio voor Performance Marketers Beta

Deze nota&#39;s benadrukken significante Adobe GenStudio voor de fixes en de verhogingen van de Marketers van Prestaties voor de week die 13 september beëindigt.

## Verbeteringen

* De inhoudskiezer van [!DNL Create] is vernieuwd om het laden van elementen te verbeteren. <!-- GS-2586 -->

## Bekende problemen

De volgende bekende problemen zullen worden opgelost in de GenStudio for Performance Marketers GA-release.

* Problemen met intermitterende latentie zijn van invloed op bepaalde Canvasbewerkingen van [!DNL Create] . <!-- GS-5203 -->

* E-mailgeneratie resulteert in een onvolledig e-mailbericht. **Oplossing**: vernieuw de pagina en regenerate. <!-- GS-5209 -->

* Sjablonen kunnen worden geüpload, maar niet worden weergegeven. **Oplossing**: Creeer of upload activa en ga een naam van de activagroep op het **[!UICONTROL Campaigns]** gebied in. Als u het element toewijst aan een [!DNL Campaign] , wordt de metagegevenswaarde voor de groepsnaam toegevoegd. Vervolgens uploadt u de sjabloon opnieuw. <!-- GS-4815 -->

* Campagneminiaturen ontbreken in [!DNL Insights] . <!-- GS-4648 -->

* Gebruikers moeten zich twee keer aanmelden bij een kanaal voor Meta Ads-account wanneer zij zich ook bij Facebook hebben aangemeld. **Oplossing**: Logout van Facebook alvorens het programma te openen in een rekening van de Advertentie van het kanaal Meta. <!-- GS-4806 -->

### Aanvullende verbeteringen en opgeloste problemen

* Met het canvas [!DNL Create] worden afbeeldingen in Metaadvertenties onjuist weergegeven. <!-- GS-4864 -->

* Hoewel er verschillen kunnen bestaan tussen voorvertoningen van Meta Ads Canvas en geëxporteerde weergaven, werken geëxporteerde ervaringen goed. <!-- GS-4492 4401 -->

* Geüploade afbeeldingen bevatten niet altijd de verwachte slimme tags. <!-- GS-4856 -->

* Het CSV-bestand voor metagegevens en exporteren bevat nu naar behoren afbeeldingen. Eerder bevatte het ZIP-bestand het CSV-exportbestand en NULL-bestanden in plaats van afbeeldingen.  <!-- GS-5107 -->

* Gebruikers kunnen nu naar behoren tekst invoeren in het veld Sjabloondetailweergave **[!UICONTROL Uploaded by]** . Voorheen kon het ladingspictogram gebruikers geen tekst invoeren. <!-- GS-4887 -->

* Gebruikers worden niet meer omgeleid naar de detailweergave van een merk nadat het merk is verwijderd. <!-- GS-2663 -->

* Editors ontvangen niet langer de volgende fout wanneer ze variabelen ter controle en goedkeuring verzenden: `You have no access to view comments on this Object` . <!-- GS-5140 -->

* De e-mailsjabloon bijgewerkt in de workflow voor revisie en goedkeuring. <!-- GS-5239 -->

* GenStudio geeft nu een foutbericht weer wanneer er een netwerkfout optreedt tijdens het laden van de sjabloonkiezer. <!-- GS-4682 -->

* Oplossing voor problemen met het navigeren van een element, ervaring of sjabloonkaart naar het geselecteerde object. <!-- GS-4390 -->

* _voeg Assets_ popup toe wordt nu gelokaliseerd wanneer geopend van Create Canvas.  <!-- GS-4867 -->

* Merkvalidatie wordt nu geactiveerd voor opnieuw gegenereerde varianten. Als een editor eerder varianten van een bestaand concept opnieuw genereerde, werd de validatie niet gestart. <!-- GS-3971 -->

## Vorige Beta-releases

In vorige Beta-releases waren de volgende markeringen en oplossingen opgenomen.

### Hooglichten

* GenStudio biedt nu ondersteuning voor de optie om een voorvertoning van media-elementen weer te geven in tabel- en galerieweergaven van [!DNL Insights] . De videoduimnagels omvatten a **Spel** knoop met een dempingsoptie. <!-- GS-4398 -->

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

* **MetaAds Resize**: De redacteurs kunnen breedte/hoogteverhoudingen resize MetaAd. (vaste 8/16)

* **Beperkte [!DNL Insights] login rekeningen**: [!DNL Insights] login steunt nu slechts één rekening per klant. (vaste 8/16)

### Extra verbeteringen en vaste problemen

* _voeg Assets_ popup toe wordt nu gelokaliseerd zoals verwacht. <!-- GS-3834 -->

* Problemen met het schalen van de ervaringssjabloon Meta-advertenties zijn opgelost. <!-- GS-4174 -->

* De tekstvelden in het CSV-exportbestand voor e-mails met meerdere onderdelen worden nu op de verwachte manier geordend. <!-- GS-4013 -->

* Het [!DNL Content] onderzoeksgebied verdwijnt niet meer wanneer een gebruiker herhaaldelijk op de **Backspace** sleutel duwt om de tekst van het onderzoeksgebied te wissen.  <!-- GS-4543 -->

* GenStudio for Performance Marketers laadt nu de gebruikers zoals verwacht wanneer een medewerker een `@` -vermelding aan een opmerking toevoegt. Eerder werden gebruikers niet geladen en werd een fout weergegeven: `Unable to load users. Refresh the page` . <!-- GS-4113 -->

* GenStudio toont niet meer het **Iets ging fout** bericht wanneer een redacteur **Uitgezochte inhoud** tijdens e-mailverwezenlijking in het snelle gebied klikt. <!-- GS-4879 -->

* De _naam van de de paginadebietplaatsing van het Detail van de Ervaring_ specificeert nu de voer van Facebook of van Instagram. (vaste 8/16)

* Het snijden van grotere beelden en video is nu verenigbaar wanneer de gebruiker van de _mening van het Overzicht van het Middel 0} {aan de_ mening van het Detail van Activa _navigeert._ (vaste 8/16)

* Het aantal zoekresultaten op het scherm Kenmerken wordt niet langer weergegeven `0 of` voordat een gebruiker zich aanmeldt. (vast 8/16) <!-- GS-3665 -->

* Wanneer u op het veld **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Asset]** aantal klikt, worden de zoek- en filterinstellingen niet meer gewist. (vast 8/16) <!-- GS-3476 -->

* GenStudio geeft een fout weer wanneer een gebruiker referenties probeert in te voeren in de weergave [!DNL Insights] . (vast 8/29) <!-- GS-4689 -->

* Het uploaden van merkrichtlijnen mislukt vanwege problemen met het ACS-opslagplatform. (vast 8/22) <!-- GS-4369 -->

* In het vervolgkeuzemenu Vragen [!DNL Brands] wordt een spinner aan het einde van de lijst in [!DNL Brands] weergegeven tijdens het maken van e-mail. (vast 8/22) <!-- GS-4077 -->
