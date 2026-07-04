# 🛡️ MONACO — Guide d'Utilisation et de Configuration du Serveur

Bienvenue sur le guide officiel de **Monaco (v1.1.10)**, votre système de sécurité et de protection autonome. Ce document est conçu pour vous aider à installer le bot sur votre serveur, comprendre le fonctionnement de chaque module et configurer vos protections en toute simplicité.

---

## 🚀 Première Installation (Mise en route)

Pour lancer la protection de Monaco sur votre serveur, suivez ces deux étapes simples :

### 1. Initialisation (`/setup`)
Dès que le bot rejoint votre serveur, la toute première action à faire est de taper la commande suivante dans n'importe quel salon :
/setup

> ⚠️ **Sécurité :** Cette commande ne peut être exécutée **qu'une seule fois**. Si votre serveur est déjà configuré et protégé, le bot bloquera la commande et affichera un message d'erreur rouge vous invitant à utiliser la commande des réglages.

### 2. Accéder aux Réglages (`/settings`)
Pour activer, désactiver ou modifier les options des différents modules de sécurité, utilisez la commande :
/settings

Cette commande ouvre un panneau de contrôle interactif avec des boutons et des menus déroulants pour piloter le bot directement depuis Discord.

---

## 📊 Tableau des Modules Configurables (`/settings`)

Utilisez le tableau ci-dessous pour comprendre le rôle de chaque système de sécurité que vous pouvez ajuster :

| Nom du Système | À quoi sert-il ? | Comportement par défaut |
| :--- | :--- | :--- |
| **🛡️ Anti-JointSpam** | Détecte et bloque les raids (arrivées massives et simultanées de faux comptes). | Active un mode de confinement automatique si trop de comptes rejoignent en même temps. |
| **🔞 Anti-AgeGate** | Empêche les comptes Discord trop récents de nuire sur votre serveur. | Place en quarantaine ou expulse les profils créés il y a moins de X jours. |
| **🤖 Captcha Évolué** | Force les nouveaux arrivants à valider un code visuel pour prouver qu'ils ne sont pas des robots. | Crée les rôles automatiquement et isole l'utilisateur jusqu'à sa validation. |
| **💬 Anti-Spam & Mentions** | Bloque les utilisateurs qui envoient trop de messages ou qui mentionnent trop de personnes en peu de temps. | Applique une restriction de parole temporaire (Timeout) automatique. |
| **🚨 Staff Suspect (Anti-Nuke)** | Surveille les modérateurs et administrateurs pour éviter qu'un compte de staff piraté ne détruise le serveur. | Verrouille instantanément les actions si un modérateur supprime trop de salons/rôles d'affilée. |

---

## 🛡️ Les Sécurités Natives (Toujours Actives)

Ces systèmes sont intégrés d'office dans l'intelligence du bot. **Vous n'avez rien à activer**, ils fonctionnent en tâche de fond 24h/24 pour protéger vos membres :

* **Analyse Anti-Token :** Détecte et neutralise immédiatement les faux comptes qui publient 1 mention et 4 images dans plusieurs salons d'affilée (publicités de faux serveurs, arnaques crypto). Le message est supprimé et l'utilisateur est exclu temporairement 10 minutes.
* **Scan d'Images Inappropriées :** Analyse automatique des images envoyées. Les images à caractère sexuel ou choquant sont supprimées sur-le-champ.
* **Filtre de Mots Interdits :** Censure stricte et intelligente des insultes graves et des tentatives de chantage ou d'intimidation (bloque aussi les contournements comme les écritures avec des points ou des tirets).
* **Anti-Homoglyphes :** Empêche les utilisateurs de tricher sur leur pseudonyme en utilisant des lettres invisibles ou des alphabets étrangers imitant des lettres normales.

---

## ⚖️ L'Échelle des Sanctions Automatiques

Lorsqu'un utilisateur enfreint les règles de sécurité automatiques (messages supprimés pour insultes ou images interdites), Monaco applique une punition graduelle :

| Nombre d'infractions cumulées | Sanction Automatique |
| :---: | :--- |
| **5 messages supprimés** | ⏳ Exclusion temporaire (Mute) de **10 minutes** |
| **10 messages supprimés** | ⏳ Exclusion temporaire (Mute) de **30 minutes** |
| **15 messages supprimés** | ⏳ Exclusion temporaire (Mute) de **1 heure** |
| _Au-delà de 15_ | ⏳ **+1 heure** toutes les 5 nouvelles infractions. |

---

## 🗄️ Le Système de Sauvegarde Intégrale

Monaco intègre un système de secours ultra-performant pour protéger la structure de votre communauté.

1. **Sauvegarde Manuelle :** Les administrateurs peuvent taper `/save` pour enregistrer l'état actuel du serveur.
2. **Sauvegarde Automatique :** Chaque soir à **00h00**, Monaco effectue une sauvegarde complète (salons textuels, vocaux, catégories, rôles, émojis et options du serveur).
3. **Restauration d'urgence :** En cas de problème majeur, les responsables de la sécurité peuvent cloner et réinjecter toute la structure sauvegardée instantanément sur un serveur de secours.

---

## 👤 Fonctionnalité Membre : Signaler un message

Chaque membre de votre serveur peut aider à la modération grâce au bouton de signalement Monaco :
1. Faites un clic droit (ou appuyez sur les **...**) sur un message suspect.
2. Allez dans l'onglet **Applications**.
3. Cliquez sur **Monaco — Signaler le message**.

Le bot va alors analyser instantanément et de manière approfondie le texte et les fichiers pour décider s'il doit supprimer le contenu et sanctionner l'auteur.

---
<p align="center">⚙️ Monaco - Cramponeur — Protection Autonome de Communauté</p>
