# CLAUDE.md — quick-lab

## À quoi sert ce dépôt
Ce n'est pas un projet de code. C'est un **espace de travail pour des actions rapides** :
- tester ou analyser un outil, un logiciel ou un dépôt GitHub trouvé sur Internet ;
- vérifier un lien et dire si c'est fonctionnel, utile ou risqué ;
- répondre à des questions ponctuelles ou faire de petites expériences jetables.

L'utilisateur envoie un lien ou une question. Claude analyse, teste si possible, puis rend compte en français.

## Règles de travail
1. **Ne jamais mettre le code d'un dépôt externe dans ce dépôt.** On le clone dans le dossier scratchpad de la session (temporaire). Ici, on garde seulement nos notes.
2. **Documenter chaque action dans `architecture/`** (obligatoire) :
   - créer une fiche `architecture/AAAA-MM-JJ-nom-court.md` à partir de `architecture/_modele.md` ;
   - ajouter une ligne dans `architecture/HISTORIQUE.md` (le tableau qui sert d'index) ;
   - si une suite est prévue, l'ajouter dans `architecture/A-FAIRE.md` (le cahier des charges).
3. Faire un commit puis pousser sur `main` à la fin de chaque action.
4. Rester honnête sur les limites : pas de GPU dans le conteneur, réseau filtré par proxy, pas d'accès au matériel de l'utilisateur.
5. Ne pas lancer d'outil destructeur, malveillant ou qui retire des protections. L'analyser et l'expliquer reste possible.

## Environnement habituel
Conteneur Linux éphémère : 4 cœurs, environ 15 Go de RAM, pas de GPU.
Disponibles : Python (`uv`), Node, git, Chromium/Playwright.
