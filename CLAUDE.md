# Chatons-Atelier

**Dossier de création de Chatons : scénarios, scènes et fiches en JSON, écrits par des agents puis récupérés dans l'appli par le MJ. Vérification : `npm run verifier` depuis le dépôt Chatons. Branche unique `main`, poussée sur `github.com/Laox23/Chatons-Atelier`.**

Chatons est l'outil d'un MJ débutant pour le jeu de rôle *Donjons et Chatons* (dépôt `github.com/Laox23/Chatons`, cloné sur le poste). Ce dossier est son « dossier de création » : Chatons l'écrit (Envoyer vers le dossier), l'agent le modifie, le MJ le relit et le récupère (Récupérer du dossier).

## À lire avant d'écrire

Dans cet ordre, à chaque session :

1. `chatons/format.md` : le format des fichiers et ce que l'agent peut faire dans ce dossier (§ Le dossier de création). Il fait foi.
2. `lore.md` : le monde, le ton, les joueuses, ce qui est interdit.
3. `regles/` et `cartes/` : les règles du jeu et les cartes (enfance, miagie, talents). Un test, une querelle ou un sort suit ces règles, sans en inventer.
4. `bibliotheque/` : les PNJ, lieux, factions, objets et le lexique existants.
5. Les scénarios précédents de la même saga (`sagas/<saga>/`, dans l'ordre de `ordre`) et, s'il y en a, `campagnes/` : ce qui s'est vraiment joué. `campagnes/` se lit seulement.

`chatons/` est régénéré par `npm run atelier -- <ce dossier>` depuis le dépôt Chatons : ne pas le modifier. Il est hors git.

## Règles d'écriture

- **Réutiliser avant de créer.** Un PNJ, lieu, faction, objet ou mot qui existe dans `bibliotheque/` se cite par son `id`, jamais en double. Une fiche neuve n'est créée que si rien n'existe, avec un `id` qui porte sa nature en tête (`pnj-renard`, `lieu-moulin`).
- **Rester fidèle aux fiches.** Un PNJ garde son rôle, son attitude, ses qualités et sa voix. Changer une fiche existante est une décision du MJ : la proposer, ne pas l'écrire.
- **Continuité.** Un scénario part de là où la saga s'est arrêtée : faits posés (#faits), PNJ rencontrés, lieux visités.
- **Ne pas toucher aux `id`** d'un élément modifié.
- Le ton, les limites et le public sont dans `lore.md` ; en cas de doute, le plus doux et le plus clair, sans trop simplifier : il faut garder de l'intérêt. Réglage à ajuster après les premières parties.

## Avant de dire « fini »

1. Depuis le dépôt Chatons : `npm run verifier -- <chemin vers le dossier du scénario>`.
2. Corriger jusqu'à « Aucune erreur », avertissements compris (un #fait en condition que rien ne pose).
3. Relire le scénario contre `lore.md` § Limites.
4. Dire au MJ ce qui a changé : scénarios, scènes, fiches neuves, fiches modifiées.

Le MJ fait « Récupérer du dossier » dans Chatons, puis commit.
