# Gemini Skills Brainstorm

Un espace personnel pour noter, organiser et faire mûrir des idées de skills destinés à m’aider pendant le développement, en particulier avec [Gemini CLI](https://github.com/google-gemini/gemini-cli).

Ce dépôt s’inspire de [mattpocock/skills](https://github.com/mattpocock/skills) : des consignes ciblées, réutilisables et faciles à adapter au fil du travail. Ici, les idées pourront venir de conversations avec différentes IA, puis évoluer vers des exemples concrets.

## Organisation

```text
.
├── ideas/       # Notes brutes et pistes à explorer
├── skills/      # Skills en cours ou prêts à l’emploi
│   └── gemini/  # Skills pensés pour Gemini CLI
└── examples/   # Exemples d’utilisation et de résultats
```

Le contenu est volontairement léger : une idée peut commencer comme une note dans `ideas/`, puis être déplacée ou développée dans `skills/` quand elle devient assez claire. Les exemples associés peuvent aller dans `examples/`.

## Ajouter une idée

Crée un fichier Markdown dans `ideas/` avec le problème à résoudre, le contexte où il se présente et le comportement souhaité de l’IA. Pas besoin de suivre un format strict au départ.

## Écrire un skill pour Gemini CLI

Les skills Gemini CLI peuvent être installés depuis un dépôt Git en ciblant un chemin. Une fois un skill prêt, le principe d’installation est :

```bash
gemini skills install <url-du-depot> --path skills/gemini/<nom-du-skill>
```

Consulte la [documentation Gemini CLI](https://github.com/google-gemini/gemini-cli) pour les détails et les évolutions de la commande.

## Source d’inspiration

- [mattpocock/skills](https://github.com/mattpocock/skills) — collection de skills d’ingénierie, petits, adaptables et composables.
