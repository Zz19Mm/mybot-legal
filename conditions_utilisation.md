# Conditions d'utilisation — MyBot

**Dernière mise à jour : 22/10/2026**

Ces conditions encadrent l'utilisation de **MyBot**, un robot Discord
d'administration et de modération, exploité par son propriétaire
(ci-après « l'Équipe »). En ajoutant MyBot à un serveur Discord ou en
l'utilisant, tu acceptes ces conditions et la
[Politique de confidentialité](politique_de_confidentialite.md).

MyBot opère conformément aux Conditions d'utilisation de Discord, aux
Conditions d'utilisation des développeurs (Developer ToS) et à la
Politique développeur (Developer Policy).

## 1. Commandes — slash `/` ET préfixe `=`

MyBot utilise deux systèmes de commandes, tous deux documentés :

**Commandes slash `/`** (publiques ou réservées) — visibles à tout moment
dans Discord via la liste des commandes du bot : `/help`, `/config`,
`/confidentialite`, `/securite`, `/sos`, `/suggestion`, `/sauvegardes`,
`/whitelist`, `/owner`, etc.

**Commandes préfixe `=`** (toutes réservées à l'Équipe, jamais aux
membres) — elles servent à l'exploitation technique du bot et ne sont
pas accessibles au public. Liste exhaustive :

| Commande | Usage |
|---|---|
| `=help` | Aide des commandes préfixe (Équipe uniquement) |
| `=owner list / acces / role / premium` | Administration des serveurs et du Premium |
| `=servers` / `=leave <id>` | Liste des serveurs du bot / départ du bot d'un serveur |
| `=ban`, `=kick`, `=clear`, `=supprimer-role` | Modération transverse (voir les règles en § 4) |
| `=information <@membre>`, `=history <@membre>` | Consultation, blacklist et historique de sanctions |
| `=blacklist` / `=unblacklist` | Liste noire de l'Équipe (membres interdits du bot) |

Les commandes préfixe ne laissent pas de message apparent (le message
d'invocation est supprimé) mais **toutes** sont tracées dans le journal
technique du bot et, quand cela s'applique, dans l'historique du serveur
ou de l'utilisateur concerné.

## 2. Ce que fait le bot

MyBot fournit aux serveurs Discord des outils configurables par leurs
administrateurs : rôles automatiques, règlement, tickets, niveaux,
événements/giveaways, suggestions, invitations, statistiques d'activité,
protections anti-raid, journaux de modération, sauvegardes/restauration
de configuration de serveur. Toutes les fonctionnalités « système » sont
activées ou désactivées par les administrateurs du serveur via `/config`.

## 3. De qui relève la responsabilité

- **Les administrateurs du serveur** sont responsables de la
  configuration installée et de la modération exercée via les
  fonctionnalités du serveur. L'ajout du bot par leurs invitations vaut
  acceptation de ces conditions pour le serveur.
- **L'Équipe** reste responsable des commandes préfixe (§ 1) et du bon
  fonctionnement technique du bot.

## 4. Modération transverse et règles anti-abus

Les commandes transverses de l'Équipe (`=ban`, `=kick`, `=clear`,
`=supprimer-role`, historique de sanctions transverses) existent pour
lutter contre les personnes ignorant les sanctions (évitement de
sanction) et les abus visant le bot lui-même. Leur usage est strictement
encadré :

1. **Aucun avantage** : une personne utilisant le bot ne peut jamais
   agir sur un rôle ou un membre placé AUSSI HAUT ou PLUS HAUT
   qu'elle-même dans la hiérarchie du serveur concerné — le bot le
   refuse techniquement, même à l'Équipe.
2. Les actions sur le propriétaire d'un serveur ou sur le bot lui-même
   sont techniquement impossibles.
3. Chaque action transverse est historisée et peut être contestée via
   le contact (§ 7).
4. La liste noire de l'Équipe est conservée indépendamment des données
   de serveur, uniquement dans un but de sécurité (cf. Politique de
   confidentialité, exception des sanctions).

## 5. Premium (abonnements)

- **Premium Serveur** : avantages configurables à l'échelle d'un serveur
  (limites étendues, statistiques avancées, `/securite`, sauvegardes
  « Messages des salons »).
- **Premium Personne** : avantage attaché à une personne sur le serveur
  d'assistance du bot (rôle de soutien, tickets de support prioritaires).
- Le Premium est activé ou retiré par l'Équipe (par exemple en cas
  d'abus), sans suppression des données du serveur. Aucun paiement n'est
  traité par le bot lui-même.

## 6. Données et confidentialité

Le traitement des données personnelles est décrit en détail dans la
**Politique de confidentialité** : données collectées, durée de
conservation, export `/confidentialite`, suppression `/confidentialite`
(dans le serveur / sur tous les serveurs) et purge automatique complète
quand le bot quitte un serveur — les sauvegardes serveur y compris.

## 7. Contact

- **Serveur d'assistance** : https://discord.gg/TuYD2kTkg3

## 8. Interruption et résiliation

L'Équipe peut retirer le bot d'un serveur qui viole ces conditions ou
les conditions de Discord, suspendre l'accès d'une personne (liste
noire) ou d'un serveur (Premium), sans préavis. Un serveur peut retirer
le bot à tout moment : toutes ses données sont alors supprimées
automatiquement.

## 9. Modifications

Ces conditions peuvent évoluer ; la version en vigueur est celle jointe
par le bot via `/confidentialite` → bouton « Documents », et datée en
tête de document.
