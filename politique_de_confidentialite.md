# Politique de confidentialité — MyBot

**Date d'entrée en vigueur : 20/10/2026 — mise à jour : 22/10/2026**

MyBot est un robot Discord d'administration et de modération de serveurs. Cette
politique explique quelles données MyBot collecte via l'API Discord, pourquoi,
combien de temps, et comment les faire supprimer.

> Conformément aux Conditions d'utilisation des développeurs de Discord :
> MyBot ne vend, ne partage et ne réutilise AUCUNE donnée à des fins
> publicitaires ou d'entraînement d'IA, et fournit des moyens simples de
> supprimer ou d'exporter tes données.

## 1. Données collectées

MyBot ne stocke le **texte des messages** que dans UN seul cas, désactivé
par défaut : les sauvegardes « Messages des salons » de `/backup`
(option Premium d'un serveur, actée par ses administrateurs), limitées
aux 80 derniers messages de 40 salons textuels maximum. Ces snapshots
sont supprimés quand le bot quitte le serveur, et les messages d'un
membre peuvent être retirés à tout moment via `/confidentialite`. Tout
le reste ne conserve que des données nécessaires aux fonctionnalités
activées par les administrateurs du serveur, par système :

| Système | Données conservées |
|---|---|
| Niveaux / XP | Points d'XP par membre, paliers atteints (si activé par le serveur) |
| Invitations | Compteurs d'invitations par membre (qui a invité qui, sans lien cliquable) |
| Prise de service | Temps de service cumulé et statut (en service / hors service) du staff |
| Absences | Demandes d'absence (dates, motif, statut, décision) |
| Avis / évaluations | Notes et commentaires laissés sur les membres du staff |
| Tickets | Métadonnées des tickets (créateur, priorité, assignation) ; le contenu des conversations, quand il est historisé, reste sur Discord (salon de logs du serveur) |
| Événements / giveaways / sondages | Listes de participants et résultats |
| Règlement | Liste des membres ayant accepté le règlement |
| Anti-Raid / modération | Score de menace, alertes, historique d'actions effectuées par le bot (IDs impliqués) |
| Sauvegardes serveur (Premium) | Copie de la structure du serveur (rôles, salons, permissions) ; option « Messages des salons » : 80 derniers messages par salon textuel (texte + auteur + pièce jointe si volontairement activé par les administrateurs) |
| Sécurité | Liste blanche (whitelist) des utilisateurs autorisés par le propriétaire |
| Sanctions transverses de l'Équipe | Historique des modérations transverses effectuées par l'équipe du bot (anti évitement de sanction) — voir exception en § 4 |
| Journal technique (smartlog) | Journal d'erreurs et d'actions du bot (limité à 300 entrées, sans contenu de message) |

Les identifiants suivants peuvent être traités : ID utilisateur, ID serveur,
ID de salon, ID de message (référence technique). Les pseudos/avatars affichés
proviennent de Discord et ne sont pas copiés de façon permanente.

## 2. Localisation des logs de modération

MyBot peut afficher dans un salon de logs configuré **par le serveur** des
informations sensibles lors d'événements de modération (message supprimé ou
modifié, arrivée/départ, invitation...). Ces exigences de logs sont activées
uniquement par les administrateurs du serveur : l'ajout du bot sur un serveur
par ses administrateurs vaut acceptation de ce mode de fonctionnement pour
celui-ci.

- Les logs sont envoyés **dans le serveur lui-même** (salon Discord).
- Les extensions anti-raid ne lisent le contenu des messages que **pendant
  l'exécution** (détection de spam/lien/mots interdits) et ne l'écrivent
  jamais dans des fichiers.
- Les alertes de raid / SOS peuvent être transmises au salon d'assistance du
  bot pour la prise en charge du staff du serveur concerné (envoi d'IDs +
  extraits courts, sans historique complet).

## 3. Durée de conservation

- Les données d'un serveur sont conservées **tant que le bot est présent sur
  le serveur**.
- **Quand le bot est retiré d'un serveur, TOUTES les données de ce serveur
  sont automatiquement supprimées** dans un délai raisonnable (purge
  automatique à la sortie du serveur, sauvegardes serveur comprises).
- Le journal technique est écrêté automatiquement à 300 entrées.

## 4. Tes droits

À tout moment tu peux :

1. **Exporter tes données** : commande `/confidentialite` → bouton « Exporter
   mes données » (fichier JSON envoyé uniquement à toi, en DM du bot).
2. **Supprimer tes données** :
   - dans le serveur où le bot est présent : `/confidentialite` → « Supprimer
     dans ce serveur » ;
   - sur **tous les serveurs** : `/confidentialite` → « Supprimer partout » ;
   - les administrateurs du serveur peuvent aussi demander une purge complète
     du serveur via le contact ci-dessous.
3. La suppression est immédiate et irréversible (les données sont retirées
   des fichiers du bot). Elle retire aussi tes messages des sauvegardes
   serveur.

**Note** : la suppression sur *tous* les serveurs d'un coup est une action
d'administration réservée à l'équipe du bot. Pour toi, le chemin complet
reste : exécute `/confidentialite` sur chaque serveur où le bot est présent
et supprime tes données serveur par serveur — c'est la voie accessible à
tous, sans restriction.

Exception : les données de sanction ou d'historique de modération
maintenu par l'équipe du bot (liste noire de sécurité, historique
transverse anti-évitement-de-sanction) ne sont pas supprimables par la
commande, pour ne pas permettre le contournement de sanctions. Tu peux
les contester via le contact ci-dessous.

## 5. Sécurité

- Les données sont stockées sur un hébergement isolé, accessibles uniquement
  via des identifiants sécurisés.
- Les écritures sont **atomiques et journalisées** : un crash ne corrompt pas
  les données. Aucune donnée n'est chiffrée à l'intérieur des fichiers, mais
  aucune n'est non plus diffusée ; le bot ne communique qu'avec l'API Discord.
- En cas d'accès non autorisé avéré aux données, les utilisateurs concernés
  et Discord seront informés conformément au Contrat développeur.

## 6. Tiers

- Le bot est hébergé sur **bot-hosting.cloud** (héberge du code, expose le
  stockage fichier local).
- Aucune autre partie ne reçoit de données de Discord via MyBot.
- Aucune donnée n'est revendue, cédée ou utilisée à des fins publicitaires.

## 7. Contact

Pour toute demande (suppression, modification, question) :

- **Serveur d'assistance** : 👉 COLLE ICI TON LIEN D'INVITATION
- **Email** : 👉 COLLE ICI TON EMAIL

## 8. Respect des conditions

Cette politique est maintenue conformément aux :
- Conditions d'utilisation des développeurs (Developer Terms of Service),
- Politique développeur (Developer Policy),
- Conditions d'utilisation de Discord.

Toute modification de cette politique est appliquée à partir de la date
indiquée en tête de document.
