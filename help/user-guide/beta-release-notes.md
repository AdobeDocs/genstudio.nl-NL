---
title: Opmerkingen bij de release Adobe GenStudio voor Performance Marketers Beta
description: Meer informatie over de nieuwste functies en verbeteringen in de Adobe GenStudio voor Performance Marketers.
source-git-commit: cbae3aeb1b8282fb64f2a6405a7ad9e07a48dbbd
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---


# Opmerkingen bij de release Adobe GenStudio voor Performance Marketers Beta

Deze nota&#39;s benadrukken significante correcties en verhogingen van de Adobe GenStudio voor de week die 16 augustus beëindigt.

## Hooglichten

De ontwikkeling van functies verloopt snel en voortdurend. De opmerkelijke nieuwe eigenschappen omvatten:

### [!DNL Brands]

Het validatievenster van [!DNL Brand] is uitgebreid om de gebruikerservaring te verbeteren, waaronder de volgende wijzigingen:

* **op percentage-gebaseerde bevestigingsscore**: De bevestiging van het merk toont nu de score van de brandbevestiging als percentage eerder dan een pas/ontbreekt waarde.

* **bijgewerkte de extractieinterface van het Merk**: De extractie van het merk toont nu voltooiing van het extractieproces als percentage.

* **Incrementele merklading tijdens extractie**: De richtlijnen van het merk worden nu incrementeel geladen in het gebruikersinterface.

* **Vereenvoudiging van het schema van de Richtsnoer van het Exemplaar**: Het `unique attributes` en `frequent keywords` gebied zijn verwijderd uit het schema van de Richtsnoer van het Exemplaar, dat het richtsnoer op proces vereenvoudigt.

### [!DNL Create]

* **Multi-section e-mailverwezenlijking**: De gebruikers kunnen e-mails nu tot stand brengen die uit afzonderlijke titel, beeld, lichaam, en de elementen van CTA worden samengesteld.

* **Meta Adds Resize**: De scheppers kunnen Meta en aspectverhoudingen resize.

### [!DNL Insights]

* **Beperkte Inzicht login rekeningen**: Inzicht login steunt nu slechts één rekening per klant.

## Verbeteringen en opgeloste problemen

Deze release bevat de volgende aanvullende oplossingen.

### [!DNL Insights]

* De _naam van de de paginadebietplaatsing van het Detail van de Ervaring_ specificeert nu de voer van Facebook of van Instagram.

* Het snijden van grotere beelden en video is nu verenigbaar wanneer de gebruiker van de _mening van het Overzicht van Activa 0} {aan de_ mening van het Activa detail _navigeert._

* Het aantal zoekresultaten op het scherm Kenmerken wordt niet langer weergegeven `0 of` voordat een gebruiker zich aanmeldt. <!-- GS- 3665 -->

* Wanneer u op het veld **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Asset]** aantal klikt, worden de zoek- en filterinstellingen niet meer gewist. <!-- GS-3476 -->

## Bekende problemen

De volgende bekende problemen worden opgelost door de GenStudio for Performance Marketers GA-release.

### Analyse

* Acties die door de knoppen **[!UICONTROL Add templates]** en **[!UICONTROL Upload]** worden geactiveerd, worden momenteel niet bijgehouden. <!-- GS-3505 -->

### [!DNL Insights]

* De video&#39;s kunnen niet van _Assets_ worden gespeeld. <!-- GS-3846 -->

* Gebruikers moeten zich twee keer aanmelden wanneer ze zich ook bij Facebook hebben aangemeld. **Oplossing**: logout van Facebook alvorens het programma te openen [!DNL Insights].

* **uitgaven op het niveau van de Campagne** waarden zijn niet nauwkeurig. De gegevens zijn momenteel niet consistent tussen Facebook Ads Manager en het datumpigment. <!-- GS-3202 -->

### [!DNL Reviews and Approvals]

* Maker kan elementen na goedkeuring vóór publicatie wijzigen. De fiatteurs worden niet van deze wijzigingen in kennis gesteld.

