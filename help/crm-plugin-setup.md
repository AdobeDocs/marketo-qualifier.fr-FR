---
title: Configuration du plug-in CRM
description: Découvrez comment installer le plug-in Marketo Qualifier CRM dans Salesforce ou Microsoft Dynamics 365. Configurez les actions Salesforce pour les workflows et les campagnes Marketo.
feature: Agentic AI, Sales Insights, Account Journeys
role: Admin
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Marketo Qualifier
feature_v2:
  - id: da701e37-3227-4187-b68a-914277252a79
    internal-label: Integrations
  - id: f8f8b877-7295-5853-989f-e21f73bc94c4
    internal-label: Administration
subfeature_v2:
  - id: d2fe5f36-5653-5902-937c-9d3026104284
    internal-label: CRM integrations
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: df256cf271296b82fab2ed10725a0d6bd165e05b
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%
---

# Configuration du plug-in CRM

Installez le plug-in CRM [!DNL Adobe Marketo Qualifier] afin que les représentants puissent utiliser [!DNL Marketo Sales Insights] et les informations générées par l’IA sur les pages d’enregistrement de lead, contact et compte sans quitter Salesforce ou Microsoft Dynamics 365. Le plug-in fournit également une vue d’accueil pour [hiérarchiser les prospects dans votre CRM](admin-settings.md#prioritize-leads-in-the-crm-plugin).

Dans Salesforce, les représentants peuvent également ajouter des prospects aux workflows sortants ou aux campagnes Marketo à partir des vues Liste de prospects et de contacts et des pages d’enregistrement individuelles.

## Avant de commencer

Assurez-vous que les personnes qui installent et utilisent le plug-in disposent de l’accès requis :

* **Administrateur Salesforce** : autorisation d’installer des packages et de modifier les mises en page.
* **Administrateur Microsoft Dynamics 365** : autorisation d’importer des solutions dans l’environnement cible dans Power Apps.
* **Représentants** : accès à Marketo Qualifier et aux enregistrements CRM pertinents.

L’installation du plug-in est distincte de la [connexion de votre CRM à Marketo Qualifier](getting-started.md#connect-your-crm).

## Installation dans Salesforce

Installez le package, puis ajoutez ses composants aux pages d’enregistrement que les représentants utilisent.

1. Ouvrez la page d’installation de [Salesforce](https://experience.adobe.com/solutions/OneAdobe-sales-workflow-optimizer-sales-insight-ui/install/sales-insight?crm=salesforce) et connectez-vous à Salesforce en tant qu’administrateur.
1. Sur la page d’installation du package, sélectionnez **[!UICONTROL Installer pour tous les utilisateurs]**, puis **[!UICONTROL Installer]**.

   Vous pouvez toujours contrôler l’accès des utilisateurs individuels via les autorisations Salesforce.

1. Lorsque vous êtes invité à approuver l&#39;accès tiers, cochez la case d&#39;approbation et sélectionnez **[!UICONTROL Continuer]**.
1. Une fois l’installation terminée, sélectionnez **[!UICONTROL Terminé]**.

   L’installation prend quelques minutes. Vérifiez que le package apparaît sur la page **[!UICONTROL Packages installés]**.

1. Dans Lightning App Builder, modifiez les pages d’enregistrement Lead, Contact et Compte et ajoutez les composants Marketo Qualifier.

### Ajout d’actions aux vues de liste

Configurez **[!UICONTROL Ajouter au workflow sortant]** et **[!UICONTROL Ajouter à Marketo Campaign]** séparément pour les vues Liste de leads et Liste de contacts. Utilisez les boutons inclus dans le package pour éviter les doublons.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Gestionnaire d’objets]** et sélectionnez **[!UICONTROL Lead]** ou **[!UICONTROL Contact]**.
1. Ouvrez **[!UICONTROL Boutons, liens et actions]** et recherchez les boutons de liste **[!UICONTROL Ajout AMQ au workflow sortant]** et **[!UICONTROL Ajout AMQ à Marketo Campaign]**.
1. Ouvrez la **[!UICONTROL disposition des boutons de la vue Liste]** de l’objet et sélectionnez **[!UICONTROL Modifier]**.

   Selon la configuration de Salesforce, la disposition de la vue Liste peut se trouver sous **[!UICONTROL Dispositions de recherche]** > **[!UICONTROL Vue Liste]**.

1. Déplacez les deux boutons de liste vers **[!UICONTROL Boutons sélectionnés]** et enregistrez.
1. Répétez l’opération pour l’autre objet.

Les représentants sélectionnent un ou plusieurs enregistrements dans une vue Liste, puis sélectionnent l’action.

### Ajouter des actions pour enregistrer des pages

Les actions de page d’enregistrement doivent être configurées séparément des boutons de vue de liste. Ajoutez les deux actions à chaque mise en page de lead et de contact utilisée.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Gestionnaire d’objets]** et sélectionnez **[!UICONTROL Lead]** ou **[!UICONTROL Contact]**.
1. Ouvrez **[!UICONTROL Boutons, liens et actions]** et recherchez les boutons de détail **[!UICONTROL Ajout AMQ au workflow sortant]** et **[!UICONTROL Ajout AMQ à la campagne Marketo]**.
1. Ouvrez **[!UICONTROL Mises en page]** et modifiez une mise en page affectée à vos représentants.
1. Ajoutez les deux boutons de détails aux **[!UICONTROL actions Salesforce Mobile et Lightning Experience]** et enregistrez.
1. Répétez l’opération pour chaque mise en page applicable et pour l’autre objet.

Les actions s&#39;affichent dans la barre d&#39;actions de l&#39;enregistrement ou dans son menu et s&#39;appliquent à l&#39;enregistrement affiché.

>[!NOTE]
>
>Ces actions fonctionnent dans Salesforce Lightning Experience de bureau, et non dans l’application mobile Salesforce. La section de disposition nommée **[!UICONTROL Salesforce Mobile et actions d’expérience Lightning]** est également utilisée pour les actions de bureau.

### Remplacer un bouton manquant

Si un bouton empaqueté est manquant, créez un remplacement sous les **[!UICONTROL Boutons, liens et actions]** de l’objet.

1. Sélectionnez **[!UICONTROL Nouveau bouton ou lien]**.
1. Saisissez un libellé pour l’action, tel que `Add to Outbound Workflow` ou `Add to Marketo Campaign`.
1. Choisissez **[!UICONTROL Bouton de liste]** pour une vue de liste ou **[!UICONTROL Bouton de page de détail]** pour une page d’enregistrement.
1. Définissez **[!UICONTROL Source de contenu]** sur **[!UICONTROL Page Visualforce]** et sélectionnez la page d’action du package correspondant à l’action, à l’objet et à l’emplacement.

   La liste de leads, les détails de leads, la liste de contacts et les emplacements de détails de contacts utilisent différentes pages. Vérifiez que la page sélectionnée correspond à l’emplacement que vous êtes en train de configurer.

1. Pour un bouton de liste, sélectionnez **[!UICONTROL Exiger une sélection de ligne]**.
1. Enregistrez le bouton et ajoutez-le à la disposition de bouton de vue de liste appropriée ou aux actions de page d’enregistrement, comme décrit ci-dessus.

### Vérifier les actions Salesforce

Après avoir enregistré les mises en page, vérifiez que les deux actions apparaissent dans les vues Liste de prospects et de contacts et dans les pages d’enregistrement. Tester chaque action de liste avec les enregistrements sélectionnés et chaque action de page d&#39;enregistrement à partir d&#39;un enregistrement individuel.

Si une action n’est pas disponible ou ne s’ouvre pas, procédez comme suit :

| Problème | Éléments à vérifier |
| --- | --- |
| Bouton manquant dans la vue Liste | Vérifiez que le bouton de liste se trouve dans **[!UICONTROL Boutons sélectionnés]** dans la **[!UICONTROL disposition de bouton de vue Liste]** de l’objet approprié, puis enregistrez la disposition. |
| Bouton manquant dans une page d’enregistrement | Vérifiez que le bouton de détail se trouve dans les **[!UICONTROL actions d’expérience Salesforce Mobile et Lightning]** dans la disposition affectée à l’utilisateur. Si votre organisation utilise des actions dynamiques, vérifiez également la visibilité des actions de la page d’enregistrement. |
| Option de page attendue non disponible lors de la création d’un bouton | Vérifiez que le type d’affichage est **[!UICONTROL Bouton de liste]** pour une vue de liste ou **[!UICONTROL Bouton de page de détail]** pour une page d’enregistrement. |
| L’action ne s’ouvre pas ou affiche une erreur d’accès. | Vérifiez que l&#39;utilisateur a accès à Marketo Qualifier et aux enregistrements sélectionnés. |

## Installation dans Microsoft Dynamics 365

Importez le package de module externe dans l’environnement de travail de vos représentants.

1. Ouvrez la page d’installation de [Microsoft Dynamics 365](https://experience.adobe.com/solutions/OneAdobe-sales-workflow-optimizer-sales-insight-ui/install/sales-insight?crm=dynamics) et téléchargez le fichier ZIP du package.
1. Connectez-vous à [Power Apps](https://make.powerapps.com/) en tant qu’administrateur et sélectionnez l’environnement cible.
1. Ouvrez **[!UICONTROL Solutions]** et sélectionnez **[!UICONTROL Importer la solution]**.
1. Sélectionnez **[!UICONTROL Parcourir]**, choisissez le fichier ZIP téléchargé, puis sélectionnez **[!UICONTROL Suivant]**.
1. Vérifiez les détails du package et sélectionnez **[!UICONTROL Suivant]**.
1. Conservez la valeur de la variable d’environnement préremplie et sélectionnez **[!UICONTROL Importer]**.
1. Attendez le message de confirmation en haut de la page indiquant que la solution a bien été importée.

L’importation prend quelques minutes.

>[!MORELIKETHIS]
>
>* [Hiérarchiser les prospects dans le plug-in CRM](admin-settings.md#prioritize-leads-in-the-crm-plugin)
>* [Intégrations](integrations.md)
>* [Commencer](getting-started.md)
