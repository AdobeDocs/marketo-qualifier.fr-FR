---
title: Notes de mise à jour d’[!DNL Adobe Marketo Qualifier]
description: Découvrez les nouveautés de la version [!DNL Adobe Marketo Qualifier].
feature: Agentic AI, Sales Insights, Account Journeys
role: User
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Marketo Qualifier
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: ab54d20ccc80d88c3592d89c9f43feeb062ed82c
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 11%
---
# Notes de mise à jour d’[!DNL Adobe Marketo Qualifier]

## Version à venir

* Recherchez et hiérarchisez les comptes et les prospects appropriés avec l’audience intelligente (Beta). Décrivez en langage simple les comptes souhaités, ajoutez des données CRM et des signaux de croissance, passez en revue les prospects notés et ajoutez-les à un workflow sortant. [En savoir plus](smart-audience.md).
* Filtrez les contacts par champs de compte, à côté des champs de contact et d’opportunité, pour trouver les contacts appropriés et cibler plus précisément les workflows sortants. [En savoir plus](prospects.md#filter-and-find-prospects).
* Les contacts affichent leur compte associé et le nom du propriétaire, et la page d’un prospect affiche désormais 90 jours d’activité marketing, contre 30 auparavant. [En savoir plus](prospects.md#review-prospect-details).

## 10-08-2026

Cette version comprend les éléments suivants :

* Réutiliser un workflow sortant ou modifier les points de contact d’un workflow en cours d’exécution, le dupliquer et modifier la copie. La copie démarre comme un brouillon privé sans prospects et le workflow d’origine reste inchangé. [En savoir plus](outbound-workflows.md#duplicate-an-outbound-workflow).
* Configurez les workflows sortants dans une disposition compacte avec une navigation entre l’objectif, le ciblage, les points de contact et les paramètres. [En savoir plus](outbound-workflows.md#create-an-outbound-workflow).
* Les demandes de désinscription effacées dans les réponses par e-mail sont automatiquement reconnues. Le prospect est marqué comme étant exclu et aucun autre point de contact n’est envoyé. [En savoir plus](outbound-workflows.md#opt-out-requests-in-replies).
* Préparez-vous aux réunions avec un seul résumé qui combine des recherches sur le Web et des études de cas clients spécifiques à des produits, avec des points de discussion classés par pertinence et des sources identifiées. [En savoir plus](prospects.md#generate-meeting-prep).
* Les e-mails générés sont vérifiés par rapport aux directives de qualité et réécrits si nécessaire avant que vous les examiniez. Vous révisez, modifiez et approuvez toujours chaque e-mail avant son envoi. [En savoir plus](outbound-workflows.md#review-and-refine-generated-emails).

## 09-22-2026

Cette version comprend les éléments suivants :

* Affichez les données [!DNL Marketo Sales Insights] et agentiques dans le plug-in CRM incorporé et ajoutez des prospects aux [!DNL Marketo Qualifier]. [En savoir plus](admin-settings.md#crm-mcp-and-the-embedded-plugin).
* Hiérarchisez les prospects CRM avec les meilleurs résultats, ma liste de surveillance, l’activité web, l’engagement par e-mail et l’activité de webinaire. [En savoir plus](admin-settings.md#prioritize-leads-in-the-crm-plugin).
* Inscrivez automatiquement les prospects aux workflows sortants lorsque leur activité Live [!DNL Marketo] correspond aux critères du workflow. [En savoir plus](home.md#automatically-enroll-prospects-from-marketing-highlights).
* Passez en revue le contexte du prospect, exportez la liste des prospects et affichez les résumés de personne IA sur les instances Prime et Ultimate [!DNL Marketo Optimizer]. [En savoir plus](prospects.md#review-prospect-context-and-export-the-list).
* Examinez et approuvez les e-mails de prospects générés provenant de la file d’attente des tâches et répondez avec des suggestions d’agent pendant un workflow sortant. [En savoir plus](tasks.md).

## 09-08-2026

Cette version comprend les éléments suivants :

* Définissez votre propre style de dessin d’e-mail une fois dans les paramètres de profil, et chaque e-mail généré le suit. [En savoir plus](profile-settings.md#email-drafting-context).
* Générez une préparation de réunion personnalisée ou basée sur des objectifs à partir de la page d&#39;un prospect, dans un nouvel onglet de recherche de réunion. [En savoir plus](prospects.md#generate-meeting-prep).
* Les administrateurs peuvent affecter un workflow sortant à un coéquipier et réinitialiser les paramètres de workflow sur leurs valeurs par défaut. [En savoir plus](outbound-workflows.md#create-an-outbound-workflow).
* Mappez des champs personnalisés lors de l’importation de prospects à partir d’un fichier CSV et utilisez ces valeurs dans les e-mails générés. [En savoir plus](prospects.md#build-your-prospect-list).
* Les e-mails générés utilisent toutes les données supplémentaires du prospect que vous importez et peuvent être écrits en mode natif dans sa langue. [En savoir plus](outbound-workflows.md#step-5-add-prospects-and-start-email-generation).
* Performances sortantes affiche le taux d’ouverture et le taux de clics par défaut, avec un bouton (bascule) pour les nombres bruts et le nombre total de prospects au niveau de l’organisation. [En savoir plus](performance.md).
* Les règles de synchronisation CRM mettent automatiquement à jour le statut du CRM lorsqu’un prospect se déplace dans un workflow sortant. [En savoir plus](admin-settings.md#configure-crm-sync-rules).
* Posez des questions sur le Chat IA sur vos données [!DNL Marketo Qualifier], CRM, [!DNL Marketo] et [!DNL Marketo Optimizer]. [En savoir plus](ai-assistant.md#ask-ai-chat-across-your-connected-data).

## 08-17-2026

[!DNL Marketo Qualifier] est désormais disponible en tant qu’application autonome. Il prend en charge [!DNL Marketo Engage] et [!DNL Marketo Optimizer].

Cette version comprend les éléments suivants :

* Hiérarchisation des prospects et des comptes avec des résumés des activités générés par l’IA et une notation basée sur les signaux. [En savoir plus](prospects.md#review-prospect-details) sur les prospects ou les [comptes](accounts.md#account-insights).
* Workflows sortants pilotés par des objectifs avec cadences proposées par l’IA et brouillons d’e-mails. [En savoir plus](outbound-workflows.md).
* Une file d’attente de tâches unifiée pour les appels téléphoniques, LinkedInMails et les révisions d’e-mails. [En savoir plus](tasks.md).
* Réservation automatique des réunions via l&#39;intégration du calendrier. [En savoir plus](outbound-workflows.md#meeting-booking).
* Un centre de connaissances pour ancrer la sensibilisation à l’IA dans votre propre matériel de playbook. [En savoir plus](admin-settings.md#knowledge-center).
* Discutez avec l’IA pour poser des questions en langage naturel en fonction de vos données CRM, d’engagement et de centre de connaissances. [En savoir plus](ai-assistant.md).
* Rapports sur les performances des e-mails et des réservations de réunions. [En savoir plus](performance.md).
* Plug-ins de navigateur et d’e-mail pour accéder à votre CRM ou Outlook. [En savoir plus](admin-settings.md#crm-mcp-and-the-embedded-plugin).
* Prise en charge des intégrations Salesforce et Microsoft Dynamics 365. [En savoir plus](integrations.md).
