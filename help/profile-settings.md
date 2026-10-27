---
title: Configurer les paramètres de profil
description: Découvrez comment configurer la connexion par e-mail, la signature et la disponibilité du calendrier dans les paramètres du profil Adobe Marketo Qualifier.
feature: Agentic AI, Sales Insights, Account Journeys
role: User
TQID: 'https://experienceleague.adobe.com/YsrBduYA7jKhgxttexqMBBpgDIq23s6wUb4Wp6y6h3g'
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Marketo Qualifier
feature_v2:
  - id: f8c781b4-253f-436e-b9f1-a71172814e41
    internal-label: Profile Settings
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: beb7a3c1-66ab-4786-b879-7621375b3c40
    internal-label: Email marketing
source-git-commit: ab54d20ccc80d88c3592d89c9f43feeb062ed82c
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%
---

# Paramètres de profil

Dans le volet de navigation de gauche, développez **[!UICONTROL Configuration]** et sélectionnez **[!UICONTROL Paramètres de profil]**. Utilisez ces paramètres pour gérer vos informations personnelles, la connexion par e-mail, le calendrier et la disponibilité du chat.

![Paramètres de profil](assets/profile-email-config.png)

## Paramètres d’e-mail

Dans l’onglet **[!UICONTROL Paramètres de messagerie]**, configurez vos connexions par e-mail.

* **[!UICONTROL Connexions par e-mail]** — Sélectionnez Microsoft Outlook ou Google et suivez le processus de connexion. Voir [Connexion à Outlook](integrations.md#connect-outlook) pour connaître l&#39;accès que vous approuvez et le chemin d&#39;approbation de l&#39;administrateur, le cas échéant.
* **[!UICONTROL Signature d&#39;email]** — Ajoutez ou mettez à jour la signature utilisée dans les emails générés. Incluez votre lien [réservation de réunion](outbound-workflows.md#meeting-booking) afin que les prospects puissent planifier du temps avec vous.
* **[!UICONTROL Lien de réservation de réunion]** - Envoyez une invitation à une réunion dans vos e-mails. Prend l&#39;URL de la réunion.

### Contexte de rédaction des emails

![Contexte des emails](assets/profile-email-instructions.png)

Utilisez **[!UICONTROL contexte de rédaction des e-mails]** pour définir le ton, la structure et le style des e-mails, afin que ceux-ci soient cohérents.

Écrivez votre contexte en Markdown simple dans la zone **[!UICONTROL Contexte de rédaction d’e-mail]**.
Utilisez-la pour définir :

* Ton et voix
* Structure et longueur
* Personalization et règles de salutations
* Style de la ligne d&#39;objet
* Utilisation des signaux d’engagement
* comment les mesures, les points de BAT et les témoignages de clients sont encadrés ;

Par défaut, les brouillons utilisent un contexte de style maison, de sorte que les brouillons existants ne changent pas tant que vous n’avez pas ajouté votre propre contexte.

## Configuration du calendrier

Définissez votre fuseau horaire et votre disponibilité dans l’onglet **[!UICONTROL Configuration du calendrier]**.

* **[!UICONTROL Connexion au calendrier]**—Sélectionnez **[!UICONTROL Connexion]** et suivez le processus de connexion à Microsoft.
* **[!UICONTROL E-mail de confirmation de réunion]**—Définissez l&#39;objet et le corps de l&#39;e-mail de confirmation qu&#39;un prospect reçoit après avoir réservé une réunion.
* **[!UICONTROL Préférences]** : définissez la durée de réunion par défaut et la marge entre les réunions.

Si vous déconnectez votre calendrier :

* Les liens de réservation actifs ne fonctionnent plus.
* La page de réservation affiche un message d’indisponibilité temporaire.
* Vos paramètres sont conservés lorsque vous vous reconnectez.

## Disponibilité du calendrier

La disponibilité de votre calendrier dans Adobe Marketo Qualifier repose sur deux entrées :

* Votre calendrier professionnel connecté, tel qu’Outlook ou Gmail
* Les règles de disponibilité et de créneau horaire dans **[!UICONTROL configuration du calendrier]**

Marketo Qualifier lit le statut de disponibilité, et non les détails de l’événement, à partir du calendrier connecté. Il associe ce statut à vos règles afin de déterminer les créneaux horaires que les prospects peuvent réserver.

Vous pouvez configurer les éléments suivants :

* Heures de travail par jour de la semaine
* Plusieurs blocs par jour, par exemple, de 9 h à midi et de 13 h à 17 h.
* Votre fuseau horaire
* Durée de la réunion
* Mettre en mémoire tampon avant et après les réunions
* Avis minimal
* Fenêtre de réservation

>[!MORELIKETHIS]
>
>* [Workflows sortants](outbound-workflows.md)
>* [Intégrations](integrations.md)
>* [Tâches](tasks.md)
