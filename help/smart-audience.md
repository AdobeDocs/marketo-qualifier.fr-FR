---
title: Audience intelligente (Beta)
description: Découvrez comment utiliser l’audience intelligente (Beta) pour créer des listes de comptes, ajouter des données CRM et des signaux de croissance, hiérarchiser les prospects et les ajouter à un workflow sortant.
feature: Agentic AI, Sales Insights, Account Journeys
role: User
badgeBeta: label="Beta" type="Informative"
source-git-commit: bf94a2d28913093923f446025405339e4e64919c
workflow-type: tm+mt
source-wordcount: '1125'
ht-degree: 1%
---

# Audience intelligente (Beta)

L’audience intelligente (Beta) vous aide à trouver les comptes et les personnes à utiliser ensuite dans [!DNL Adobe Marketo Qualifier]. Décrivez votre audience en langage simple, affinez la liste des comptes avec les données CRM et les signaux de croissance, recherchez les prospects pertinents et ajoutez les prospects sélectionnés à un workflow sortant.

Utilisez la vue Liste avec sa grille, ses filtres et ses boutons, ou utilisez le graphique pour décrire ce que vous souhaitez. Les deux fonctionnent sur la même liste : les modifications de l’une apparaissent dans l’autre. Si une modification n’apparaît pas immédiatement, sélectionnez **[!UICONTROL Actualiser]**.

Le suivi de progression en haut de chaque liste affiche trois étapes : **[!UICONTROL Créer une liste d’audiences intelligentes]**, **[!UICONTROL Hiérarchiser les prospects]** et **[!UICONTROL Ajouter au workflow sortant]**.

## Avant de commencer

L’audience intelligente nécessite un CRM Salesforce ou Microsoft Dynamics 365 connecté. Il lit les données du CRM en direct et n’écrit pas dans le CRM. Pour obtenir des instructions sur la connexion, voir [Prise en main](getting-started.md#connect-your-crm).

Vous pouvez créer jusqu’à 100 listes. Chaque liste contient jusqu’à 500 comptes et 2 000 prospects. Les comptes ou les prospects dépassant ces limites ne sont pas ajoutés. Limitez vos critères ou divisez l’audience en plusieurs listes, par exemple par région ou par segment.

## Description et prévisualisation des comptes

Commencez par une description des comptes que vous souhaitez atteindre. L’aperçu n’enregistre pas de liste.

1. Ouvrez **[!UICONTROL Audience intelligente]** et sélectionnez **[!UICONTROL Nouvelle audience intelligente]** ou **[!UICONTROL Créer une liste]**.
1. Dans le chat, décrivez les comptes que vous souhaitez. Par exemple, saisissez `Find healthcare accounts with revenue over $50M`.
1. Vérifiez le nombre de comptes correspondants et l’échantillon dans l’aperçu.

Votre demande peut inclure les critères suivants :

| Critères | Exemples |
| --- | --- |
| Données firmographiques | Secteur d’activité, nombre d’employés, chiffre d’affaires annuel, type de compte et évaluation |
| Emplacement | Région, pays, état ou ville |
| Propriété | Vos comptes ou comptes affectés à un propriétaire nommé |
| Pipeline | Comptes avec ou sans opportunité ouverte, soumis aux limites de [](#current-scope-and-limits) |
| Détails du compte | Nom, site web ou domaine et numéro de compte |

Voici d’autres exemples de requêtes :

* `Accounts in the US with more than 1000 employees`
* `My accounts in Germany or France`
* `Accounts with no open opportunity`

Si une partie d’une requête ne peut pas être appliquée à vos données CRM, la conversation identifie la condition ignorée. La prévisualisation reflète uniquement les conditions qui ont été appliquées. Passez en revue ces omissions avant d’enregistrer.

## Enregistrer ou affiner l’aperçu

Enregistrez l’aperçu lorsqu’il correspond à l’audience prévue.

1. Pour modifier l’aperçu, envoyez une nouvelle demande avec les conditions de votre choix. Rien n’est enregistré tant que vous n’avez pas confirmé.
1. Lorsque l’aperçu est prêt, demandez au chat de l’enregistrer en tant que liste et de donner un nom à la liste.
1. Examinez les comptes enregistrés dans l’onglet **[!UICONTROL Comptes]**.

Vous pouvez renommer une liste à partir de sa page. Pour supprimer une liste, ouvrez-la et sélectionnez **[!UICONTROL Supprimer la liste d’audience dynamique]**.

>[!CAUTION]
>
>La suppression d’une liste supprime définitivement ses comptes, prospects et colonnes de l’audience dynamique. Il ne supprime pas les enregistrements CRM.

## Enrichir et sélectionner des comptes

Ajoutez des colonnes d’informations pour vous aider à choisir les comptes à utiliser. Demandez une colonne ou un signal par demande.

Pour ajouter des informations CRM, saisissez une requête telle que `Add a column showing which accounts have an open opportunity`. Voir [Portée et limites actuelles](#current-scope-and-limits) pour connaître les restrictions de Salesforce.

Pour ajouter des signaux de croissance, sélectionnez **[!UICONTROL Enrichir les comptes]** dans la vue Liste ou demandez dans le chat. Les signaux disponibles sont les suivants :

| Signal | Ce qu’il montre |
| --- | --- |
| Financement | Événements récents de financement et de financement |
| Embauche | Offres d’emploi récentes et demande d’embauche |
| Signaux d&#39;extension | Nouveaux bureaux, nouveaux marchés et annonces d&#39;expansion |
| Changements technologiques | Ajouts et modifications à la pile technologique d&#39;une entreprise |
| Licenciements | Informations sur les mises à pied demandées par le biais du chat |

Par exemple, saisissez `Which of these accounts have raised funding recently?` ou `Which of these accounts have had layoffs?`.

Sur les listes volumineuses, l’ajout d’un signal peut prendre quelques minutes. Suivez la progression indiquée dans la liste, passez en revue chaque nouvelle colonne, puis conservez-la ou ignorez-la.

Pour limiter et classer par priorité les comptes :

1. Dans l’onglet **[!UICONTROL Comptes]**, ouvrez **[!UICONTROL Filtres]**.
1. Filtrez par compte, domaine, secteur, propriétaire, nombre minimal ou maximal d’employés, chiffre d’affaires minimal ou maximal ou colonnes personnalisées. Les colonnes personnalisées sont les colonnes CRM et signal que vous avez ajoutées. Par exemple, filtrez les comptes pour lesquels la colonne d’embauche est définie sur `Yes`.
1. Si vous le souhaitez, sélectionnez **[!UICONTROL Hiérarchiser les comptes]** pour classer les comptes par score.
1. Supprimez tous les comptes que vous ne souhaitez pas utiliser.

Les filtres sont enregistrés avec la liste. Les prospects sont disponibles uniquement pour les comptes filtrés. Définissez donc les filtres de compte avant de donner la priorité aux prospects.

## Recherche et hiérarchisation des prospects

Trouvez des personnes pertinentes dans les comptes que vous avez sélectionnés. Sous **[!UICONTROL Hiérarchiser les prospects]**, choisissez un paramètre prédéfini ou décrivez les personnes que vous souhaitez voir discutées.

| Préréglage | Contacts trouvés |
| --- | --- |
| **[!UICONTROL Contacts commerciaux]** | Directeur des ventes et contacts du directeur des ventes |
| **[!UICONTROL Contacts marketing]** | Vice-président des contacts Marketing et Marketing Manager |
| **[!UICONTROL Contacts produit]** | Contacts de produit et de responsable produit SVP |
| **[!UICONTROL Contacts technologiques]** | Directeur informatique et vice-président des contacts en ingénierie |
| **[!UICONTROL Tous les contacts CRM]** | Chaque contact disponible sur les comptes, jusqu’à la limite de 2 000 leads |

Pour une demande de conversation, saisissez `Find VP and Director level people at these accounts`, `Find C-level executives (CEO, CTO, CFO) at these accounts` ou `Find managers at these accounts`.

Consultez les résultats dans l’onglet **[!UICONTROL Leads]**. Chaque prospect affiche son nom, son titre, son compte, son adresse e-mail, son propriétaire et son score. Filtrez par ancienneté, si une adresse e-mail est disponible, score minimal ou maximal, ou si le prospect se trouve dans un workflow. La colonne **[!UICONTROL Raisonnement]** explique pourquoi chaque prospect est classé où il se trouve.

### Fonctionnement des scores

Les scores vont de 0 à 100. Un score plus élevé indique une meilleure adéquation et une meilleure préparation à l’engagement. Les mêmes données produisent le même score.

Un score combine :

* **Ajuster** : dans quelle mesure le compte correspond à votre profil client idéal, tel que le secteur et la taille.
* **Signaux d’achat et de croissance** : signaux tels que l’embauche, le financement et les changements de leadership. Les signaux récents comptent davantage.
* **Contexte des ventes** : contexte tel qu’un client existant avec une opportunité d’extension.

Examinez le raisonnement et les données disponibles avant de décider qui contacter.

## Ajouter des prospects à un workflow sortant

Après avoir examiné les prospects, ajoutez ceux de votre choix à un workflow sortant existant.

1. Dans l’onglet **[!UICONTROL Prospects]**, filtrez et sélectionnez les prospects souhaités. Par exemple, sélectionnez les prospects avec une adresse e-mail et un score minimum de 70.
1. Sélectionnez **[!UICONTROL Ajouter au workflow sortant]**.
1. Sélectionnez le workflow et confirmez-le.
1. Vérifiez la confirmation. La colonne **[!UICONTROL Workflow]** affiche **[!UICONTROL Affecté]** pour les prospects ajoutés.

Vous pouvez également demander à la discussion d’ajouter les prospects à un workflow par nom. Si vous ne connaissez pas le nom, demandez à la conversation de répertorier vos workflows disponibles. Vérifiez le nom du workflow et le nombre de leads dans la réponse.

L’ajout de prospects ne remplace pas la révision et l’approbation des e-mails. Suivez les étapes pour [examiner les e-mails générés](outbound-workflows.md#review-and-refine-generated-emails) et [approuver et inscrire les prospects](outbound-workflows.md#approve-and-enroll-prospects) avant l’envoi de la diffusion.

## Portée et limites actuelles

Pendant le Beta, gardez à l’esprit les points suivants :

* Demandez une colonne ou un signal par demande.
* L’audience dynamique utilise des champs de compte CRM standard. Les champs CRM personnalisés ne sont pas pris en charge.
* Le filtrage par produits détenus par un compte n’est pas pris en charge.
* Pour Salesforce, il n’est pas possible de rechercher les comptes ayant une opportunité ouverte. La recherche de comptes sans opportunité ouverte fonctionne avec les deux CRM.
* Pour Salesforce, les demandes d’embauche pour un rôle spécifique, comme un représentant commercial, ne sont pas disponibles.

>[!MORELIKETHIS]
>
>* [Comptes](accounts.md)
>* [Prospects](prospects.md)
>* [Workflows sortants](outbound-workflows.md)
>* [Conversation IA](ai-assistant.md)
