---
title: Opmerkingen bij de release Adobe GenStudio voor Performance Marketers Beta
description: Meer informatie over de nieuwste functies en verbeteringen in de Adobe GenStudio voor Performance Marketers.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 7085fa5a12a6ed36c9310f8f691969d9c1366d36
workflow-type: tm+mt
source-wordcount: '1341'
ht-degree: 0%

---

# Opmerkingen bij de release Adobe GenStudio voor Performance Marketers Beta

Deze nota&#39;s benadrukken significante Adobe GenStudio voor de fixes en de verhogingen van de Marketers van Prestaties voor de week die 19 september beëindigt.

## Nieuwe en verbeterde functies

* **Integratie met Adobe Experience Manager Assets**. Alleen-lezen toegang tot Adobe Experience Manager Assets is nu beschikbaar. <!-- GS-2432 -->

* **Verbeteringen aan het werkschema van het Malplaatje van de Update**.  Gebruikers die sjablonen bijwerken, selecteren nu het kanaal waarvoor zij de sjabloon willen gebruiken. <!-- GS-4029 -->

* **Verbeterde creeer de prestaties van de paginalading**. Ongebruikte afhankelijkheden zijn verwijderd uit het laadproces van de pagina. <!-- GS-3630 -->

* **multi-sectie e-mailsteun**. Editors kunnen nu e-mailberichten genereren die meerdere secties en afbeeldingen bevatten. Ze kunnen ook specifieke fragmenten van een gegenereerde e-mail opnieuw genereren (bijvoorbeeld een kop). <!-- GS-2436 -->

* **knevel tussen Desktop en mobiele mening tijdens verwezenlijking**. Gebruikers kunnen nu schakelen tussen de weergave voor desktops en mobiele apparaten om een voorvertoning van de verschillende e-mailervaringen weer te geven. <!-- GS-4314 -->

* Met Inhoud worden nu afbeeldingen gegenereerd met uitsnijdafmetingen die relatief zijn ten opzichte van de oorspronkelijke elementafmetingen. <!-- GS-3150 -->

* Gebruikers kunnen nu gegenereerde afbeeldingsvarianten selecteren en deze uitsnijden tijdens de ontwerpworkflow met de functie Uitsnijden aanpassen. <!-- GS-5538 2342 -->

* In de weergave Details van een goedgekeurde ervaring worden nu een miniatuurafbeelding en de status van alle elementen weergegeven waarnaar in die ervaring wordt verwezen. <!-- GS-3783 -->

## Bekende problemen

De volgende bekende problemen zullen worden opgelost in de GenStudio for Performance Marketers GA-release.

* Problemen met intermitterende latentie zijn van invloed op bepaalde Canvasbewerkingen van [!DNL Create] . <!-- GS-5203 -->

* E-mailgeneratie resulteert in een onvolledig e-mailbericht. **Oplossing**: vernieuw de pagina en regenerate. <!-- GS-5209 -->

* Sjablonen kunnen worden geüpload, maar niet worden weergegeven. **Oplossing**: Upload activa met het **[!UICONTROL Campaigns]** bevolkte gebied. Vervolgens uploadt u de sjabloon opnieuw. <!-- GS-4815 -->

* Gebruikers moeten zich twee keer aanmelden bij een kanaal voor Meta-advertenties wanneer zij zich ook bij Facebook hebben aangemeld. **Oplossing**: Logout van Facebook alvorens het programma te openen in de advertenties van het kanaalMeta. <!-- GS-4806 -->

### Aanvullende verbeteringen en opgeloste problemen

* Slepen en neerzetten werkt nu zoals u had verwacht in het snelle gebied. <!-- GS-3977 -->

* Correctie van problemen met het gebruik van de Tab-toets om door elementen op de linkernavigatiebalk te navigeren. Eerder, waren de veelvoudige kliks nodig om van één element aan het volgende actieve element te navigeren.  <!-- GS-2639 -->

* GenStudio slaat nu ervaringsnamen op wanneer gebruikers de naam bewerken terwijl de ervaring wordt geladen. <!-- GS-5242 -->

* Gebruikers kunnen nu een ervaringstitel bewerken. Eerder werd de titeltekst standaard ingesteld op de originele tekst nadat een gebruiker had geprobeerd deze te bewerken. <!-- GS-5246 -->
* Geselecteerde afbeeldingen worden nu op het canvas gerenderd zoals u had verwacht tijdens het maken van meerdelige e-mail. <!-- GS-5263 -->

* Alle tekenreeksen op de detailpagina [!DNL Content] Ervaring zijn nu gelokaliseerd. <!-- GS-5016 -->

* Gebruikers kunnen nu een product verwijderen waarvan de detailweergave wordt geopend in [!DNL Products] . <!-- GS-5057 -->

* Het bericht dat GenStudio weergeeft wanneer een zoekopdracht geen overeenkomende resultaten oplevert, is verbeterd. <!-- GS-4544 -->

* `aria-label` -kenmerkwaarden voor waarden van zoekfilters worden nu naar behoren omgezet. <!-- GS-5388 -->

* Gebruikers kunnen nu dubbele elementen verwijderen in het gebied met [!DNL Create] Canvas-vragen.  <!-- GS-5233 -->

* Het accountfilter werkt nu zoals u had verwacht met ervaringen, elementen en kenmerken. <!-- GS-4812 -->

* Problemen met lettertypen op Meta-advertentiesjablonen zijn opgelost om de leesbaarheid en toegankelijkheid te verbeteren. <!-- GS-5354 -->

* Wijzigingen in concepttitels blijven nu op de verwachte manier behouden. Eerder werden titels na bewerking teruggezet naar de standaardnaam. <!-- GS-2951 -->

#### Sjablooncorrecties

* De functie voor vergroten/verkleinen werkt nu zoals u had verwacht bij meerdere afbeeldingen in Meta-advertentiesjablonen. Eerder heeft GenStudio de grootte van afbeeldingen voor alle geselecteerde sjablonen niet gewijzigd. <!-- GS-4696 -->

* Als u een sjabloon verwijdert, wordt de pagina van [!DNL Content] nu naar behoren vernieuwd. <!-- GS-5397 -->

* Gebruikers kunnen nu alleen waarden voor [!DNL Personas] , [!DNL Brands] of [!DNL Products] kiezen in het vervolgkeuzemenu. Eerder, uploadt het _Malplaatje_ dialoog laat gebruikers om het even welke [!DNL Persona], [!DNL Brand], of [!DNL Product] naam ingaan. <!-- GS-5072 5071-->

* De knop **[!UICONTROL Back]** is nu uitgeschakeld tijdens het uploaden van een sjabloon. <!-- GS-5358 -->

* Alle tekenreeksen in de weergave Sjabloondetails selecteren van [!DNL Create] zijn nu gelokaliseerd. <!-- GS-5025 -->

## Vorige Beta-releases

In vorige Beta-releases waren de volgende markeringen en oplossingen opgenomen.

### Hooglichten

* De inhoudskiezer van [!DNL Create] is vernieuwd om het laden van elementen te verbeteren. <!-- GS-2586 -->

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

* **Metaadvertenties Resize**: De redacteurs kunnen Meta en aspectverhoudingen resize. (vaste 8/16)

* **Beperkte [!DNL Insights] login rekeningen**: [!DNL Insights] login steunt nu slechts één rekening per klant. (vaste 8/16)

### Extra verbeteringen en vaste problemen

* Met het canvas van [!DNL Create] worden afbeeldingen nu correct weergegeven in metagegevensadvertenties. (vast 9/13) <!-- GS-4864 -->

* Hoewel er verschillen kunnen bestaan tussen voorvertoningen van Meta-advertenties en geëxporteerde weergaven, werken geëxporteerde ervaringen goed. (vast 9/13) <!-- GS-4492 4401 -->

* Geüploade afbeeldingen bevatten nu de verwachte slimme tags. (vast 9/13) <!-- GS-4856 -->

* Het CSV-bestand voor Meta-advertenties bevat nu naar verwachting afbeeldingen. Eerder bevatte het ZIP-bestand het CSV-exportbestand en NULL-bestanden in plaats van afbeeldingen. (vast 9/13) <!-- GS-5107 -->

* Gebruikers kunnen nu naar behoren tekst invoeren in het veld Sjabloondetailweergave **[!UICONTROL Uploaded by]** . Voorheen kon het ladingspictogram gebruikers geen tekst invoeren. (vast 9/13) <!-- GS-4887 -->

* Gebruikers worden niet meer omgeleid naar de detailweergave van een merk nadat het merk is verwijderd. (vast 9/13) <!-- GS-2663 -->

* Editors ontvangen niet langer de volgende fout wanneer ze variabelen ter controle en goedkeuring verzenden: `You have no access to view comments on this Object` . (vast 9/13) <!-- GS-5140 -->

* De e-mailsjabloon bijgewerkt in de workflow voor revisie en goedkeuring. (vast 9/13) <!-- GS-5239 -->

* GenStudio geeft nu een foutbericht weer wanneer er een netwerkfout optreedt tijdens het laden van de sjabloonkiezer. (vast 9/13) <!-- GS-4682 -->

* Oplossing voor problemen met het navigeren van een element, ervaring of sjabloonkaart naar het geselecteerde object. (vast 9/13) <!-- GS-4390 -->

* _voeg Assets_ popup toe wordt nu gelokaliseerd wanneer geopend van Create Canvas. (vast 9/13) <!-- GS-4867 -->

* Merkvalidatie wordt nu geactiveerd voor opnieuw gegenereerde varianten. Als een editor eerder varianten van een bestaand concept opnieuw genereerde, werd de validatie niet gestart. (vast 9/13) <!-- GS-3971 -->

* _voeg Assets_ popup toe wordt nu gelokaliseerd zoals verwacht. (vast 9/5) <!-- GS-3834 -->

* Problemen met het schalen van de ervaringssjabloon Meta-advertenties zijn opgelost. (vast 9/5) <!-- GS-4174 -->

* De tekstvelden in het CSV-exportbestand voor e-mails met meerdere onderdelen worden nu op de verwachte manier geordend. (vast 9/5) <!-- GS-4013 -->

* Het [!DNL Content] onderzoeksgebied verdwijnt niet meer wanneer een gebruiker herhaaldelijk op de **Backspace** sleutel duwt om de tekst van het onderzoeksgebied te wissen. (vast 9/5) <!-- GS-4543 -->

* GenStudio for Performance Marketers laadt nu de gebruikers zoals verwacht wanneer een medewerker een `@` -vermelding aan een opmerking toevoegt. Eerder werden gebruikers niet geladen en werd een fout weergegeven: `Unable to load users. Refresh the page` . (vast 8/29) <!-- GS-4113 -->

* GenStudio toont niet meer het **Iets ging fout** bericht wanneer een redacteur **Uitgezochte inhoud** tijdens e-mailverwezenlijking in het snelle gebied klikt. <!-- GS-4879 -->

* De _naam van de de paginadebietplaatsing van het Detail van de Ervaring_ specificeert nu de voer van Facebook of van Instagram. (vaste 8/16)

* Het snijden van grotere beelden en video is nu verenigbaar wanneer de gebruiker van de _mening van het Overzicht van het Middel 0} {aan de_ mening van het Detail van Activa _navigeert._ (vaste 8/16)

* Het aantal zoekresultaten op het scherm Kenmerken wordt niet langer weergegeven `0 of` voordat een gebruiker zich aanmeldt. (vast 8/16) <!-- GS-3665 -->

* Wanneer u op het veld **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Asset]** aantal klikt, worden de zoek- en filterinstellingen niet meer gewist. (vast 8/16) <!-- GS-3476 -->

* GenStudio geeft een fout weer wanneer een gebruiker referenties probeert in te voeren in de weergave [!DNL Insights] . (vast 8/29) <!-- GS-4689 -->

* Het uploaden van merkrichtlijnen mislukt vanwege problemen met het ACS-opslagplatform. (vast 8/22) <!-- GS-4369 -->

* In het vervolgkeuzemenu Vragen [!DNL Brands] wordt een spinner aan het einde van de lijst in [!DNL Brands] weergegeven tijdens het maken van e-mail. (vast 8/22) <!-- GS-4077 -->
