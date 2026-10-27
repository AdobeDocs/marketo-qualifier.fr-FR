---
title: Tâches dans [!DNL Adobe Marketo Qualifier]
description: Découvrez comment traiter les tâches de sensibilisation manuelles et examiner les prospects suggérés par l’agent dans la file d’attente de tâches [!DNL Adobe Marketo Qualifier].
feature: Agentic AI, Sales Insights, Account Journeys
role: User
TQID: 'https://experienceleague.adobe.com/MbTN1r-ARrW-XYtdIS-KZT7K1Lk-B3GihT8iXL60GrQ'
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Marketo Qualifier
feature_v2:
  - id: d7511d14-12fe-4594-9d3b-65310015f8cb
    internal-label: Tasks
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
    internal-label: Customer engagement
source-git-commit: fcdc5d36cbb1500cf984e1439291aa8dbf17b72b
workflow-type: tm+mt
source-wordcount: '1086'
ht-degree: 0%
---

# Tâches

Utilisez **[!UICONTROL Tâches]** pour exécuter les actions générées par les workflows sortants. Sélectionnez une tâche, effectuez une action, marquez la tâche comme terminée et passez à la tâche suivante sans quitter la page.

Dans le volet de navigation de gauche, accédez à **[!UICONTROL Activités]** > **[!UICONTROL Tâches]**.

![Panneau Tâche](assets/tasks.png)

## Vues des tâches

La page comporte deux onglets :

* **[!UICONTROL Tâches manuelles]**—Appels téléphoniques, LinkedInMails et révisions d&#39;e-mails pour les prospects inscrits à un workflow sortant.
* **[!UICONTROL Suggestions d’agent]** : prospects correspondant aux critères de ciblage d’un workflow sortant et recommandés pour l’inscription.

Chaque onglet possède ses propres filtres, options de tri et disposition à deux panneaux. La liste des tâches s’affiche à gauche, et le panneau de travail à droite. La sélection d’une tâche charge ses détails dans le panneau de travail. Lorsque vous terminez une tâche, la tâche suivante est automatiquement sélectionnée.

## Tâches manuelles

### Types de tâches

Les tâches manuelles sont liées aux étapes de workflow sortant et existent en trois types :

* **[!UICONTROL Appel téléphonique]** : créé lorsqu’une cadence atteint une étape d’appel téléphonique. Le panneau de travail affiche le numéro de téléphone du prospect et, le cas échéant, un script d’appel généré par l’IA.

* **[!UICONTROL LinkedInMail]** : créé lorsqu’une cadence atteint une étape LinkedInMail. Le panneau de travail affiche le contenu à copier et à envoyer à partir de LinkedIn. Développez **[!UICONTROL Justification de l’IA]** pour en examiner la justification.

* **[!UICONTROL Révision d’e-mail]** : créé après [!DNL Adobe Marketo Qualifier] génère les e-mails personnalisés d’un prospect. Pour examiner et approuver les brouillons avant le début de la diffusion, sélectionnez **[!UICONTROL Réviser les e-mails]**. Voir [Vérifier et affiner les emails générés](outbound-workflows.md#review-and-refine-generated-emails).

![Email Review](assets/tasks-review.png)

### Le panneau de travail

Pour une tâche **[!UICONTROL Appel téléphonique]** ou **[!UICONTROL LinkedInMail]**, le panneau de travail contient :

* **[!UICONTROL Prospect]** : le nom du prospect, le lien de l&#39;e-mail et le numéro de téléphone, le cas échéant.
* **[!UICONTROL Workflow sortant]** : nom du workflow sortant lié, date d’échéance et indicateur d’omission automatique, le cas échéant.
* **Contenu de la tâche** : script d&#39;appel ou contenu InMail.
* **[!UICONTROL Notes]** : les notes sont enregistrées automatiquement lorsque vous sélectionnez une autre tâche. Vous ne pouvez pas modifier de notes une fois qu’une tâche est terminée, ignorée ou annulée.

### Générer un script d’appel

Pour une tâche **[!UICONTROL Appel téléphonique]**, sélectionnez **[!UICONTROL Générer le script d’appel]**. Une fois la génération terminée, sélectionnez **[!UICONTROL Afficher le script d’appel détaillé]**. Si la génération échoue, réessayez à partir du panneau.

### Actions liées à la tâche

Deux actions sont disponibles à partir de l’en-tête du panneau de travail :

* **[!UICONTROL Marquer comme terminé]** : utilisez cette action après avoir passé l&#39;appel, envoyé l&#39;InMail ou examiné les e-mails. La file d&#39;attente passe à la tâche suivante.
* **[!UICONTROL Ignorer]** : utilisez cette action lorsque vous ne pouvez pas terminer l’étape, mais que vous souhaitez conserver le prospect dans le workflow sortant. Le prospect passe à l’étape de cadence suivante.

Les tâches d’appel téléphonique et LinkedInMail peuvent être automatiquement ignorées si elles restent ouvertes au-delà du seuil configuré. Un saut automatique fait progresser le prospect tout au long de la cadence et n’affecte pas les points de contact d’e-mail planifiés.

### Filtrer, rechercher et trier

La barre d’outils située au-dessus de la liste contrôle les tâches qui apparaissent et dans quel ordre. Vos choix de filtre et de tri sont enregistrés et réappliqués la prochaine fois que vous ouvrez la page.

* **[!UICONTROL Filtrer]** : permet d&#39;ouvrir le panneau de filtrage :
  * **[!UICONTROL Statut]**—**[!UICONTROL Actuel]**, **[!UICONTROL À Venir]**, **[!UICONTROL En Retard]**, **[!UICONTROL Terminé]**, **[!UICONTROL Annulé]**, **[!UICONTROL Ignoré]**.
  * **[!UICONTROL Type de tâche]**—**[!UICONTROL Révision par e-mail]**, **[!UICONTROL LinkedIn InMail]**, **[!UICONTROL Appel téléphonique]**.
  * **[!UICONTROL Date d’échéance]**.
  * **[!UICONTROL Workflow sortant]** : liste interrogeable de vos workflows sortants.
* **[!UICONTROL Trier]**—Trier par date d&#39;échéance ou date de création. L’ordre de tri détermine également l’ordre dans lequel la file d’attente avance.
* **[!UICONTROL Rechercher des tâches]** : recherchez des tâches par nom de prospect, nom de société ou workflow sortant. La recherche s’applique avec les filtres actifs.

Les filtres actifs s’affichent sous forme de puces sous la barre d’outils. Pour les réinitialiser, sélectionnez **[!UICONTROL Effacer tout]**.

### Statut de la tâche

Chaque tâche affiche son statut actuel :

| Statut | Description |
| --- | --- |
| **[!UICONTROL Actuel]** | Dû maintenant et prêt à agir. Les tâches actuelles n’affichent aucun badge. |
| **[!UICONTROL À venir]** | L’étape précédente est terminée, mais la date d’échéance se situe dans le futur. Vous pouvez agir tôt si le moment est venu. |
| **[!UICONTROL En retard]** | A dépassé la date d&#39;échéance et n&#39;est pas encore terminé. La tâche est marquée pour attention. |
| **[!UICONTROL Terminé]** | Vous avez terminé l’action et marqué la tâche comme terminée. |
| **[!UICONTROL Ignoré]** | Vous avez ignoré l’étape ou elle a été automatiquement ignorée. Le prospect progresse dans le workflow sortant. |
| **[!UICONTROL Annulé]** | Le système a annulé la tâche en raison d&#39;une modification du workflow sortant. |

Les tâches terminées, ignorées et annulées sont finales. Leurs actions ne sont plus disponibles et leurs notes sont en lecture seule.

## Suggestions d’agent

L’onglet **[!UICONTROL Suggestions d’agent]** répertorie les prospects correspondant aux critères de ciblage d’un workflow sortant et sont recommandés pour l’inscription. Pour activer les recommandations, voir [Workflows sortants](outbound-workflows.md).

Pour examiner une suggestion dans le panneau de travail, sélectionnez-la :

* Un badge de récence marque chaque suggestion comme **[!UICONTROL Nouvelle]** ou **[!UICONTROL Précédente]**.
* Le tableau **[!UICONTROL Prospects recommandés]** ou **[!UICONTROL Contacts recommandés]** répertorie les prospects proposés avec des colonnes pour **[!UICONTROL Nom]**, **[!UICONTROL Titre]**, **[!UICONTROL Compte]**, **[!UICONTROL Status]**, **[!UICONTROL Email]** et **[!UICONTROL Dernière mise à jour]**.

Deux actions sont disponibles :

* **[!UICONTROL Vérifier les prospects]**—Ouvrez le workflow sortant pour vérifier et inscrire les prospects recommandés. Voir [ Ajouter des prospects et commencer la génération d’e-mails](outbound-workflows.md#step-5-add-prospects-and-start-email-generation).
* **[!UICONTROL Marquer comme terminé]**—Ignorez la suggestion après l&#39;avoir examinée.

L’onglet **[!UICONTROL Suggestions d’agent]** comprend les filtres de statut **[!UICONTROL Actuel]**, **[!UICONTROL Terminé]** et **[!UICONTROL Annulé]**, un filtre Workflow sortant et un tri par date de création.

### Répondre à un prospect avec une suggestion d’agent

Lorsqu’un prospect répond à un e-mail, [!DNL Marketo Qualifier] pouvez rédiger une réponse intégrée et l’ajouter en tant que tâche sous **[!UICONTROL Suggestions d’agent]**. Le projet utilise le contexte pertinent suivant :

* Le thread d’e-mail complet, pas seulement le dernier message.
* Recherche de produits et documentation connexe de votre centre de connaissances.
* Signaux de compte, tels que les nouvelles récentes, l’engagement marketing et l’activité CRM.
* Votre [contexte de rédaction d’e-mail](profile-settings.md#email-drafting-context) enregistré.

L&#39;assistant adapte la réponse à l&#39;intention du prospect. Par exemple, il peut offrir des heures par le biais de votre lien de réservation pour une demande de réunion, renforcer la valeur lorsque le prospect est intéressé, répondre à une question sur un produit à partir de votre garantie, partager un actif pertinent, répondre à une objection avec un facteur de différenciation ou utiliser une réponse à faible pression lorsque le prospect souhaite différer.

Des messages sur les prix, les exigences légales ou de sécurité, les réponses hostiles et les demandes peu claires restent au représentant pour une réponse personnelle.

1. Ouvrez la suggestion de réponse et examinez le thread complet et la réponse brouillée.
1. Pour créer un autre brouillon, modifiez la réponse ou sélectionnez **[!UICONTROL Générer avec l’IA]**.
1. Pour envoyer la réponse et poursuivre le workflow sortant du prospect, sélectionnez **[!UICONTROL Approuver et envoyer]**.

## Effectuer des tâches à partir d’un workflow sortant

Sur la vue **[!UICONTROL Prospects engagés]** d’un workflow sortant, un point de contact manuel fournit les mêmes options **[!UICONTROL Marquer comme terminé]**, **[!UICONTROL Ignorer]** et Notes. Y terminer une tâche met également à jour son statut sur la page **[!UICONTROL Tâches]**. Voir [Workflows sortants](outbound-workflows.md).

## États vides

* Lorsque vous n’avez aucune tâche à effectuer, la liste affiche un message _Vous êtes tous pris pour aujourd’hui_.
* Lorsque les filtres ne correspondent à aucune tâche, la liste indique qu’aucune tâche ne correspond à vos filtres.
* Lorsqu’aucune tâche n’est sélectionnée, le panneau de travail vous invite à sélectionner une tâche. Pour afficher les détails, sélectionnez une tâche.

>[!MORELIKETHIS]
>
>* [Workflows sortants](outbound-workflows.md)
>* [Performance sortante](performance.md)
>* [Prospects](prospects.md)
