---
title: Paramètres d’administration
description: Découvrez comment gérer les champs CRM, la synchronisation des activités, le processus d’opt-out des e-mails et d’autres paramètres d’administration des [!DNL Adobe Marketo Qualifier].
feature: Agentic AI, Sales Insights, Account Journeys
role: Admin
internal-label: Administration
autotag-review: '2026-10-08T17:58:28.029Z'
TQID: 'https://experienceleague.adobe.com/2eccZWj1XY7qP20n6GcnBe6PZwNkp0ALhZfOhljwZF8'
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Sales Qualifier
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
  - id: fd2e3797-f2ea-4b36-a9af-52acf5e90513
    internal-label: Customer profiles
source-git-commit: bf94a2d28913093923f446025405339e4e64919c
workflow-type: tm+mt
source-wordcount: '1356'
ht-degree: 0%
---

# Paramètres d’administration

Utilisez **[!UICONTROL Paramètres d’administration]** pour configurer les intégrations CRM, gérer le Centre de connaissances et configurer le processus de désinscription aux e-mails.

[!DNL Adobe Marketo Qualifier] se connecte à Salesforce ou Microsoft Dynamics 365. La connexion donne au Account Qualification Agent (AQA) une vue cohérente des prospects, comptes, contacts, activités et propriétaires. Marketo Qualifier peut également écrire des activités de sensibilisation et un statut d’opt-out dans le CRM et synchroniser les activités de sensibilisation avec Marketo.

Pour configurer les connexions CRM, le mappage des champs et la synchronisation des activités, accédez à **[!UICONTROL Administration]** > **[!UICONTROL Paramètres d’administration]** > **[!UICONTROL Connexions CRM]**. Les utilisateurs standard peuvent utiliser les données et les filtres CRM configurés, mais ne peuvent pas modifier ces paramètres. Pour connecter un CRM pour la première fois, voir [Prise en main](getting-started.md#connect-your-crm).

>[!IMPORTANT]
>
>Pour accéder à **[!UICONTROL Paramètres d’administration]**, vous devez être membre des groupes d’utilisateurs `Marketo Qualifier` et `Marketo Qualifier Admins`.

## CRM MCP et le plug-in intégré

Marketo Qualifier fonctionne avec votre CRM des manières suivantes :

* **Requêtes CRM MCP** : les requêtes Account Qualification Agent interrogent les données CRM actives afin que les réponses et les informations reflètent l’état actuel de vos enregistrements.
* **Plug-in intégré** : le plug-in CRM affiche des informations [!DNL Marketo Sales Insights] (MSI) et des données agentiques dans votre CRM. Utilisez le plug-in pour ajouter un prospect à [!DNL Marketo Qualifier].
* **Synchronisation des activités** : lorsqu’un administrateur active **[!UICONTROL Synchronisation des activités]**, les activités d’extension se synchronisent avec le CRM et Marketo.

### Hiérarchiser les prospects dans le plug-in CRM

Le plug-in CRM fournit une page d’accueil par défaut où les représentants peuvent hiérarchiser les prospects sans quitter le CRM. Les onglets disponibles organisent le travail par source et par intention :

* **[!UICONTROL Meilleurs résultats]** : recommandations de leads prêtes à l’emploi.
* **[!UICONTROL Ma liste de surveillance]** — Leads que vous suivez.
* **[!UICONTROL Activité Web]** : visites récentes de sites par des prospects connus.
* **[!UICONTROL Activité Web anonyme]**—Visites de visiteurs non identifiés.
* **[!UICONTROL Mon e-mail]** : engagement par e-mail associé à vos prospects.
* **[!UICONTROL Webinaire]**—Inscription au webinaire et activité de présence.

Chaque prospect peut inclure un aperçu d’e-mail [!DNL Marketo], un lien vers les détails du prospect et des recherches sur LinkedIn. Les onglets et les données auxquels vous pouvez accéder dépendent de la configuration de votre plug-in CRM.

## Étendue de l’accès CRM

Marketo Qualifier lit les utilisateurs, les contacts, les mappages des propriétaires, les prospects, les comptes, les opportunités et les activités à partir du CRM. Il écrit uniquement les activités de sensibilisation consignées et le statut d’opt-out dans le CRM, et synchronise les activités de sensibilisation avec Marketo. Votre administrateur CRM prépare l’accès à l’API dans Salesforce ou Dynamics. Un administrateur Marketo Qualifier se connecte ensuite au CRM, mappe les champs entrants et choisit de synchroniser ou non les activités.

>[!NOTE]
>
>Les étapes d’identification de la section [Prise en main](getting-started.md#connect-your-crm) décrivent l’accès en lecture aux objets CRM. Si vous activez la synchronisation des activités ou l’écriture différée d’opt-out, contactez votre administrateur CRM pour obtenir l’accès en écriture correspondant à celui requis par votre configuration CRM.

## Mappage des champs CRM (mapping entrant)

Une fois le CRM connecté, sélectionnez **[!UICONTROL Gérer]** pour la connexion et ouvrez **[!UICONTROL Mapping entrant]**. Le mappage entrant contrôle les champs CRM que Marketo Qualifier extrait dans l’application.

1. Sélectionnez **[!UICONTROL Ajouter une section]**.
1. Saisissez un nom et une description de section.
1. Sélectionnez un type d’entité. **[!UICONTROL Prospects]** est sélectionné par défaut. **[!UICONTROL Contacts]**, **[!UICONTROL Comptes]** et **[!UICONTROL Opportunités]** sont également disponibles.
1. Pour importer des champs CRM, sélectionnez les champs.

   Chaque ligne de champ affiche ses **[!UICONTROL Nom d’affichage]**, **[!UICONTROL Nom du champ]** et **[!UICONTROL Type de données]**.

1. Activez **[!UICONTROL Filtrable]** pour chaque champ de prospect, contact, compte ou opportunité que vous souhaitez rendre disponible en tant que filtre sur la liste **[!UICONTROL Prospects]** et dans le [ciblage des workflows sortants](outbound-workflows.md#step-2-configure-targeting-filters).
1. Prévisualisez la section et sélectionnez **[!UICONTROL Ajouter]**.

Les champs mappés apparaissent dans les zones correspondantes de Marketo Qualifier :

* Les champs du prospect apparaissent dans l’onglet **[!UICONTROL Personne]**.
* Les champs Compte s’affichent dans l’onglet **[!UICONTROL Compte]**. Dans une section dotée du type d&#39;entité **[!UICONTROL Comptes]**, les champs peuvent être filtrés afin que les représentants puissent filtrer les contacts en fonction des attributs de leur compte associé, tels que le secteur, la région ou le type de compte.
* Les champs d’opportunité apparaissent dans la section **[!UICONTROL Opportunité de compte]**. Les champs d’opportunité filtrables apparaissent également comme leurs propres colonnes dans **[!UICONTROL Mes contacts d’opportunité]**, avec des libellés tels que **[!UICONTROL Étape (opportunité)]** pour les distinguer des champs de contact.

Le filtrage des champs de compte est disponible pour Salesforce et Microsoft Dynamics 365. Les représentants peuvent combiner des champs filtrables de compte, de contact et d&#39;opportunité pour rechercher des contacts et définir des critères de ciblage de workflow sortant.

## Configuration de la synchronisation des activités (mapping sortant)

1. Dans **[!UICONTROL Connexions CRM]**, sélectionnez **[!UICONTROL Gérer]** pour le CRM connecté.
1. Ouvrez **[!UICONTROL Mapping sortant]**.
1. Activez **[!UICONTROL Synchronisation des activités]** pour synchroniser les activités de sensibilisation Marketo Qualifier avec le CRM et Marketo.

Lorsque la synchronisation des activités est désactivée, Marketo Qualifier continue à utiliser les données CRM entrantes, mais ne synchronise pas les activités de sensibilisation avec votre CRM ou votre Marketo.

## Configuration des règles de synchronisation CRM

Marketo Qualifier peut automatiquement renvoyer les mises à jour de statut des prospects à Salesforce et Microsoft Dynamics lorsqu’un prospect se déplace dans un workflow sortant, de sorte que les représentants ne mettent plus à jour le CRM manuellement.

### À quoi servent les règles de synchronisation CRM

Une mise à jour peut cibler l’enregistrement **[!UICONTROL Lead]**, **[!UICONTROL Contact]**, **[!UICONTROL Compte]** ou **[!UICONTROL Opportunité]**, et pas seulement le lead.

Les mises à jour se déclenchent à ces moments de workflow sortant :

* Ajouté à un workflow, répondu ou réunion réservée
* Supprimé par un représentant ou workflow terminé sans réponse
* Opt-out ou e-mail bounce

Les valeurs de champ peuvent être personnalisées avec des jetons dynamiques afin que la mise à jour du CRM reflète le parcours réel du prospect plutôt qu’une valeur statique. Des jetons sont disponibles pour obtenir des détails tels que le nom du représentant, le nom du workflow sortant, ainsi que la date et l’heure de la réunion.

Seules les valeurs compatibles avec le CRM sont écrites, un champ en échec ne bloque pas les autres, et les problèmes temporaires réessayent automatiquement. Chaque mise à jour est suivie afin que vous puissiez voir ce qui a été synchronisé et ce qui requiert une attention particulière.

### Configurer des règles de synchronisation CRM

Pour configurer des règles de synchronisation CRM :

1. Dans le volet de navigation de gauche, développez **[!UICONTROL Administration]** et sélectionnez **[!UICONTROL Paramètres d’administration]** > **[!UICONTROL Connexions CRM]**.
1. Sélectionnez **[!UICONTROL Gérer]** pour le CRM connecté, puis sélectionnez **[!UICONTROL Règles de synchronisation]**.
1. Sélectionnez l’entité et les champs CRM cibles, mappez-les aux moments du workflow ci-dessus, puis activez le bouton (bascule).

Une fois les règles de synchronisation CRM configurées, les équipes commerciales bénéficient d’un statut précis, personnalisé et à jour des prospects, contacts, comptes et opportunités à chaque étape, avec moins de décalage des données et de travail manuel.

## Créer un guide pratique pour le centre de connaissances {#knowledge-center}

Le **[!UICONTROL Centre de connaissances]** donne à Account Qualification Agent (AQA) accès à vos documents de vente. Marketo Qualifier utilise ces ressources pour générer des recherches, des informations sur les qualifications et des informations qui reflètent les ventes de votre entreprise. Seuls les administrateurs peuvent créer et gérer le playbook.

![ Centre de connaissances ](assets/knowledge-center.png){width="800" zoomable="yes"}

1. Dans le volet de navigation de gauche, développez **[!UICONTROL Administration]**, sélectionnez **[!UICONTROL Paramètres d’administration]**, puis sélectionnez **[!UICONTROL Centre de connaissances]**.
1. Définissez les paramètres **[!UICONTROL Nom de la société]** et **[!UICONTROL URL de la société]** que Marketo Qualifier utilise pour effectuer des recherches dans votre société et rédiger des e-mails.
1. Chargez des pièces de théâtre commerciales, des profils client idéaux, des guides de positionnement et d’autres documents promotionnels au format PDF, PPTX ou DOCX.
1. Sélectionnez **[!UICONTROL Créer un playbook]**.

La page affiche le statut du playbook le plus récemment créé et fournit l’action suivante une fois le contenu chargé. Pour récupérer le dernier statut après une version, sélectionnez **[!UICONTROL Actualiser]**.

Chaque document chargé affiche également son statut de traitement, tel que **[!UICONTROL Prêt]**, et la date de sa dernière mise à jour.

>[!NOTE]
>
>Le traitement d’un playbook peut prendre jusqu’à 24 heures.

Lorsque le manuel est prêt, les représentants peuvent l’utiliser à deux endroits :

* **Invites de courrier électronique sortant** : dans une invite de point de contact, nommez le document et décrivez le contexte à utiliser. Par exemple, saisissez `Use the ABC positioning guide from the Knowledge Center and focus on the security value proposition`. Voir [ Configuration des points de contact ](outbound-workflows.md#step-3-generate-and-review-touchpoints).
* **Chat IA** : Reportez-vous au Centre de connaissances dans votre question. Par exemple, saisissez `From the Knowledge Center, help me position our security solution for ABC Corp before tomorrow's call`. Voir [Conversation IA](ai-assistant.md).

Dans les deux cas, le contenu généré reflète le message de votre playbook plutôt que la recherche générique.

## Configuration du processus d’opt-out global des e-mails

1. Dans le volet de navigation de gauche, développez **[!UICONTROL Administration]** et sélectionnez **[!UICONTROL Paramètres d’administration]**.
1. Sélectionnez **[!UICONTROL Paramètres de messagerie]** sous **[!UICONTROL Conformité]**.
1. Activez **[!UICONTROL Inclure un lien d’opt-out dans chaque e-mail]** pour ajouter un pied de page de désabonnement aux e-mails sortants.
1. Dans **[!UICONTROL Modèle de message d’opt-out]**, saisissez le texte du pied de page. Incluez le jeton `{opt_out_link}` où le lien de désabonnement doit apparaître.

Les paramètres sont enregistrés automatiquement.

Lorsqu’un prospect sélectionne le lien, Marketo Qualifier cesse d’envoyer des e-mails à ce prospect et synchronise le statut de désinscription sur le CRM connecté. Marketo Qualifier reconnaît également les demandes de désinscription claires dans la réponse par e-mail d’un prospect, telles que « veuillez arrêter de m’envoyer un e-mail » ou « désabonner », et marque le prospect comme étant automatiquement désabonné. Le même statut et le même badge **[!UICONTROL Opt-out]** s’appliquent et aucun autre point de contact n’est envoyé. Aucune configuration supplémentaire n’est nécessaire. Les réponses qui ne demandent pas clairement à arrêter, comme « pas maintenant », ne sont pas traitées comme des opt-outs. Voir [Demandes d’opt-out dans les réponses](outbound-workflows.md#opt-out-requests-in-replies).

## Référence : exemples de paramètres d’API

Votre équipe CRM peut utiliser ces exemples pour confirmer que l’accès en lecture renvoie les champs de prospect attendus.

### Exemple OData Dynamics

```text
$select=fullname,_ownerid_value,leadid,emailaddress1,jobtitle,statuscode,createdon,modifiedon,statecode
$filter=_ownerid_value eq '<crmUserId>' [AND additional filters]
$expand=Lead_ActivityPointers(...),parentaccountid(...)
$orderby=modifiedon desc
```

### Exemple SOQL Salesforce

```sql
SELECT Id, Salutation, FirstName, LastName, Name, Title, Company, Email,
  LeadSource, Status, OwnerId, LastModifiedDate, LastActivityDate, CreatedDate,
  (SELECT Id, Subject, ActivityDate, Status FROM Tasks ORDER BY ActivityDate DESC LIMIT 1),
  (SELECT Id, Subject, ActivityDateTime FROM Events ORDER BY ActivityDateTime DESC LIMIT 1)
FROM Lead
WHERE OwnerId = '<crmUserId>' AND IsDeleted = false
ORDER BY LastModifiedDate DESC
```

>[!MORELIKETHIS]
>
>* [Prise en main](getting-started.md)
>* [Prospects](prospects.md)
