---
title: Vérifier la boîte d’envoi d’e-mail
description: Découvrez comment vérifier les e-mails que Adobe Marketo Qualifier a envoyés en votre nom, y compris les réponses, dans la boîte d’envoi d’e-mails.
feature: Agentic AI, Sales Insights, Account Journeys
role: User
product_v2:
  - id: d98caee2-fd67-486e-9513-36435358ebff
    internal-label: Marketo Qualifier
feature_v2:
  - id: e6e1112f-735e-4244-9aeb-08972bded7e7
    internal-label: Email
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: beb7a3c1-66ab-4786-b879-7621375b3c40
    internal-label: Email marketing
source-git-commit: fcdc5d36cbb1500cf984e1439291aa8dbf17b72b
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%
---

# Boîte d’envoi d’e-mail

Utilisez **[!UICONTROL boîte d’envoi d’e-mail]** pour consulter les e-mails envoyés par les workflows sortants et les réponses. Vous pouvez confirmer l’envoi, lire les réponses dans leur contexte et ouvrir le workflow sortant qui a envoyé un message.

La page comporte deux panneaux : une liste d’e-mails à gauche et une vue de lecture à droite. Faites glisser le séparateur entre eux pour redimensionner la liste.

## Lire la liste d&#39;emails

La liste **[!UICONTROL Tous les e-mails]** contient une ligne pour chaque e-mail envoyé, l&#39;e-mail le plus récent en premier. Chaque ligne affiche le nom du destinataire, l’objet et la date d’envoi. Un e-mail sans objet affiche _(Aucun objet)_. Faites défiler l’écran pour charger les anciens e-mails.

Lorsque vous ouvrez la page, Adobe Marketo Qualifier sélectionne automatiquement le premier e-mail afin que son contenu s’affiche à droite.

Si vous n’avez envoyé aucun e-mail, la liste affiche _Votre boîte d’envoi est vide_. Une fois que vous avez envoyé ou planifié un e-mail par le biais d’un workflow sortant, il apparaît ici.

## Lire un email et ses réponses

Pour ouvrir un e-mail à droite, sélectionnez-le dans la liste. La vue lecture comporte trois parties :

* **Destinataire** : le nom, la fonction et le compte du destinataire, le cas échéant.
* **Objet et workflow sortant** : l’objet, le nom du [workflow sortant](outbound-workflows.md) qui a envoyé l’e-mail et le statut du workflow sortant. Pour ouvrir le workflow sortant, sélectionnez son nom.
* **Conversation** : l&#39;e-mail envoyé et toutes les réponses dans un thread. Chaque entrée identifie si le message a été envoyé ou reçu et inclut un horodatage.

Les e-mails s’affichent tels qu’ils ont été envoyés, y compris le contenu personnalisé. Si le corps d’un message n’est pas disponible, Marketo Qualifier affiche une note courte _Contenu d’e-mail non disponible_ à sa place.

>[!NOTE]
>
>La boîte d’envoi d’e-mail est en lecture seule. Pour suivre un prospect qui a répondu, ouvrez le workflow sortant ou le prospect. Pour consulter les performances des e-mails et des réponses, voir [Performances sortantes](performance.md).

>[!MORELIKETHIS]
>
>* [Workflows sortants](outbound-workflows.md)
>* [Performance sortante](performance.md)
>* [Tâches](tasks.md)
