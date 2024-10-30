---
title: "Verbind met een  [!DNL AEM Assets Content Hub]  bewaarplaats"
description: Leer hoe te om Adobe GenStudio for Performance Marketing met een Adobe Experience Manager (AEM) te verbinden  [!DNL Content Hub]  bewaarplaats en hefboomwerking bestaande goedgekeurde inhoud.
level: Experienced
feature: Assets, Content
source-git-commit: bd3c5c9ff12c962d4123ac992fb74cd94e184172
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Verbinding maken met een [!DNL AEM Assets Content Hub] -opslagplaats

Als u middelen hebt in Adobe Experience Manager (AEM), kunt u deze stappen volgen om ze toegankelijk te maken in GenStudio for Performance Marketing.

>[!BEGINSHADEBOX]

**Eerste vereisten**:

De volgende stappen vereisen administratieve toegang tot Admin Console en AEM Assets as a Cloud Service.

>[!ENDSHADEBOX]

## Stap 1: Inschakelen [!DNL AEM Assets Content Hub]

Volg **stel Content Hub** zelfbedieningsproces op om [!DNL Content Hub] voor uw bestaande AEM Assets in Cloud Manager toe te laten. Zie [ opstellen  [!DNL Content Hub] ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub) in de _AEM as a Cloud Service_ documentatie.

Nadat u [!DNL AEM Assets Content Hub] hebt ingeschakeld, hebt u een nieuwe instantie met het `contenthub` achtervoegsel [!DNL AEM Assets as a Cloud Service] op de Admin Console.

## Stap 2: GenStudio-gebruikers aan boord

Voeg in [!DNL Admin Console] GenStudio-gebruikers of -gebruikersgroepen toe aan de productprofielen van [!DNL AEM Assets Content Hub] . [!DNL AEM Assets Content Hub] -gebruikers kunnen elementen weergeven, maar kunnen geen elementen toevoegen of bestaande elementen wijzigen.

- [ Onboard  [!DNL Content Hub]  beheerder ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [ Onboard  [!DNL Content Hub]  gebruikers ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## Stap 3: activa goedkeuren

Goedkeuren van elementen voor gebruik in [!DNL AEM Assets Content Hub] , zodat deze beschikbaar zijn in GenStudio for Performance Marketing. Zie [ activa in Experience Manager ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets) in de _AEM as a Cloud Service_ documentatie goedkeuren.

## Stap 4: Zichtbaarheid van middelen configureren

Controleer in de configuratieopties van _[!DNL AEM Assets Content Hub]_elke set configuratieopties voor filters, elementdetails, zoeken en brandmerken. Zie [ Content Hub gebruikersinterface ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options) in de_ AEM as a Cloud Service _documentatie vormen.

## Stap 5: Controleer de verbinding

In GenStudio for Performance Marketing Content is de lijst _[!UICONTROL Location]_beschikbaar boven de galerie aan de rechterkant. De lijst is niet beschikbaar als u geen toegang hebt of als uw organisatie een [!DNL AEM Assets Content Hub] -opslagplaats niet heeft geïmplementeerd en aangesloten.
