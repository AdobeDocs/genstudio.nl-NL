---
title: Opmerkingen bij de release Adobe GenStudio voor Performance Marketers Beta
description: Leer meer over de nieuwste functies en verbeteringen op het gebied van Adobe GenStudio.
source-git-commit: 5505e3fdc78e217dd1eb73ed5bffa5e43d4f3084
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---


# Opmerkingen bij de release Adobe GenStudio voor Performance Marketers Beta

Deze nota&#39;s benadrukken significante correcties en verhogingen van de Adobe GenStudio voor de week die 16 augustus beëindigt.

## Hooglichten

De ontwikkeling van GenStudio-functies verloopt snel en continu. De opmerkelijke nieuwe eigenschappen omvatten:

### Merk

Het deelvenster Merkvalidatie is uitgebreid om de gebruikerservaring te verbeteren, inclusief de volgende wijzigingen:

* _op percentage-gebaseerde bevestigingsscore_: De bevestiging van het merk toont nu de score van de brandbevestiging als percentage eerder dan een pas/ontbreekt waarde.

* _bijgewerkte de extractieinterface van het Merk_: De extractie van het merk toont nu voltooiing van het extractieproces als percentage.

* _Incrementele merklading tijdens extractie_: De richtlijnen van het merk worden nu incrementeel geladen in het gebruikersinterface.

* _Vereenvoudiging van het schema van de Richtsnoer van het Exemplaar_: Het `unique attributes` en `frequent keywords` gebied zijn verwijderd uit het schema van de Richtsnoer van het Exemplaar, dat het richtsnoer op proces vereenvoudigt.

### Maken

* **Multi-section e-mailverwezenlijking**: De gebruikers kunnen e-mails nu tot stand brengen die uit afzonderlijke titel, beeld, lichaam, en de elementen van CTA worden samengesteld.

* **Meta Adds Resize**: De scheppers kunnen Meta en aspectverhoudingen resize.

### Inzichten

* **Beperkte Inzicht login rekeningen**: Inzicht login steunt nu slechts één rekening per klant.

## Verbeteringen en opgeloste problemen

Deze release bevat de volgende aanvullende oplossingen.

### Inzichten

* De _naam van de de paginadebietplaatsing van het Detail van de Ervaring_ specificeert nu de voer van Facebook of van Instagram.

* Het snijden van grotere beelden en video is nu verenigbaar wanneer de gebruiker van de _mening van het Overzicht van Activa 0} {aan de_ mening van het Activa detail _navigeert._

* Het aantal zoekresultaten op het scherm Kenmerken wordt niet langer weergegeven `0 of` voordat een gebruiker zich aanmeldt. <!-- GS- 3665 -->

* Wanneer u op het veld **[!UICONTROL Insight]** > **[!UICONTROL Asset]** aantal klikt, worden de zoek- en filterinstellingen niet meer gewist. <!-- GS-3476 -->

## Bekende problemen

De volgende bekende problemen worden opgelost door de GenStudio for Performance Marketers GA-release.

### Analyse

* Acties die door de knoppen **[!UICONTROL Add templates]** en **[!UICONTROL Upload]** worden geactiveerd, worden momenteel niet bijgehouden. <!-- GS-3505 -->

### Inzichten

* De video&#39;s kunnen niet van _Assets_ worden gespeeld. <!-- GS-3846 -->

* Gebruikers moeten zich twee keer aanmelden wanneer ze zich ook bij Facebook hebben aangemeld. **Oplossing**: logout van Facebook alvorens het programma te openen in Inzichten.

* **uitgaven op het niveau van de Campagne** waarden zijn niet nauwkeurig. De gegevens zijn momenteel niet consistent tussen Facebook Ads Manager en het datumpigment. <!-- GS-3202 -->

### Revisies en goedkeuringen

* Maker kan elementen na goedkeuring vóór publicatie wijzigen. De fiatteurs worden niet van deze wijzigingen in kennis gesteld.

