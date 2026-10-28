---
title: Prospects en [!DNL Adobe Marketo Qualifier]
description: Découvrez comment créer votre liste de prospects à partir de sources CRM, importées et ajoutées manuellement, filtrer les prospects et consulter les détails des prospects dans [!DNL Adobe Marketo Qualifier].
feature: Agentic AI, Sales Insights, Account Journeys
role: User
TQID: 'https://experienceleague.adobe.com/zf2H5rq1JlIT26LqLPMrm2Mq3tSIrLOiTEw6BXb1w2U'
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Marketo Qualifier
feature_v2:
  - id: da87d43a-78d4-4b1e-bb4a-743cbd343472
    internal-label: Prospects
subfeature_v2:
  - id: 6aa13f53-6e49-5228-b98a-64c9ebe5af74
    internal-label: Contacts
  - id: 4143255e-1853-5eb6-a189-dece7126669f
    internal-label: Leads
  - id: 78e1f6f5-7122-5e4d-81c3-d3a90e954414
    internal-label: People lists
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
topic_v2:
  - id: fd2e3797-f2ea-4b36-a9af-52acf5e90513
    internal-label: Customer profiles
source-git-commit: ab54d20ccc80d88c3592d89c9f43feeb062ed82c
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 1%
---

# Prospects

Pour afficher les prospects et les contacts auxquels vous pouvez accéder, sélectionnez **[!UICONTROL Prospects]** dans le volet de navigation de gauche. Utilisez la liste pour consulter le statut de chaque prospect et sa dernière activité.

![Tableau des prospects affichant le statut du prospect et la dernière activité pour la gestion des prospects](./assets/prospects.png){width="800" zoomable="yes"}

* **[!UICONTROL Leads]** Leads qui vous sont affectés dans le CRM connecté.
* **[!UICONTROL Contacts]** Contacts qui vous sont affectés dans le CRM connecté, avec leur compte associé. Les coordonnées comprennent également le nom du propriétaire. Ces détails sont disponibles pour Salesforce et Microsoft Dynamics 365.
* **[!UICONTROL Points forts marketing]** prospects disposant d’une activité Marketo en direct, comme les ouvertures d’e-mail ou les clics.
* **[!UICONTROL Liste des personnes]** Prospects que vous importez ou ajoutez manuellement.

## Consulter le contexte du prospect et exporter la liste

La liste des prospects résume si un contexte supplémentaire est disponible pour une diffusion personnalisée. Un résumé situé au-dessus de la liste indique le nombre de prospects dans chaque état, et la colonne Contexte affiche l&#39;état de chaque prospect :

* **[!UICONTROL Appliqué]** Le contexte disponible a été appliqué au prospect.
* **[!UICONTROL Partiel]** Seule une partie du contexte disponible a été appliquée.
* **[!UICONTROL Manquant]** Aucun contexte supplémentaire n’est disponible.

Pour télécharger la liste actuelle des prospects au format CSV, sélectionnez **[!UICONTROL Exporter CSV]**.

## Création de votre liste de prospects

La liste des prospects regroupe des personnes provenant de plusieurs sources :

* **Prospects CRM** : [!DNL Adobe Marketo Qualifier] importe automatiquement les leads et les contacts affectés à l&#39;utilisateur connecté. Pour plus d&#39;informations, consultez la section [&#x200B; Intégrations &#x200B;](integrations.md).
* **Prospects importés**—Prospects importés à partir d&#39;un fichier CSV.
* **Prospects ajoutés manuellement**—Prospects ajoutés individuellement dans Marketo Qualifier.

Pour ajouter des prospects qui ne proviennent pas de votre CRM :

1. Sur la page **[!UICONTROL Prospects]**, sélectionnez **[!UICONTROL Liste des personnes]**.

   ![Liste des personnes](assets/prospects-people-list.png){width="800" zoomable="yes"}

1. Sélectionnez **[!UICONTROL + Ajouter des personnes]** puis sélectionnez **[!UICONTROL Importer CSV]** ou **[!UICONTROL Ajouter une personne]**.

   * Pour un import CSV, chargez un fichier CSV au format `firstname,email`.
     Vous devez indiquer votre prénom et votre adresse e-mail. Le nom est facultatif. Le modèle CSV n’inclut pas la colonne d’ID de prospect CRM, mais vous pouvez ajouter la colonne et ses valeurs au fichier avant l’importation. Si l’importation échoue, consultez le message d’erreur pour les champs ou valeurs à corriger, puis chargez à nouveau le fichier.
     Mappez tous les champs CSV personnalisés ou supplémentaires, et pas seulement les champs standard. Marketo Qualifier enregistre ces valeurs pour chaque prospect et les rend disponibles ultérieurement, y compris pour la [&#x200B; génération d’e-mails](outbound-workflows.md#step-5-add-prospects-and-start-email-generation).
   * Pour ajouter une personne manuellement, saisissez ses détails dans le formulaire.

1. Sélectionnez **[!UICONTROL Enregistrer]**.

## Filtrer et rechercher des prospects

Pour réduire la liste, sélectionnez **[!UICONTROL Filtrer]**. Vous pouvez filtrer par :

* Statut du workflow sortant
* Création par
* Titre du traitement
* Compte
* Source
* Dernière mise à jour

Les administrateurs peuvent également rendre les champs CRM mappés disponibles en tant que filtres. Dans **[!UICONTROL Paramètres d’administration]**, activez **[!UICONTROL Filtrable]** pour chaque champ que les utilisateurs utilisent pour rechercher des prospects. Voir [&#x200B; Mappage des champs CRM &#x200B;](integrations.md#map-crm-fields-inbound-mapping).

Dans **[!UICONTROL Mes contacts d’opportunité]**, vous pouvez également filtrer les contacts par champs à partir des opportunités associées, telles que l’étape, le type et la date de fermeture. Les champs d’opportunité comportent des libellés tels que **[!UICONTROL Phase (Opportunité)]** qui les distinguent des champs de contact. Votre administrateur contrôle les champs d’opportunité disponibles en tant que filtres.

Vous pouvez également filtrer les contacts par champs du compte associé, tel que le secteur, la région ou le type de compte. Votre administrateur choisit les champs de compte filtrables. Combinez des filtres de compte, de contact et d’opportunité pour rechercher, par exemple, des contacts ayant un rôle spécifique dans des comptes d’un secteur spécifique. Le filtrage des champs de compte est disponible pour Salesforce et Microsoft Dynamics 365. Il est possible d’utiliser les mêmes champs dans le [ciblage des workflows sortants](outbound-workflows.md#step-2-configure-targeting-filters).

### Filtrer par points forts marketing

Examinez et hiérarchisez les prospects en fonction de leur engagement dans les [!DNL Marketo] en direct, comme l’activité des e-mails, les visites web et les remplissages de formulaires. L’engagement apparaît en temps quasi réel, comme cela se produit.

Pour filtrer les prospects par points forts marketing :

1. Sélectionnez **[!UICONTROL Filtrer]**.
1. Ajoutez un filtre Points forts marketing et définissez le type d’activité, la campagne ou d’autres attributs pour vous concentrer sur l’engagement qui compte.

Chaque prospect montre sa dernière activité [!DNL Marketo] ainsi que son historique récent.

L’option Points forts marketing est disponible dans toutes les régions de production. Un administrateur effectue une configuration unique qui connecte [!DNL Marketo] à Marketo Qualifier. Voir [Configurer les points forts marketing](integrations.md#turn-on-marketo-engagement-filtering).

## Consulter les détails du prospect

Pour ouvrir le profil d’un prospect, sélectionnez-le. Examinez les signaux qui comptent avant de vous adresser à :

* **Résumé de personne par IA** : instantané écrit par IA du prospect ou du contact et de son engagement récent. Utilisez le résumé pour comprendre rapidement la personne avant de passer en revue les activités individuelles. Les résumés des personnes par IA sont disponibles sur les instances s’exécutant [!DNL Marketo Optimizer] Prime ou Ultimate.
* **Liste des activités** : liste chronologique qui répertorie les 90 derniers jours d&#39;activité marketing.
* **Vue Chronologie** : chronologie visuelle qui affiche les 90 derniers jours d’engagement marketing sur l’ensemble des canaux.
* **Contenu affiché** : pages Web et ressources consultées par le prospect. Pour ouvrir un élément, sélectionnez-le.

### Générer la préparation de la réunion

Outre le résumé de la personne IA permanente, vous pouvez générer une préparation de réunion adaptée à un appel à venir spécifique à partir de l’onglet **[!UICONTROL Recherche de réunion]** en regard de **[!UICONTROL Recherche de compte]**.

La préparation de réunion associe les recherches sur le Web sur le prospect et son entreprise à des données issues d’études de cas sur des clients pairs qui utilisent le produit que vous vendez. Les points de discussion des études de cas peuvent inclure des résultats clients mesurables. Les sources sont regroupées en un seul mémoire, avec des points de discussion classés par pertinence. Chaque point de discussion permet de déterminer s’il provient d’études de cas, de recherches sur le Web ou des deux. Si aucune preuve d&#39;étude de cas pertinente n&#39;est disponible, la préparation de la réunion utilise la recherche sur le Web.

* **Basé sur un objectif** : si le prospect est inscrit à un workflow sortant en cours d’exécution, sélectionnez-le. La préparation correspond à l’objectif de ce workflow sortant, tel que réserver une réunion ou réengager le prospect.
* **Invite personnalisée**—Saisissez ce pour quoi vous souhaitez vous préparer, par exemple `Focus on renewal risk` ou `Prepare for a technical deep dive with their IT lead`. La préparation correspond à votre invite. L’option d’invite personnalisée est disponible lorsque le prospect ne se trouve pas dans un workflow sortant en cours d’exécution.

Le brief continue de suivre l’objectif du workflow sortant ou l’invite personnalisée que vous choisissez. La manière dont vous générez la préparation des réunions ne change pas.

>[!MORELIKETHIS]
>
>* [Comptes](accounts.md)
>* [Workflows sortants](outbound-workflows.md)
>* [Conversation IA](ai-assistant.md)
