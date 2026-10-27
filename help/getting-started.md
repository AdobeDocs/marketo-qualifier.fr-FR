---
title: Prise en main de Adobe Marketo Qualifier
description: Découvrez comment effectuer la configuration d’administrateur unique pour Adobe Marketo Qualifier, y compris les groupes d’utilisateurs et une connexion CRM, avant que votre équipe ne commence à utiliser l’application.
feature: Agentic AI, Sales Insights, Account Journeys
role: Admin
TQID: 'https://experienceleague.adobe.com/-nfmFwZyZFUZhm-uQUjSyTvrORuqJgKSKnENWYtvubs'
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Marketo Qualifier
feature_v2:
  - id: da701e37-3227-4187-b68a-914277252a79
    internal-label: Integrations
  - id: f8f8b877-7295-5853-989f-e21f73bc94c4
    internal-label: Administration
subfeature_v2:
  - id: 74576239-3a5e-5e17-9c2d-f86db4fbb490
    internal-label: User management
  - id: d2fe5f36-5653-5902-937c-9d3026104284
    internal-label: CRM integrations
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: fcdc5d36cbb1500cf984e1439291aa8dbf17b72b
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 0%
---

# Prise en main de Adobe Marketo Qualifier

Une fois qu’Adobe a configuré Marketo Qualifier pour votre organisation, un administrateur système [!DNL Marketo] doit créer les groupes d’utilisateurs requis et connecter Salesforce ou Microsoft Dynamics 365.

![Page d&#39;accueil de ](assets/homepage.png){width="800" zoomable="yes"}

## Configurer des groupes d’utilisateurs

Dans Adobe Admin Console, les groupes d’utilisateurs sont utilisés pour contrôler l’accès à Marketo Qualifier. Les deux groupes doivent être créés avant que les utilisateurs puissent se connecter.

Consultez la [documentation de ](https://helpx.adobe.com/business/enterprise/users/users-and-groups/user-groups.html) pour plus d’informations sur la configuration des groupes.

>[!PREREQUISITES]
>
>L’administrateur ou l’administratrice qui crée les groupes doit répondre à ces deux exigences :
>
>* Être un administrateur d’organisation ayant accès à **** à partir du sélecteur d’applications Adobe.
>* être affecté au produit Adobe Experience Platform ou être administrateur système. Dans le cas contraire, Adobe Experience Platform n’apparaît pas dans la liste des produits.

### Utilisateurs de Marketo Qualifier

Les utilisateurs doivent appartenir au groupe d’utilisateurs `Marketo Qualifier` pour accéder à l’application.

Ces étapes sont effectuées dans le Adobe Admin Console.

1. Dans le sélecteur d’applications, sélectionnez ****.
1. Sélectionnez **[!UICONTROL Utilisateurs]** > **[!UICONTROL Groupes d’utilisateurs]** > **[!UICONTROL Nouveau groupe d’utilisateurs]**.
1. Saisissez `Marketo Qualifier` pour le nom du groupe et sélectionnez **[!UICONTROL Enregistrer]**.
1. Ouvrez **[!UICONTROL Profils de produit attribués]** et sélectionnez **[!UICONTROL Attribuer le profil]**.
1. Sélectionnez ****.
1. Sélectionnez le profil de produit **[!UICONTROL Accès à tous les produits de production par défaut]**, sélectionnez **[!UICONTROL Appliquer]**, puis sélectionnez **[!UICONTROL Enregistrer]**.
1. Pour ajouter tous ceux qui ont besoin d’accéder à Marketo Qualifier, ouvrez **[!UICONTROL Utilisateurs]** et sélectionnez **[!UICONTROL Ajouter des utilisateurs]**.

### Administrateurs Marketo Qualifier

Les administrateurs qui configurent les connexions CRM, le [Centre de connaissances](admin-settings.md#knowledge-center) et les paramètres de désinscription globale aux e-mails doivent également appartenir au groupe d’utilisateurs `Marketo Qualifier Admins`.

1. Dans Adobe Admin Console, sélectionnez **[!UICONTROL Utilisateurs]** > **[!UICONTROL Groupes d’utilisateurs]** > **[!UICONTROL Nouveau groupe d’utilisateurs]**.
1. Saisissez `Marketo Qualifier Admins` pour le nom du groupe et sélectionnez **[!UICONTROL Enregistrer]**.
1. Ouvrez **[!UICONTROL Utilisateurs]**, sélectionnez **[!UICONTROL Ajouter des utilisateurs]** et ajoutez les administrateurs.
1. Vérifiez que chaque administrateur est également membre du groupe `Marketo Qualifier`.

L’appartenance aux deux groupes rend **[!UICONTROL Paramètres d’administration]** visible sous **[!UICONTROL Administration]** dans le volet de navigation de gauche. Les utilisateurs standard utilisent les champs, les filtres et le playbook configurés par l’administration. Le pied de page d’opt-out configuré s’applique automatiquement à leurs e-mails sortants. Les utilisateurs standard ne peuvent pas modifier ces paramètres.

Les noms des groupes d’utilisateurs doivent correspondre exactement comme indiqué dans les étapes précédentes.

Vous pouvez également créer un groupe de `Marketo Qualifier BDR managers` facultatif. Les membres de ce groupe peuvent accéder aux rapports de performances des e-mails.

## Connexion à votre CRM

Marketo Qualifier se connecte à Salesforce ou à Microsoft Dynamics 365 pour offrir aux rapports sur l’ensemble des appareils une vue unifiée des utilisateurs, des prospects, des contacts, des comptes, des opportunités, des mappages des propriétaires et des activités associées. La connexion initiale nécessite un accès en lecture seule à ces données CRM. Pour préparer les informations d’identification avant de connecter Marketo Qualifier, contactez votre administrateur CRM. Voir [ Intégrations ](integrations.md) pour plus d’informations sur l’intégration.

>[!PREREQUISITES]
>
>Pour accéder à l&#39;interface d&#39;administration du CRM, vous devez appartenir aux groupes `Marketo Qualifier Admins` Adobe Admin Console et `Marketo Qualifier` .

>[!BEGINTABS]

>[!TAB Salesforce]

Un administrateur système Salesforce crée une application cliente externe (également appelée application connectée) et configure son utilisateur d’exécution.

>[!PREREQUISITES]
>
>Vérifiez que l’administrateur Salesforce dispose des autorisations suivantes :
>
>* Personnaliser l’application
>* Afficher l’installation et la configuration
>* Modifier toutes les données
>* Gérer les applications connectées
>
>L’administrateur a besoin de l’option _Gérer les applications connectées_ pour afficher l’identifiant client et le secret client.

1. Dans Salesforce, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL App Manager]** et sélectionnez **[!UICONTROL Nouvelle application connectée]** ou **[!UICONTROL Nouvelle application cliente externe]**.
1. Saisissez un nom d’application et une adresse e-mail de contact administratif.
1. Activez OAuth et saisissez une URL de rappel.

   Si la connexion n’utilise pas de redirection, saisissez une URL valide.

1. Ajoutez les portées OAuth suivantes :

   * Accéder au service d’URL d’identité (`id`, `profile`, `email`, `address`, `phone`)
   * Gestion des données utilisateur par le biais des API (`api`)
   * Accéder aux identifiants d’utilisateur uniques (`openid`)

1. Activez le flux d’informations d’identification du client et sélectionnez un utilisateur **[!UICONTROL Exécuter en tant que]**.
1. Vérifiez que l’utilisateur exécutant dispose d’un accès en **lecture** à `Leads`, `Accounts`, `Contacts`, `Tasks`, `Events`, `Opportunity`, `OpportunityContactRoles` et `OpportunityLineItems`. Vérifiez également que l’option **Accéder aux activités** est activée.
1. Enregistrez l’application.
1. Dans **[!UICONTROL App Manager]**, ouvrez l’application et sélectionnez **[!UICONTROL Afficher]** > **[!UICONTROL Détails du client]**.
1. Copiez les valeurs suivantes pour la connexion Marketo Qualifier :

   * Consumer Key (ID client)
   * Secret du client
   * URL de rappel
   * URL de l’instance Salesforce

Les étapes sont légèrement différentes de celles décrites ici. Pour plus d&#39;informations, consultez la documentation de [](https://help.salesforce.com/s/?language=en_US).

### Recherche de l’URL de votre instance Salesforce

1. Connectez-vous et notez votre organisation _Mon domaine_ sous-domaine dans la barre d’adresse du navigateur (valeur `{{mydomain}}`).
1. Utilisez le formulaire canonique pour Marketo Qualifier : `https://{{mydomain}}.my.salesforce.com`.

N’utilisez pas d’URL `lightning.force.com` comme URL d’instance.

>[!TIP]
>
>Si l’interface de connexions CRM signale des portées manquantes, vérifiez le profil de l’utilisateur exécutant en tant que sous **[!UICONTROL Autorisations d’objet standard]** pour obtenir un accès **Lecture** aux prospects, contacts, comptes et opportunités. Vérifiez également **[!UICONTROL Paramètres de l’objet]** dans chaque jeu d’autorisations affecté.

>[!TAB Microsoft Dynamics 365]

Un administrateur Microsoft Dynamics 365 ou Azure enregistre une application et l’ajoute à l’environnement Dynamics.

1. Dans Microsoft Entra ID, sélectionnez **[!UICONTROL Enregistrements des applications]** et enregistrez une application.
1. Copiez l’ID client et l’ID client, puis créez un secret client.
1. Dans le **[!UICONTROL Centre d’administration Power Platform]**, sélectionnez **[!UICONTROL Environnements]** et ouvrez l’environnement Dynamics.
1. Accédez à **[!UICONTROL Paramètres]** > **[!UICONTROL Utilisateurs + autorisations]** > **[!UICONTROL Utilisateurs de l’application]** et sélectionnez **[!UICONTROL Nouvel utilisateur de l’application]**.
1. Sélectionnez l’application Microsoft Entra enregistrée.
1. Attribuez un rôle de sécurité qui accorde un accès en lecture aux prospects, contacts, comptes, opportunités et activités.

   Un rôle de sécurité est requis. Un rôle de sécurité est requis pour que l&#39;application puisse accéder aux données Dynamics.

1. Collectez l’ID client, le secret client, l’ID client et l’URL de l’instance Dynamics. Utilisez l’`https://{{mydomain}}.crm.dynamics.com` de formulaire d’URL canonique.

>[!ENDTABS]

### Entrez votre connexion

1. En tant que membre des deux groupes Marketo Qualifier requis, connectez-vous à Marketo Qualifier et vérifiez que le sandbox ou l’environnement approprié est sélectionné.
1. Dans le volet de navigation de gauche, développez **[!UICONTROL Administration]** et sélectionnez **[!UICONTROL Paramètres d’administration]**.
1. Sélectionnez **[!UICONTROL Connexions CRM]** sous **[!UICONTROL Intégrations]**.

   La page affiche des cartes pour Salesforce et Microsoft Dynamics. Une connexion inactive affiche **[!UICONTROL Connect]**. Une connexion configurée affiche **[!UICONTROL Connecté]** et **[!UICONTROL Gérer]**.

   ![Informations d’identification ](assets/crm-salesforce-config.png){width="800" zoomable="yes"}

1. Sélectionnez **[!UICONTROL Connexion]** pour le CRM que vous utilisez.
1. Saisissez les informations d’identification et l’URL de l’instance à partir de votre administrateur CRM.
1. Une fois la connexion établie, vérifiez que la carte indique **[!UICONTROL Connecté]**.

### Importer les champs du CRM

Après la connexion au CRM, configurez le mapping entrant pour déterminer quels champs du CRM apparaissent dans Marketo Qualifier. Pour ouvrir **[!UICONTROL Mapping entrant]**, sélectionnez **[!UICONTROL Gérer]** sur la carte CRM connectée, puis ajoutez une section pour chaque type d’entité dont vous souhaitez importer les champs.

Consultez la section [Mappage des champs CRM (mappage entrant)](integrations.md#map-crm-fields-inbound-mapping) pour obtenir des instructions complètes, notamment sur la manière de rendre les champs importés disponibles sous forme de filtres.

## Étapes suivantes

>[!MORELIKETHIS]
>
>* [Prospects](prospects.md)
>* [Workflows sortants](outbound-workflows.md)
