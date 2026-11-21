# Gemini Skills Brainstorm

Un espace personnel pour noter, organiser et faire mûrir des idées de skills destinés à m’aider pendant le développement, en particulier avec [Gemini CLI](https://github.com/google-gemini/gemini-cli).

Ce dépôt s’inspire de [mattpocock/skills](https://github.com/mattpocock/skills) : des consignes ciblées, réutilisables et faciles à adapter au fil du travail. Ici, les idées pourront venir de conversations avec différentes IA, puis évoluer vers des exemples concrets.

## Organisation

```text
.
├── ideas/       # Notes brutes et pistes à explorer
├── skills/      # Skills en cours ou prêts à l’emploi
│   └── gemini/  # Skills au format Agent Skills de Gemini CLI
└── examples/   # Exemples d’utilisation et de résultats
```

Le contenu est volontairement léger : une idée peut commencer comme une note dans `ideas/`, puis être déplacée ou développée dans `skills/` quand elle devient assez claire. Les exemples associés peuvent aller dans `examples/`.

## Ajouter une idée

Crée un fichier Markdown dans `ideas/` avec le problème à résoudre, le contexte où il se présente et le comportement souhaité de l’IA. Pas besoin de suivre un format strict au départ.

## Écrire un skill pour Gemini CLI

Chaque skill est un dossier contenant un `SKILL.md` avec un frontmatter `name` et `description`. Gemini CLI découvre les skills depuis `.gemini/skills/` ou `.agents/skills/`. Dans ce dépôt, ils sont rangés sous `skills/gemini/` pour les partager sans les activer automatiquement dans ce projet.

### Premiers brouillons

| Skill | Rôle |
| --- | --- |
| [auditor](skills/gemini/auditor/SKILL.md) | Auditer le code et remonter les problèmes significatifs avec preuves. |
| [documenter](skills/gemini/documenter/SKILL.md) | Mettre à jour la documentation touchée par un changement. |
| [doc-auditor](skills/gemini/doc-auditor/SKILL.md) | Vérifier la cohérence entre documentation et comportement du code. |
| [kaizen](skills/gemini/kaizen/SKILL.md) | Analyser les sessions Gemini via le serveur MCP Kaizen et recommander des améliorations concrètes. |
| [deep-reviewer](skills/gemini/deep-reviewer/SKILL.md) | Coordonner quatre revues spécialisées avant merge et consolider les constats. |
| [repo-onboarding](skills/gemini/repo-onboarding/SKILL.md) | Cartographier un dépôt et préparer une documentation d’accueil vérifiable avec contrats et modèles. |

Ce sont des skills minimalistes, pas des agents autonomes : chacun apporte une méthode ciblée. Ils peuvent être liés localement pendant leur élaboration :

```bash
gemini skills link ./skills/gemini/auditor --scope user
```

Pour en installer un depuis le dépôt Git, utilise `gemini skills install <url-du-depot> --path skills/gemini/<nom-du-skill>`. Voir la [documentation Gemini CLI sur les Agent Skills](https://geminicli.com/docs/cli/skills/) pour les détails.

## Source d’inspiration

- [mattpocock/skills](https://github.com/mattpocock/skills) — collection de skills d’ingénierie, petits, adaptables et composables.
