---
title: Prospects en [!DNL Adobe Marketo Qualifier]
description: Découvrez comment créer votre liste de prospects à partir de sources CRM, importées et ajoutées manuellement, filtrer les prospects et consulter les détails des prospects dans [!DNL Adobe Marketo Qualifier].
feature: Agentic AI, Sales Insights, Account Journeys
role: User
TQID: 'https://experienceleague.adobe.com/zf2H5rq1JlIT26LqLPMrm2Mq3tSIrLOiTEw6BXb1w2U'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
feature_v2:
  - id: fc7979f3-56c3-43ca-9784-f1ea3dc69c4b
    internal-label: Integrations
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 2124387555f5fb08ea19eaf121fc87aa66d66de2
workflow-type: tm+mt
source-wordcount: '755'
ht-degree: 1%
---

# Prospects

Pour afficher les prospects et les contacts auxquels vous pouvez accéder, sélectionnez **[!UICONTROL Prospects]** dans le volet de navigation de gauche. Utilisez la liste pour consulter le statut de chaque prospect et sa dernière activité.

![Tableau des prospects affichant le statut du prospect et la dernière activité pour la gestion des prospects](./assets/prospects.png){width="800" zoomable="yes"}

* **[!UICONTROL Leads]** Leads qui vous sont affectés dans le CRM connecté.
* **[!UICONTROL Contacts]** Contacts qui vous sont affectés dans le CRM connecté.
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

* **Prospects CRM** : [!DNL Adobe Marketo Qualifier] importe automatiquement les leads et les contacts affectés à l&#39;utilisateur connecté. Pour plus d&#39;informations, consultez la section [ Intégrations ](integrations.md).
* **Prospects importés**—Prospects importés à partir d&#39;un fichier CSV.
* **Prospects ajoutés manuellement**—Prospects ajoutés individuellement dans le qualificateur Marketo.

Pour ajouter des prospects qui ne proviennent pas de votre CRM :

1. Sur la page **[!UICONTROL Prospects]**, sélectionnez **[!UICONTROL Liste des personnes]**.

   ![Liste des personnes](assets/prospects-people-list.png){width="800" zoomable="yes"}

1. Sélectionnez **[!UICONTROL + Ajouter des personnes]** puis sélectionnez **[!UICONTROL Importer CSV]** ou **[!UICONTROL Ajouter une personne]**.

   * Pour un import CSV, chargez un fichier CSV au format `firstname,email`.
     Vous devez indiquer votre prénom et votre adresse e-mail. Le nom est facultatif. Le modèle CSV n’inclut pas la colonne d’ID de prospect CRM, mais vous pouvez ajouter la colonne et ses valeurs au fichier avant l’importation. Si l’importation échoue, consultez le message d’erreur pour les champs ou valeurs à corriger, puis chargez à nouveau le fichier.
     Mappez tous les champs CSV personnalisés ou supplémentaires, et pas seulement les champs standard. Marketo Qualifier enregistre ces valeurs pour chaque prospect et les rend disponibles ultérieurement, y compris pour la [ génération d’e-mails](outbound-workflows.md#step-5-add-prospects-and-start-email-generation).
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

Les administrateurs peuvent également rendre les champs CRM mappés disponibles en tant que filtres. Dans **[!UICONTROL Paramètres d’administration]**, activez **[!UICONTROL Filtrable]** pour chaque champ que les utilisateurs utilisent pour rechercher des prospects. Voir [ Mappage des champs CRM ](integrations.md#map-crm-fields-inbound-mapping).

Dans **[!UICONTROL Mes contacts d’opportunité]**, vous pouvez également filtrer les contacts par champs à partir des opportunités associées, telles que l’étape, le type et la date de fermeture. Les champs d’opportunité comportent des libellés tels que **[!UICONTROL Phase (Opportunité)]** qui les distinguent des champs de contact. Votre administrateur contrôle les champs d’opportunité disponibles en tant que filtres.

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
* **Liste des activités**—Liste chronologique des activités et des comportements récents.
* **Vue Chronologie** : chronologie visuelle de l’engagement sur plusieurs canaux.
* **Contenu affiché** : pages Web et ressources consultées par le prospect. Pour ouvrir un élément, sélectionnez-le.

### Générer la préparation de la réunion

Outre le résumé de la personne IA permanente, vous pouvez générer une préparation de réunion adaptée à un appel à venir spécifique à partir de l’onglet **[!UICONTROL Recherche de réunion]** en regard de **[!UICONTROL Recherche de compte]**.

* **Basé sur un objectif** : si le prospect est inscrit à un workflow sortant en cours d’exécution, sélectionnez-le. La préparation correspond à l’objectif de ce workflow sortant, tel que réserver une réunion ou réengager le prospect.
* **Invite personnalisée**—Saisissez ce pour quoi vous souhaitez vous préparer, par exemple `Focus on renewal risk` ou `Prepare for a technical deep dive with their IT lead`. La préparation correspond à votre invite. L’option d’invite personnalisée est disponible lorsque le prospect ne se trouve pas dans un workflow sortant en cours d’exécution.

>[!MORELIKETHIS]
>
>* [Comptes](accounts.md)
>* [Workflows sortants](outbound-workflows.md)
>* [Conversation IA](ai-assistant.md)
