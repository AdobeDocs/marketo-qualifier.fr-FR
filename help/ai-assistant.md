---
title: Utiliser le chat IA
description: Découvrez comment utiliser le Module de conversation sur l’IA [!DNL Adobe Marketo Qualifier] de rechercher des comptes, de rédiger des communications et d’obtenir des réponses en fonction de vos données CRM, d’engagement et de votre centre de connaissances.
feature: Agentic AI, Sales Insights, Account Journeys
role: User
TQID: 'https://experienceleague.adobe.com/LHCHAk0rsNwLsKFhKMlHaLL7xkkCEAKFNDMEonb2TdQ'
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Marketo Qualifier
feature_v2:
  - id: ace0d1fc-8e69-4e6a-a442-37fc40985eea
    internal-label: Account Qualification Agent
subfeature_v2:
  - id: 61dd0b55-ea2d-5210-8e27-63802e0f1d81
    internal-label: AI chat
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
topic_v2:
  - id: bbbea26f-9621-49eb-9ab8-e06fb3bbce8c
    internal-label: Artificial intelligence
source-git-commit: ab54d20ccc80d88c3592d89c9f43feeb062ed82c
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 1%
---

# Conversation sur l’IA

Le Chat IA répond aux questions en langage naturel en fonction de votre contexte de vente. Utilisez-le pour effectuer des recherches sur un compte, préparer un appel, rédiger un projet de sensibilisation et établir des priorités pour votre travail sans quitter [!DNL Adobe Marketo Qualifier].

![Bouton Conversation IA](assets/ai-chat.png){width="800" zoomable="yes"}

## Ouvrir le chat IA

Pour ouvrir le panneau de conversation, sélectionnez le bouton flottant **[!UICONTROL Conversation IA]**. Le panneau s’ouvre en regard de la page active afin que vous puissiez garder un prospect, un compte ou un workflow sortant en vue. Pour redimensionner le panneau, faites glisser son bord. Pour fermer le panneau, sélectionnez à nouveau **[!UICONTROL Conversation IA]**.

>[!NOTE]
>
>La disponibilité du Module de conversation sur l’IA dépend de la configuration de votre organisation et de vos autorisations. Si le bouton **[!UICONTROL Conversation IA]** n’apparaît pas, la fonctionnalité n’est pas activée pour votre compte.

## Sources de données

AI Chat peut utiliser les sources suivantes :

* Le guide de votre entreprise dans le [Centre de connaissances](admin-settings.md#knowledge-center).
* Votre CRM connecté, y compris les prospects, contacts, comptes, opportunités et activités.
* [!DNL Marketo] les données d’activité et d’engagement.
* Recherches sur les comptes et actualités récentes recueillies par le Account Qualification Agent.
* Recherche sur le Web public.

## Utiliser le chat IA

Utilisez le Module de conversation sur l’IA pour ces types de tâches :

* **Recherche et résumé** : demandez un résumé d’un compte, d’un groupe d’achat ou de l’engagement récent d’un prospect.
* **Créer le positionnement** : demandez à l’assistant de positionner votre solution pour un compte spécifique avant une réunion.
* **Rédiger et affiner la portée** : demandez-lui d’écrire ou de réécrire un e-mail. Indiquez la tonalité, la longueur, la langue et si vous souhaitez inclure des émoticônes.
* **Obtenir des recommandations** : demandez aux prospects ou aux comptes à prioriser ou demandez un objectif ou une cadence pour un nouveau workflow sortant.
* **Rechercher les coordonnées** : demandez à l’assistant d’enrichir un prospect avec plus d’informations de contact et d’arrière-plan.

## Discutez avec Ask AI sur vos données connectées

Le Chat IA peut répondre à des questions sur vos données [!DNL Marketo Qualifier], CRM, [!DNL Marketo], [!DNL Marketo Optimizer] et d’intelligence d’entreprise. Posez une question en langage clair pour rechercher des informations ou récupérer du contexte. Ces recherches de données connectées lisent et génèrent des rapports sur vos données ; elles ne créent, ne modifient ni ne lancent de programmes ou de campagnes.

Voici quelques exemples d’invites. Plus vous êtes précis dans votre invite, plus les résultats sont ciblés.

Prospects et comptes :

* « Rechercher des prospects avec statut d’engagement Nouveau. »
* « Effectuez des recherches sur la société Adobe. »
* « Donnez-moi le profil complet d&#39;un prospect. »
* « Afficher les performances sortantes pour les 30 derniers jours. »
* « Répertoriez les réunions réservées au cours des 30 derniers jours. »

Centre de connaissances :

* « Quelles garanties sont disponibles pour traiter les objections de prix ? »
* « Quels sont les principaux facteurs de différenciation par rapport aux concurrents ? »
* « Répertorier les documents dans le Centre de connaissances. »
* « Résumer un document. »

CRM :

* « Répertoriez les opportunités ouvertes. »
* « Répertoriez les cinq premiers prospects par nom et adresse électronique. »
* « Afficher les activités de vente pour un prospect ou un compte. »

[!DNL Marketo]:

* « Parcourir mes campagnes intelligentes. »
* « Obtenez la liste dynamique nommée « Acquis ». »
* « Parcourir mes programmes ou obtenir un programme par nom. »
* « Répertoriez [!DNL Marketo] types d’activités. »

[!DNL Adobe Journey Optimizer B2B Edition]:

* « Combien de parcours ai-je ? »
* « Comment le persona segmente-t-il mon audience ? »
* « Quelles pages de destination existent dans mon compte ? »
* « Quels champs de prospect alimentent la notation ? »

Renseignements sur l’entreprise :

* « Quelles technologies une entreprise utilise-t-elle ? »
* « Afficher les actualités récentes d&#39;une entreprise. »
* « Rechercher des sociétés similaires à une société donnée. »
* « Répertorier les offres d’emploi ouvertes pour une entreprise. »

### Portée et limites actuelles

* Les recherches de données connectées lisent et génèrent des rapports sur vos données. Ils ne créent pas de programme, ne lancent pas de campagne et ne modifient pas d’enregistrement CRM.
* Dans [Audience intelligente (Beta)](smart-audience.md) la conversation prend en charge les actions sur la liste des audiences, notamment l’enregistrement d’une liste, l’ajout de colonnes d’informations, le filtrage et la hiérarchisation des comptes et des prospects et l’ajout de prospects sélectionnés à un workflow sortant existant. Cela n’écrit pas dans le CRM ou ne remplace pas la révision et l’approbation des e-mails.
* AI Chat recherche des informations ; ce n&#39;est pas un outil de reporting. Il ne crée pas d’analyses ou de tendances de style [!DNL Marketo] au fil du temps, telles que l’intégrité des e-mails pour le trimestre ou une liste de prospects créés au cours des 10 derniers jours. Utilisez les rapports natifs de [!DNL Marketo] pour ces tâches.

## Réponses au sol dans votre playbook

Pour utiliser votre guide [Centre de connaissances](admin-settings.md#knowledge-center), reportez-vous au Centre de connaissances dans votre question. Par exemple :

`From the Knowledge Center, help me position our security solution for ABC Corp ahead of tomorrow's call.`

La réponse reflète le message de votre playbook.

## Donner son avis sur les réponses

Évaluez le contenu généré à l’aide des commandes de pouces vers le haut ou vers le bas. Vos commentaires contribuent à améliorer les réponses futures.

## Vérifier les réponses de l’IA

Les réponses générées par l’IA peuvent être inexactes. Examinez tout le contenu avant de l’utiliser.

* Vérifiez les faits, les noms et les chiffres avant de vous y fier.
* Lisez attentivement les brouillons d&#39;e-mails et personnalisez-les avant de les envoyer.
* Utiliser la sortie de l&#39;assistant comme point de départ, et non comme livrable terminé.

Les termes de l’IA générative d’Adobe régissent l’utilisation du chat IA par votre entreprise.

>[!MORELIKETHIS]
>
>* [ Centre de connaissances ](admin-settings.md#knowledge-center)
>* [Comptes](accounts.md)
>* [Workflows sortants](outbound-workflows.md)
