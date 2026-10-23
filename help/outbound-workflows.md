---
title: Créer et gérer des workflows sortants
description: Découvrez comment créer, partager, réviser et gérer des workflows sortants générés par l’IA dans [!DNL Adobe Marketo Qualifier] d’exécuter des cadences de sensibilisation pilotées par les objectifs.
feature: Agentic AI, Sales Insights, Account Journeys
role: User
TQID: 'https://experienceleague.adobe.com/n3FbuiM2zF9QSqaKx1bhBSdbsf-w7vEsEGjCQTBo3g4'
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Sales Qualifier
feature_v2:
  - id: fc7979f3-56c3-43ca-9784-f1ea3dc69c4b
    internal-label: Integrations
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: bf94a2d28913093923f446025405339e4e64919c
workflow-type: tm+mt
source-wordcount: '2776'
ht-degree: 0%
---

# Workflows sortants

Un workflow sortant est une cadence de diffusion pilotée par les objectifs. Vous définissez l’objectif et les critères de ciblage. L’IA propose ensuite une cadence multipoint et écrit du contenu d’e-mail personnalisé pour chaque prospect. Avant d’activer le rythme, passez en revue et approuvez chaque e-mail.

Un workflow sortant connecte quatre éléments :

* **Objectif** : résultat que vous attendez de la sensibilisation, tel que la réservation d’un appel de découverte ou l’augmentation de l’enregistrement à un événement.
* **Filtres de ciblage**—Conditions déterminant les prospects éligibles.
* **Cadence des points de contact** : séquence ordonnée d’étapes d’e-mail, d’appel téléphonique et LinkedInMail.
* **Contenu d’e-mail personnalisé** : contenu généré par l’IA en fonction du profil du prospect, du contexte du compte, de l’historique de l’engagement et des actualités récentes.

L’IA utilise l’objectif pour suggérer des filtres de ciblage, concevoir la cadence, créer des brouillons d’invites de point de contact et personnaliser chaque e-mail généré.

## Principaux concepts

| Concept | Description |
| --- | --- |
| **Workflow sortant** | Activité sortante réutilisable définie par un objectif, des filtres de ciblage, une cadence et des paramètres. |
| **Objectif** | Ce que la sensibilisation devrait accomplir. |
| **Point de contact** | Une étape de la cadence (e-mail, appel téléphonique ou LinkedInMail), planifiée par rapport à l’inscription. |
| **invite de point de contact** | Instructions que l’IA suit lors de la génération de l’objet et du corps d’un e-mail pour un prospect, notamment le ton, la longueur, le focus et le call to action. |
| **Cadence** | La séquence complète des points de contact : combien, dans quel ordre et à quels jours. |
| **Filtre de ciblage** | Une condition qui limite le workflow sortant à un sous-ensemble de prospects. |
| **Brouillon** | Un e-mail généré qui est prêt pour la révision mais pas encore approuvé. |
| **Raisonnement** | L’IA explique comment elle a écrit un e-mail donné, y compris les signaux et les sources de données qu’elle a utilisés. |
| **Inscription** | la validation des brouillons d’un prospect, qui active le rythme et met en file d’attente les e-mails à envoyer pendant la fenêtre d’envoi du workflow sortant ; |

Les sections suivantes expliquent comment créer un workflow sortant, passer en revue les e-mails générés, approuver les prospects et gérer les workflows sortants.

## Création d’un workflow sortant

L’expérience de configuration compacte organise la configuration des workflows autour des objectifs, du ciblage, des points de contact et des paramètres. Utilisez la navigation de section pour vous déplacer entre eux. Après avoir enregistré le workflow, ajoutez les prospects pour générer leurs e-mails.

1. Dans le volet de navigation de gauche, sélectionnez **[!UICONTROL Workflows sortants]**.
1. Dans l’onglet **[!UICONTROL Parcourir]**, sélectionnez **[!UICONTROL + Créer un workflow sortant]** dans le coin supérieur droit.

Les administrateurs peuvent affecter le workflow sortant à un coéquipier plutôt qu’à eux-mêmes. Avant de lancer le workflow, sélectionnez **[!UICONTROL Affecter un utilisateur]** dans la liste déroulante et choisissez votre coéquipier.

### Définir votre objectif {#step-1-define-your-goal}

L’objectif définit le résultat prévu et guide le ciblage, la cadence et la génération d’e-mails.

1. Pour créer votre propre objectif, sélectionnez **[!UICONTROL Démarrer à partir de zéro]** ou, pour utiliser un modèle enregistré, sélectionnez **[!UICONTROL Démarrer à partir d’un modèle]**.

1. Sélectionnez l’un des **[!UICONTROL Objectifs recommandés]** correspondant à votre entreprise. Chaque recommandation comprend une brève explication de sa pertinence. Pour renseigner l’objectif, sélectionnez une recommandation. Pour parcourir l’ensemble complet des recommandations, sélectionnez **[!UICONTROL Afficher tout]** ou saisissez votre propre objectif. Vous pouvez également choisir dans la liste **[!UICONTROL Objectifs populaires]**.
1. Continuez vers le ciblage.

Indiquez un résultat spécifique dans l’objectif. Par exemple, saisissez `Book a 15-minute discovery call with marketing leaders evaluating campaign automation` au lieu de `Promote campaign automation`.

L’IA conserve les exigences de l’objectif exactement dans les points de contact générés. Insérez des phrases exactes, les lignes d’ouverture ou de fermeture requises, les sessions et les dates nommées ou une structure spécifique lorsque le contenu généré doit les conserver.

### Configuration des filtres de ciblage {#step-2-configure-targeting-filters}

Les filtres de ciblage définissent les prospects éligibles. Lorsque vous ajoutez des prospects ultérieurement, seuls ceux qui correspondent à ces filtres apparaissent dans la liste de sélection.

![&#x200B; Filtres de ciblage &#x200B;](assets/create-workflow-targeting.png){width="800" zoomable="yes"}

Décrivez votre prospect idéal en langage naturel. Par exemple, saisissez `Hot leads at companies with 500 or more employees who requested a demo`. [!DNL Adobe Marketo Qualifier] convertit la description en critères de ciblage que vous pouvez examiner et affiner.

1. Pour ouvrir la liste **[!UICONTROL Ajouter un filtre]**, sélectionnez la flèche vers le bas, puis un filtre.

1. Définissez des valeurs pour le filtre.
1. Ajoutez d’autres filtres si vous devez limiter l’audience.

1. Accédez aux points de contact.

Le ciblage peut utiliser le type d’activité, le score, l’évaluation et d’autres attributs disponibles. Combinez des critères avec [!DNL AND] ou [!DNL OR] et utilisez des opérateurs tels que égal à, contient, supérieur à, inférieur à et entre.

Pour Salesforce et Microsoft Dynamics 365, le ciblage peut également combiner les champs de compte, de contact et d’opportunité qu’un administrateur rend filtrables dans le [mappage entrant](integrations.md#map-crm-fields-inbound-mapping). Par exemple, combinez le rôle d’un contact avec le secteur de son compte associé et l’étape d’une opportunité de cibler les bons contacts.

### Inscrire automatiquement les prospects aux activités marketing

Un workflow sortant peut évaluer l’activité des points forts marketing en direct par rapport à ses critères de ciblage. Lorsque l’activité correspond, [!DNL Marketo Qualifier] résout le propriétaire du CRM du prospect par e-mail et l’inscrit uniquement dans un workflow éligible qui appartient à ce représentant.

L’inscription automatique suit cette séquence :

1. Un représentant définit les critères de ciblage du workflow.
1. L’activité Live [!DNL Marketo] arrive pour un prospect.
1. [!DNL Marketo Qualifier] résout le propriétaire du prospect à partir de Salesforce ou Microsoft Dynamics et évalue l’activité par rapport aux workflows éligibles du propriétaire.
1. Lorsque les critères correspondent, le prospect est inscrit et la diffusion commence.

Si un autre représentant contacte déjà le prospect, [!DNL Marketo Qualifier] affiche un avertissement avant le début de la diffusion en double.

### Configurer les points de contact {#step-3-generate-and-review-touchpoints}

Une fois le ciblage configuré, l’IA analyse l’objectif et les critères de ciblage, définit la cadence et écrit une invite pour chaque point de contact. Le rythme peut inclure des étapes d’e-mail, d’appel téléphonique et LinkedInMail.

Les points de contact utilisent une disposition de séquence qui facilite l’analyse de l’ordre des étapes.

![Points de contact](assets/create-workflow-touchpoints.png){width="800" zoomable="yes"}

Pour lire son invite, développez un point de contact d’e-mail. L’invite guide l’IA lorsqu’elle écrit l’e-mail de chaque prospect, y compris le ton, la longueur, le focus et le call to action.

La saisie d’une barre oblique `/` affiche la liste des jetons définis que vous pouvez utiliser pour personnaliser l’e-mail.

#### Régénérer la cadence

Si la cadence ne vous convient pas, sélectionnez **[!UICONTROL Régénérer]** et saisissez une instruction d’affinement. Par exemple :

* `Use three touchpoints across two weeks`
* `Lead with an executive briefing offer in the first email`
* `Add a nurture touch focused on a relevant case study`

L’IA réécrit la cadence complète en fonction de vos instructions. Pour ajuster un point de contact d’e-mail, modifiez son invite au lieu de générer à nouveau la cadence entière.

Définissez un délai du point de contact en jours, heures et minutes. Définissez les jours, heures et minutes à `0` pour envoyer le point de contact sans attendre après l’inscription ou l’achèvement du point de contact précédent. Utilisez un délai plus long pour espacer les points de contact ultérieurs au cours de la cadence.

#### Utiliser le Centre de connaissances dans les invites

Si votre entreprise a créé un playbook [Centre de connaissances](admin-settings.md#knowledge-center), reportez-vous à celui-ci dans l’invite. Nommez le document et décrivez le contexte à utiliser. Par exemple, saisissez `Use the ABC positioning guide from the Knowledge Center and focus on the security value proposition`.

Lorsque la cadence et les invites sont prêtes, passez aux paramètres.

Affinez les invites de point de contact avant de générer les e-mails de prospect. L’IA utilise ces invites pour chaque prospect sélectionné.

### Configurer les paramètres du workflow sortant {#step-4-configure-outbound-workflow-settings}

La section **[!UICONTROL Paramètres]** contrôle le fonctionnement du workflow sortant.

![&#x200B; Panneau Paramètres &#x200B;](assets/create-workflow-settings.png){width="800" zoomable="yes"}

1. Vérifiez le **[!UICONTROL nom du workflow sortant]** et modifiez-le si nécessaire.
1. Dans **[!UICONTROL Nombre maximal de prospects par workflow sortant]**, confirmez le nombre maximal de prospects que le workflow sortant peut gérer en même temps.
1. Définissez la **[!UICONTROL fenêtre d’envoi]** pour les heures pendant lesquelles les e-mails sortants sont autorisés à être envoyés.
1. Sélectionnez les jours de la semaine où les e-mails peuvent être envoyés. Pour éviter les envois de week-end, sélectionnez uniquement les jours de la semaine au lieu d’utiliser un paramètre **[!UICONTROL Ignorer les week-ends]** distinct.
1. Choisissez si vous souhaitez envoyer pendant les heures les plus actives de chaque prospect.
1. Pour arrêter automatiquement les points de contact de suivi une fois qu’un prospect a réservé une réunion, activez **[!UICONTROL Pause de la réservation de réunion]**.
1. Choisissez d’utiliser le fuseau horaire de chaque prospect ou le fuseau horaire du workflow sortant **[!UICONTROL Fuseau horaire]** pour la planification de l’envoi. Si vous utilisez le fuseau horaire du workflow sortant, vérifiez qu’il correspond à votre audience.
1. Sous **[!UICONTROL Autorisations]**, conservez **[!UICONTROL Privé]** (valeur par défaut) ou sélectionnez **[!UICONTROL Partagé avec tout le monde]**. Pour plus d’informations, voir [Partager un workflow sortant](#share-an-outbound-workflow).
1. Sélectionnez **[!UICONTROL Enregistrer et ajouter des prospects]** pour ouvrir la vue de sélection des prospects.

Pour rétablir les valeurs par défaut de la fenêtre d’envoi, du fuseau horaire, des jours, des règles de suivi et d’absence du bureau, de la visibilité et de la cadence des suggestions, activez **[!UICONTROL Réinitialiser aux paramètres par défaut]**. Le nom du workflow sortant reste inchangé.

Un administrateur configure globalement le pied de page d’opt-out, qui s’applique aux e-mails sortants indépendamment des paramètres du workflow sortant. Voir [&#x200B; Configuration du processus d’opt-out global des e-mails](integrations.md#configure-global-email-opt-out).

### Ajouter des prospects et commencer la génération d’e-mails {#step-5-add-prospects-and-start-email-generation}

Après l’enregistrement, ajoutez les prospects à partir de la vue de sélection. Les filtres de ciblage que vous avez configurés sont appliqués.

Vous pouvez également ajouter des prospects à un workflow sortant existant à partir d’une liste [Audience intelligente (Beta)](smart-audience.md#add-leads-to-an-outbound-workflow). Passez en revue les prospects et le workflow sélectionnés avant de confirmer. L’ajout de prospects ne remplace pas les étapes de révision et d’approbation des e-mails décrites ci-dessous.

1. Passez en revue la liste.

   Les lignes comprennent généralement le nom, le compte, l’adresse e-mail, la fonction, le statut d’engagement et le statut du prospect.

1. Ajustez les filtres ici si vous devez développer ou réduire la liste.
1. Sélectionnez des prospects à l’aide des cases à cocher.
1. Pour commencer la génération d’e-mails par prospect, sélectionnez **[!UICONTROL Suivant : vérifier les points de contact]**.

L’IA génère un e-mail personnalisé pour chaque prospect et point de contact d’e-mail sélectionné. Les points de contact Phone et LinkedInMail restent des étapes planifiées. Pour continuer à travailler pendant la génération, sélectionnez **[!UICONTROL Notifier lorsque prêt]**.

Pour chaque prospect, l’IA associe l’invite de point de contact aux données de personne et de compte, à l’historique d’engagement et aux actualités récentes afin de produire une ligne d’objet et un corps.

Les e-mails générés utilisent toutes les données supplémentaires enregistrées sur un prospect, y compris les champs personnalisés [importés avec le prospect](prospects.md#build-your-prospect-list), afin que les brouillons soient plus pertinents. Il n’existe pas de liste fixe de champs pris en charge et les champs nouveaux ou personnalisés fonctionnent sans configuration supplémentaire. L’IA utilise ces données lorsqu’elles sont pertinentes ; si un prospect ne dispose pas de données supplémentaires, la génération d’e-mails fonctionne comme auparavant.

Les e-mails peuvent également être générés dans la langue du prospect, avec des salutations correctes, des expressions naturelles et un ton professionnel approprié. Les langues prises en charge sont le français, l’allemand, l’espagnol, etc.

## Consulter et affiner les e-mails générés

Une fois la génération terminée, la vue détaillée du workflow sortant vous invite à consulter les brouillons. [!DNL Marketo Qualifier] n’envoie pas d’e-mail tant que vous ne l’avez pas approuvé.

Avant qu’un brouillon ne soit examiné, [!DNL Marketo Qualifier] le vérifie par rapport aux directives de qualité. En cas d’échec, le brouillon est réécrit à l’aide de commentaires spécifiques et vérifié à nouveau. Les mêmes directives guident le premier brouillon, de sorte que la plupart des e-mails y répondent lors de la première passe. Ces contrôles permettent de garantir que :

* Le corps de l’e-mail contient uniquement le message pour le prospect, sans notes internes, raisonnement ni références sources.
* Une demande de réunion s’affiche uniquement lorsque votre calendrier est connecté dans [Paramètres de profil](profile-settings.md), qu’un lien de réservation est disponible et que l’invite de point de contact demande une demande de réunion.
* Les listes à puces sont correctement formatées.
* L’e-mail évite les modèles courants qui sonnent à l’IA, notamment les tirets, les listes de trois utilisés pour le rythme, le phrasé « pas seulement X, mais Y » et les clichés surutilisés.

Vous révisez, modifiez et approuvez toujours chaque e-mail avant son envoi. Le raisonnement, les modifications directes et l’**[!UICONTROL génération à l’aide de l’IA]** fonctionnent comme auparavant.

1. Dans la vue détaillée du workflow sortant, sélectionnez **[!UICONTROL Vérifier les brouillons]** dans la bannière.
1. L’étape **[!UICONTROL Vérifier les points de contact]** comporte deux onglets :
   * **[!UICONTROL Prêt pour la révision]** : les e-mails dont la génération est terminée.
   * **[!UICONTROL Génération]** : les e-mails en cours d’écriture.
1. Pour charger les points de contact d’un prospect sur la droite, sélectionnez son nom dans la liste de gauche.
1. Pour développer un point de contact et lire l’objet et le corps complets, utilisez son chevron (**>**).

### Lire le raisonnement de l’IA

Pour chaque e-mail généré, la section **[!UICONTROL REASONING]** explique comment l’IA a conçu ce message, y compris les signaux, les attributs et les sources qui ont façonné le contenu et le call to action. Passez en revue ces informations et validez la personnalisation avant d’approuver.

### Modifier directement les e-mails

Pour les petits changements de libellé ou de ton :

1. Pour ouvrir l’éditeur, sélectionnez l’icône **[!UICONTROL Modifier]** sur le point de contact développé.
1. Modifiez l’objet ou le corps.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

### Affiner les e-mails avec l’IA

Pour les modifications structurelles ou d’accentuation, utilisez **[!UICONTROL Générer avec l’IA]**. L’IA réécrit l’email tout en conservant son contexte de personnalisation.

1. Dans l’éditeur d’email, sélectionnez **[!UICONTROL Générer avec l’IA]**.

1. Saisissez une instruction claire, par exemple :
   * `Make it shorter and more direct. Keep it under 100 words.`
   * `Focus more on the prospect's role and how the solution helps them specifically.`
   * `Change the call-to-action to suggest a 15-minute introductory call instead.`
1. Passez en revue la révision et modifiez-la si nécessaire.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

>[!TIP]
>
>Utiliser des modifications directes du libellé et du ton. Utilisez **[!UICONTROL Générer avec l’IA]** pour réécrire l’e-mail.

## Approuver et inscrire des prospects

La validation active le rythme d’un prospect. Le système n’envoie pas d’e-mails à un prospect tant que vous ne l’avez pas approuvé et inscrit.

1. Dans la liste de gauche des prospects, sélectionnez les prospects dont vous avez vérifié les e-mails et qui sont prêts à envoyer.
1. Sélectionnez **[!UICONTROL Approuver et inscrire les prospects]** dans le coin inférieur droit.

Les e-mails approuvés sont envoyés en fonction des jours sélectionnés du workflow sortant, de la fenêtre d’envoi, de l’option des heures actives et du paramètre de fuseau horaire. Un point de contact à retard nul envoie immédiatement ; un point de contact sur deux suit son retard configuré. Les prospects non approuvés sont toujours dans l’état **[!UICONTROL Prêt pour la révision]**.

## Partage d’un workflow sortant

Chaque workflow sortant comporte un paramètre **[!UICONTROL Autorisations]**. Les workflows sortants sont **[!UICONTROL privés]** par défaut. Pour mettre un workflow sortant à la disposition de l&#39;équipe, le propriétaire peut sélectionner **[!UICONTROL Partagé avec tout le monde]**.

>[!CAUTION]
>
>Le partage est permanent. Une fois qu’un workflow sortant est défini sur **[!UICONTROL Partagé avec tout le monde]**, il ne peut pas être redéfini sur **[!UICONTROL Privé]**.

Sur un workflow sortant partagé, les coéquipiers peuvent inscrire leurs propres prospects. Chaque personne ne peut gérer ou suspendre que les prospects auxquels elle est inscrite, y compris lors de l’utilisation d’actions en masse. Le propriétaire du workflow sortant peut seul modifier les paramètres au niveau du plan, tels que la fenêtre d’envoi et le fuseau horaire. Ces paramètres sont en lecture seule pour les coéquipiers. Pour modifier les points de contact sur un workflow sortant en cours d’exécution, dupliquez-le et modifiez la copie.

Lorsque vous inscrivez des prospects à un workflow sortant partagé, choisissez si l’e-mail est envoyé en tant que propriétaire du workflow ou représentant affecté de chaque prospect.

Utilisez ces filtres pour que les workflows sortants partagés et les résultats restent ciblés :

* Dans **[!UICONTROL Prospects engagés]** et **[!UICONTROL Performances]**, utilisez **[!UICONTROL Inscrit par]** pour filtrer les prospects par la personne qui les a inscrits. Le filtre correspond par défaut aux prospects que vous avez inscrits.
* Sur l’onglet **[!UICONTROL Parcourir]**, utilisez le filtre de partage pour sélectionner **[!UICONTROL Partagé par moi]**, **[!UICONTROL Partagé avec moi]**, **[!UICONTROL Privé]** ou **[!UICONTROL Tout]**.

## Gestion des réponses d’absence du bureau

Lorsqu’un prospect répond avec un message d’absence du bureau, le workflow sortant le gère automatiquement.

* **Reprise automatique** : activé par défaut. Si la réponse d’absence du bureau comprend une date de retour, le workflow sortant reprend le rythme à cette date. Si aucune date de retour n’est indiquée, le workflow sortant reprend après une mémoire tampon de reprise que votre équipe peut configurer.
* **Options manuelles** : un rep peut toujours sélectionner **[!UICONTROL Reprendre maintenant]** ou planifier une date de reprise spécifique. Voir [&#x200B; Gestion des workflows sortants existants &#x200B;](#manage-existing-outbound-workflows).

### Demandes d’opt-out dans les réponses

Lorsqu’un prospect répond avec une demande claire de cesser de recevoir des e-mails, comme « veuillez arrêter de m’envoyer des e-mails », « désabonnez-vous », « supprimez-moi de cette liste » ou « retirez-moi de votre liste », [!DNL Marketo Qualifier] marque automatiquement le prospect comme étant désabonné. Il s’agit du même statut et du même badge **[!UICONTROL Opt-out]** que celui utilisé pour sélectionner le lien d’opt-out. Aucun autre point de contact n’est envoyé. Toute mise à jour du statut du CRM configuré fonctionne comme pour un lien d’opt-out.

Seules les requêtes claires sont comptabilisées. Par exemple, la mention « Je ne suis pas la bonne personne » ou « Pas en ce moment » est traitée comme n’importe quelle autre réponse, et non comme un droit d’opposition. Aucune configuration n’est nécessaire ; les désinscriptions en réponse fonctionnent avec le lien d’exclusion configuré dans [Paramètres d’administration](admin-settings.md#configure-global-email-opt-out).

## Dupliquer un workflow sortant

Vous pouvez dupliquer un workflow sortant que vous avez créé ou qui est partagé avec vous. Dupliquez-le à partir de la liste des workflows sortants de l’onglet **[!UICONTROL Parcourir]** ou à partir de la vue détaillée du workflow.

La copie comprend l’objectif, le ciblage, les points de contact et les paramètres d’origine, mais pas ses prospects. La copie commence en tant que **[!UICONTROL brouillon]** avec des autorisations **[!UICONTROL privées]** afin que vous puissiez la réviser et la modifier avant de l’ajouter aux prospects ou de la partager. Le workflow d’origine et ses prospects ne sont pas affectés.

Pour modifier les points de contact d’un workflow sortant en cours d’exécution, dupliquez-le et modifiez la copie. Ajoutez des prospects à la copie ; les prospects déjà inscrits à l’original continuent à courir sans interruption. Chaque workflow possède ses propres résultats dans [Performances sortantes](performance.md).

## Gestion des workflows sortants existants

Sur la page **[!UICONTROL Workflows sortants]**, l’onglet **[!UICONTROL Parcourir]** répertorie tous les workflows sortants disponibles. Chaque carte affiche l’objectif, les points de contact configurés et les mesures de performances. Utilisez cette vue pour surveiller les workflows sortants, réviser les brouillons, ajouter des prospects ou dupliquer un workflow.

## Boîte d’envoi d’e-mail

La [boîte d’envoi d’e-mail](email-outbox.md) répertorie les e-mails automatisés envoyés en votre nom et les réponses.

## Réservation de réunion

Lorsque vous connectez votre calendrier, Marketo Qualifier génère un lien de réservation personnel que les prospects peuvent utiliser pour planifier des heures avec vous.

* **Liens de réservation**—Configurez la connexion et la disponibilité de votre calendrier dans [Paramètres du profil](profile-settings.md). Ajoutez le lien de réservation à votre signature d’e-mail afin qu’il apparaisse dans les e-mails sortants.
* **Placement de cadence** : Marketo Qualifier insère votre lien de réservation aux points pertinents d’une cadence. Vous pouvez modifier son emplacement.
* **Pause de la réservation** : lorsqu’un prospect réserve une réunion, **[!UICONTROL Pause de la réservation de la réunion]** arrête les autres suivis. Voir [Étape 4 : Configurer les paramètres de workflow sortant](#step-4-configure-outbound-workflow-settings).

Suivez les résultats de la réservation sur la page [Performances sortantes](performance.md).

## Bonnes pratiques relatives au workflow sortant

* **Définissez un objectif spécifique.** Le ciblage, la cadence et les e-mails dérivent tous de l’objectif . Indiquez le résultat que vous souhaitez que le workflow sortant atteigne.
* **Finalisez les invites de point de contact avant la génération par prospect.** Après la génération en bloc, les modifications sont généralement apportées un prospect à la fois.
* **Utiliser le raisonnement comme contrôle de qualité.** Si le mauvais signal est mis en évidence ou si un signal approprié est manquant, modifiez l’e-mail ou révisez l’invite de point de contact et régénérez la cadence.
* **Faire correspondre l’outil d’édition à la modification.** Utiliser des modifications directes du libellé et du ton. Utilisez **[!UICONTROL Générer avec l’IA]** pour restructurer ou recadrer.
* **Approuver uniquement ce que vous avez révisé.** Développez les points de contact, lisez le contenu et affinez-les si nécessaire avant l’inscription.

>[!MORELIKETHIS]
>
>* [Tâches](tasks.md)
>* [&#x200B; Centre de connaissances &#x200B;](admin-settings.md#knowledge-center)
>* [Performance sortante](performance.md)
