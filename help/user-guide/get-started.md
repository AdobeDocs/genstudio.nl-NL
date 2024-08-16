---
title: Aan de slag met Adobe GenStudio voor prestatiemarkeringen
description: Leer hoe u GenStudio for Performance Marketers instelt om nieuwe marketinginhoud te genereren die is afgestemd op het merk.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: c9d09801f0bd3732611b01d4a98cc7ebf38884d7
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 0%

---


# Aan de slag met Adobe GenStudio voor prestatiemarkeringen

GenStudio for Performance Marketers is een uitgebreid platform voor het maken, evalueren en beheren van marketingervaringen die uw merkidentiteit weerspiegelen en respecteren.

De toegang van belanghebbenden tot zijn vele mogelijkheden wordt gecontroleerd door toegewezen gebruikersrollen. Uw toegewezen gebruikersrol bepaalt de taken die u kunt uitvoeren binnen GenStudio for Performance Marketers. Een beheerder stelt uw machtigingen in. Deze worden gedefinieerd in uw welkomstbericht.

Als u aan generatieve op AI-Gebaseerde hulpmiddelen nieuw bent of eenvoudig nieuwsgierig over GenStudio voor de kernbeginselen van de Marketers van Prestaties zie [ Concepten ](concepts.md) en [ schrijven efficiënte herinneringen ](effective-prompts.md).

## Gebruikersrollen

Voor het maken en implementeren van moderne marketingcampagnes is samenwerking tussen belanghebbenden met verschillende verantwoordelijkheden en vaardigheden vereist.

Drie soorten GenStudio for Performance Marketers-gebruikersrollen ondersteunen deze verscheidenheid aan organisatorische rollen. De toestemmingen worden aangepast aan elk van deze gebruikerstypes en steunen de verantwoordelijkheden van elke gebruiker in de marketing organisatie.

**de drie types van gebruikersrol zijn**:

* **gebruik GenStudio for Performance Marketers generatieve AI mogelijkheden van de scheppers** om marketing campagneactiva tot stand te brengen, om inhoudsoverzicht en goedkeuring te verzoeken, en goedgekeurde ontwerpen van deze inhoud te publiceren. Alle gebruikers GensStudio kunnen tot activa toegang hebben en gebruiken zodra zijn schepper het aan Inhoud heeft bewaard.

* **Medewerkers** zijn de breedste waaier van GenStudio voor de gebruikers van de Marketers van Prestaties. Medewerkers kunnen inhoud weergeven en goedkeuren en vormen een essentieel onderdeel van de workflow dat ervoor zorgt dat de inhoud die u genereert, aansluit bij de behoeften en standaarden van uw organisatie.

* **de beheerders van het Systeem** hebben de breedste reeks toestemmingen binnen GenStudio voor de Marketers van Prestaties. Systeembeheerders kunnen gebruikers en inhoud toevoegen en verwijderen. Beheerders vervullen de essentiële instapkaarttaak, namelijk het vaststellen van de basisinstructies voor het creëren en implementeren van campagnemiddelen. Admins voeren deze gidsen uit door merk en organisatie-specifieke informatie zoals [ merkrichtlijnen ](/help/user-guide/guidelines/overview.md) te uploaden.

>[!NOTE]
>Alvorens om het even welke gebruikers provisioned in deze rollen zijn, moet een beheerder als superuser in de console van Admin van de Adobe worden aangewezen om éénmalige opstellingstaken uit te voeren. Deze supergebruikersrol werkt alleen in de context van de Adobe Admin Console. Het speelt geen rol in de GenStudio for Performance Marketers platforminterface. Er is geen concept van superuser in GenStudio for Performance Marketers roltoewijzingen.

### Maker

**de Makers** hebben de kerntoestemmingen nodig om GenStudio voor de Marketers van Prestaties [!DNL Brands], [!DNL Campaigns], en [!DNL Content] activa tot stand te brengen. Ze kunnen ook elementen die ze hebben gemaakt bewerken en verwijderen. GenStudio for Performance Marketers ondersteunt het snel maken van honderden stukken inhoud. Deze gebruikers kunnen inhoudsfragmenten of hele ervaringen genereren die afzonderlijke goedgekeurde inhoud ordenen om aan de behoeften van specifieke marketingcampagnes te voldoen.

De scheppers werken met GenStudio voor de generatieve AI technologieën van de Marketers van Prestaties door _het veroorzaken_ in wisselwerking. Het snelle gebied op het canvas verstrekt hulpmiddelen om herinneringen in de context van een specifieke campagnerichtlijnen te plaatsen. Als gevolg hiervan is de kwaliteit en het succes van gegenereerde inhoud gedeeltelijk afhankelijk van de kwaliteit van de merkrichtlijnen die uw organisatie heeft geüpload en de specificiteit van uw vraag.

Zie [ efficiënte herinneringen ](effective-prompts.md) schrijven.

In de volgende tabel worden de standaardmachtigingen voor de maker weergegeven:

| Functie | Maken | Bijwerken | Verwijderen | Weergave |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | nee | nee | nee | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Insights] | kan slechts en schakelaars vormen |    |     | ja |
| [!DNL Personas] | ja | ja | ja | ja |
| [!DNL Products] | ja | ja | ja | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |

### Medewerkers

**de Medewerkers** kunnen activa in GenStudio voor de Marketers van Prestaties bekijken maar creëren, uitgeven of schrappen niet deze activa. Deelnemers zijn belanghebbenden die van essentieel belang zijn voor het welslagen van het beoordelings- en goedkeuringsproces voor inhoud, maar die geen inhoud hoeven te maken of rechtstreeks hoeven te bewerken. Juridische experts en managers van ontwerpers zijn voorbeelden van potentiële medewerkers. Medewerkers van GenStudio for Performance Marketers hebben mogelijk machtigingen om middelen in andere producten van de Creative Cloud te maken en weer te geven.

In de volgende tabel worden de standaardmachtigingen voor medewerkers weergegeven:

| Functie | Maken | Bijwerken | Verwijderen | Weergave |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | ja | ja | ja | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Insights] | nee | nee | nee | ja |
| [!DNL Personas] | ja | ja | ja | ja |
| [!DNL Products] | ja | ja | ja | ja |
| [!DNL Reviews and approvals] | nee | nee | nee | ja |

### Beheerders

**de Beheerders** creëren en wijzen gebruikers aan om het even welke GenStudio voor de Marktdeelnemers van Prestaties toe steunden rollen. Zij kunnen nieuwe toestemmingen aan individuele creators of medewerkers toewijzen zoals vereist. Hun belangrijkste taak is het uitvoeren van de eerste instaptaken die uw organisatie voorbereiden op de implementatie van GenStudio for Performance Marketers.

In de volgende tabel worden de standaardmachtigingen van de systeembeheerder weergegeven:

| Functie | Maken | Bijwerken | Verwijderen | Weergave |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | ja | ja | ja | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Insights] | ja | ja | ja | ja |
| [!DNL Personas] | ja | ja | ja | ja |
| [!DNL Products] | ja | ja | ja | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |


## GenStudio for Performance Marketers voorbereiden om inhoud te genereren

Systeembeheerders bereiden de GenStudio for Performance Marketers-omgeving van hun organisatie voor zodat ontwerpers en medewerkers campagnemiddelen kunnen maken. Deze voorbereidende taken omvatten:

1. [ voegt richtlijnen ](./guidelines/overview.md) voor [!DNL Brands], [!DNL Products], en [!DNL Personas] toe. Het opzetten van de belangrijkste bouwstenen van de merkidentiteit van uw organisatie is een essentiële voorwaarde voor het werk van ontwerpers en medewerkers. U kunt documenten met brandrichtlijnen uploaden of handmatig merkgegevens invoeren.
   * **bereidt uw documenten van richtlijnen** voor. Hoe beschrijvender en uitgebreider uw merkrichtlijnen, hoe beter de uitvoer. Voeg korte voorbeelden toe van functies die u belangrijk vindt voor uw merk en voeg beschrijvingen toe van het gedrag dat u wilt uitsluiten van het maken van inhoud. GenStudio for Performance Marketers extraheert informatie uit deze geüploade documenten en begint uw merk te maken. Informatie zoals stem van het merk, kanaal, en beeldrichtlijnen, zijn bevolkt aangezien GenStudio for Performance Marketers elke richtlijn van uw geüploade documenten samenstelt.
   * **geef of volledige gebieden van de merkrichtlijn uit zoals nodig**. Uitgebreide merkrichtlijnen vormen de basis voor het inzicht van GenStudio for Performance Marketers in het merk van uw organisatie. Zodra GenStudio for Performance Marketers de benodigde informatie uit de documenten met uw merkenrichtlijnen heeft gehaald, wordt u gevraagd om velden met geëxtraheerde informatie handmatig te bewerken of in te vullen. Afzonderlijke productfocusgebieden voor het maken van inhoud opgeven door een [!DNL Product] toe te voegen. Met de richtlijnen van [!DNL Personas] kunt u de creatie van inhoud voor bepaalde klantsegmenten afstemmen.

   Hoewel het opzetten van de merkrichtlijnen van een organisatie een eenmalige actie kan zijn, zou u deze richtlijnen kunnen moeten herzien en verbeteren die op de volatiliteit, de groei, en veranderende marktomstandigheden van uw organisatie worden gebaseerd.

1. **[uploadt malplaatjes](./content/use-templates.md)**. Sjablonen bieden sneltoetsen en versnellen het maken van inhoud. Een sjabloon bevat goedgekeurde functies, zoals kop- en voetteksten, en stelt hulplijnen voor het maken van inhoud in. Beheerders uploaden en beheren doorgaans sjablonen voor hun organisatie. Maker gebruikt malplaatjes om het proces van de inhoudsverwezenlijking binnen de vastgestelde grenzen van organisatiemerk te springen.

1. **[uploadt goedgekeurde activa](./content/manage-assets.md)**. Goedgekeurde middelen in [!DNL Content] zijn beschikbaar voor alle makers van GenStudio for Performance Marketers. U kunt [!DNL Content] samenvoegen met elementen die ontwerpers kunnen gebruiken om nieuwe ervaringen of elementen te maken.

1. **[verbind met een rekening van Meta (Facebook)](./insights/connect-channel.md)**. U moet een verbinding tussen GenStudio for Performance Marketers en de sociale accounts van uw organisatie configureren om gegevens te ontvangen van uw actieve marketingcampagnes, middelen en ervaringen. [[!DNL Insights]](./insights/overview.md) biedt hulpprogramma&#39;s voor het analyseren van gegevens die zijn afgeleid van kanalen.
