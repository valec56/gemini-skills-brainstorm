---
name: repo-onboarding
description: >
  Analyse un dépôt logiciel et prépare un dossier d'onboarding fiable :
  présentation, architecture, commandes de développement, carte des modules
  et lacunes documentaires. À utiliser pour comprendre un projet, préparer
  l'arrivée d'un développeur ou d'un agent IA, créer un README ou cartographier
  l'architecture et les commandes du dépôt.
---

# Repo Onboarding

Produis une compréhension actionnable du dépôt pour un développeur qui le découvre. Fonde chaque affirmation sur les fichiers et indices observés ; distingue les faits des hypothèses.

## Méthode

1. **Inventorier** les fichiers de configuration, manifestes, scripts, CI, documentation, modules, points d'entrée et tests pertinents.
2. **Cartographier** le périmètre du projet, les composants, leurs responsabilités, les flux principaux et les dépendances externes.
3. **Relever les commandes** de build, test, lint, formatage, migration et démarrage. Indique leur source et leurs prérequis. N'affirme pas qu'une commande fonctionne sans l'avoir exécutée ; exécute-la uniquement si c'est sans risque et dans le périmètre demandé.
4. **Préparer les documents** pertinents dans `docs/onboarding-proposal/`, en t'appuyant sur les modèles de `assets/` :
   - `README.md` : objectif, prérequis, installation, configuration, démarrage et commandes.
   - `ARCHITECTURE.md` : composants, responsabilités, flux et décisions visibles.
   - `DEVELOPMENT.md` : workflow, commandes, tests, conventions et dépannage.
   - `module-map.md` : modules, dépendances et tests associés.
   - `onboarding-gaps.md` : informations manquantes, incohérences et questions.
   Ne conserve que les documents utiles et évite de dupliquer une documentation existante.
5. **Terminer** par le rapport décrit dans `references/output-contract.md`.

## Limites et qualité

- N'invente ni comportement, ni prérequis, ni décision technique. Marque les incertitudes « À confirmer ».
- Ne modifie pas le code applicatif, les tests, la CI ou la configuration.
- Évite d'exposer des secrets et valeurs sensibles. Ne copie pas les valeurs de fichiers d'environnement.
- Si les documents proposés ne sont pas explicitement autorisés, présente-les comme proposition et ne modifie aucun autre emplacement.

