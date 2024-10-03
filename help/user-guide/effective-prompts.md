---
title: Effectieve aanwijzingen schrijven
description: Leer hoe u effectieve herinneringen voor Adobe GenStudio for Performance Marketing schrijft.
feature: Prompt, Generative AI, Brands Service, Personas Service, Products Service, Guidelines
exl-id: 0cd4db4f-d031-4c1f-a4e7-adc220f947fc
source-git-commit: c16d9f611348d0eaf3a1d4af4948196d3a06b0a1
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Effectieve aanwijzingen schrijven

Communiceren met de generatieve AI is van essentieel belang voor een effectieve werking in Adobe GenStudio for Performance Marketing.

GenStudio for Performance Marketing biedt een generatieve AI-prompt wanneer er een mogelijkheid is om een element te wijzigen. De componenten van een efficiënte herinnering zouden beschrijvende taal, voorbeelden, en informatie moeten omvatten niet die door uw gevormde richtlijnen wordt verstrekt.

Als beste praktijken, levering GenStudio for Performance Marketing van uw merkinformatie gebruikend [ richtlijnen ](/help/user-guide/guidelines/overview.md), dan kunt u volledig hefboomwerking generatieve AI om merkgerichte inhoudservaringen te produceren.

## Beschrijvende taal

U kunt natuurlijke taal gebruiken om uw ideeën uit te dragen om ervaringen te creëren. Uw vraag leidt AI om kanaalinhoud te produceren die wordt gepersonaliseerd en beelden die uw visie aanvullen. Hoe meer details u verstrekt, hoe groter de kans om een beeld of een ervaring te produceren die aan uw behoeften voldoet. Gebruik duidelijke en beschrijvende taal om zoveel mogelijk details te verschaffen:

- Voor **beelden**, gebruikswoorden die ambiance, stemming, kleur, samenstelling, en stijl beschrijven.
- Voor **exemplaar**, gebruikswoorden die het publiek, het doel, nieuwe eigenschapbeschrijvingen, voorbeelden, en acties beschrijven.

Hieronder volgt een voorbeeldprompt waarin informatie over uw intentie, doelpubliek en stijl wordt uitgelegd.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++Zie voorbeeldresultaten

![ drie geproduceerde e-mails ](/help/assets/sample-email.png)

+++

## Vrachtcriteria

In GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md), kunt u **[!UICONTROL Prompt criteria]** ([_Parameters_](/help/user-guide/create/overview.md#parameters) en een herinnering) in het snelle gebied gebruiken om details door selectie toe te voegen om de AI interpretatie te verbeteren.

Voor [ e-mails ](/help/user-guide/create/email-experiences.md), zouden de snelle criteria het toevoegen van [ richtlijnen ](/help/user-guide/guidelines/overview.md) in _Parameters_ kunnen omvatten, upload van een activa aan gebruik in de e-mailvarianten, en een beschrijvende herinnering. Voor a [ Meta en ](/help/tutorials/create-meta-ad.md), zouden de snelle criteria een merkrichtlijn in _Parameters_, selectie of upload van een bestaand activa, montages met betrekking tot beelden of activa zoals aspectverhouding, en een herinnering kunnen omvatten. De echte macht begint met [ vormende richtlijnen ](/help/user-guide/guidelines/add-guidelines.md).

>[!NOTE]
>
>Als de richtsnoeren in _Parameters_ in het snelle gebied worden toegevoegd, te hoeven u niet om verwijzing naar hen in uw herinnering te omvatten. GenStudio for Performance Marketing maakt gebruik van [!DNL Brands] , [!DNL Products] en [!DNL Personas] bij het genereren van inhoud.

### Richtsnoeren

De richtlijnen van GenStudio for Performance Marketing helpen generatieve AI om uw activa samenstelling te personaliseren. Wanneer u snelle criteria ziet, kunt u een [[!DNL Brand]](/help/user-guide/guidelines/brands.md) , een [[!DNL Persona]](/help/user-guide/guidelines/personas.md) en een [[!DNL Product]](/help/user-guide/guidelines/products.md) optie kiezen in de geconfigureerde richtlijnen.

>[!TIP]
>
>U bepaalt hoe en wanneer GenStudio for Performance Marketing de [!DNL Brand] -richtlijnen gebruikt. Zie [ Richtlijnen ](/help/user-guide/guidelines/overview.md) leren hoe te om uw merkrichtlijnen te vormen en te beheren.

### Gestructureerde vragen

Voor multi-sectiemails, kunt u herinneringen structureren om sectie-specifieke instructies te verstrekken om variërende inhoud voor elke sectie in een [ e-mail ](/help/user-guide/create/email-experiences.md) te produceren. De gestructureerde herinneringen zouden [ sectienamen in het e-mailmalplaatje ](/help/user-guide/content/email-template.md#multi-section-emails) direct van verwijzingen moeten voorzien zodat de geproduceerde inhoud in de overeenkomstige inhoudsplaatsaanduidingen kan worden opgenomen.

U kunt GenStudio for Performance Marketing bijvoorbeeld de instructie geven om in de eerste sectie van een e-mailbericht inhoud te genereren waarmee een nieuw product wordt bevorderd en om inhoud te genereren waarin de kostenbesparende voordelen van het product in de tweede e-mailsectie worden beschreven.

De gestructureerde herinnering moet:

- Gebruik een van de volgende verwijzingen naar de sectienaam in het e-mailmalplaatje:
   - Pod
   - Groep
   - Sectie
   - Module

  Als uw sjabloon bijvoorbeeld `moduleA` of `Group-3` als sectienaam gebruikt, kunt u naar die sectienamen verwijzen in de vraag.

- Volg de aanbevolen regels/structuur. Als de snelle structuur niet aan het verstrekte formaat aanhoudt, is de herinnering op *alle* e-mailsecties van toepassing en vergemakkelijkt nog inhoudsgeneratie.
- De sectienamen van het gebruik zoals [ die in uw e-mailmalplaatje ](/help/user-guide/content/email-template.md#code-an-email-template) worden bepaald. Vragen moeten overeenkomen met de sectienamen die in uw e-mailsjabloon zijn gecodeerd.
- Wees niet hoofdlettergevoelig. U kunt bijvoorbeeld `Pod` of `pod` gebruiken in uw e-mailsjabloon en gestructureerde prompt.
- Verwijs eerst de generische gebruikersherinnering, en toen de sectie-specifieke richtlijnen.
- Gebruik een dubbele punt, afbreekstreepje, komma of andere afbakening (`,:;#$!~|@=-%&*^_`) als scheiding tussen de verwijzing van de sectienaam en de richtlijn. U kunt bijvoorbeeld het volgende gebruiken als een sectiespecifieke prompt instructie: `Pod1; Describe how to easily edit text and swap images.`

Hieronder volgt een voorbeeldprompt waarin de aanbevolen snelle structuur wordt uitgelegd en een e-mailsjabloon wordt gebruikt waarin de identificerende term `Pod` wordt gebruikt, zoals in `Pod1` , `Pod2` en `Pod3` .

```properties
Create an exciting multi-pod email focusing on Creative Cloud and its powerful generative AI capabilities.

Encourage customers to convert to Photoshop or use a free Photoshop trial. We want to better educate them about app features.

Pod1: Focus on Adobe Photoshop and its new generative AI tools that enable creators to bring images to life in minutes.

Pod2: Focus on Adobe Illustrator and its new generative AI tools, such as Generative Shape Fill, which allows you to quickly fill your vector outline and explore a variety of options that match the look and feel of your own artwork.

Pod3: Focus on Adobe Acrobat Pro. Make users aware that with Acrobat Pro they can edit images and text inside a PDF.
```

Zie [ een e-mailmalplaatje ](/help/user-guide/content/email-template.md#code-an-email-template) voorbereiden.

## Opnieuw proberen

Vragen is een herhalend proces. Als de resultaten niet aan uw verwachtingen voldoen, herzie uw herinnering en breng sommige veranderingen aan of voeg meer details toe. Of u kunt in secties plakken uit een campagneremap. U kunt GenStudio for Performance Marketing zelfs vragen bepaalde woorden, elementen of thema&#39;s te vermijden.

## Aanbevolen procedures

Sommige eenvoudige beste praktijken voor het ontwerpen van efficiënte herinneringen:

- Wees specifiek en geef details over wat je moet doen en niet.
- Zorg voor context met externe referenties.
- Gebruik GenStudio for Performance Marketing-richtlijnen.
- Richtlijnen regelmatig controleren en aanpassen.
- Herhalen en verfijnen.
- Leer door te experimenteren.
