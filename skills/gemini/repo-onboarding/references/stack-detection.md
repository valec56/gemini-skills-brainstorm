# Détection de stack

Utilise ces indices comme pistes, puis confirme-les dans les manifestes, scripts et sources. Ne conclus pas à partir d'un nom de dossier seul.

## Java et Spring Boot

**Indices :** `pom.xml`, `build.gradle*`, `src/main/java`, `application.yml`, dépendances Spring.

**À relever si présent :** version Java, outil et commandes de build, profils, base de données, migrations et points d'entrée HTTP.

## Front-end web

**Indices :** `package.json`, `src/`, `app/`, `pages/`, `components/`, dépendances ou configuration Vite, Next.js, Angular, React ou Vue.

**À relever si présent :** gestionnaire de paquets, commandes dev/build/test, routage, gestion d'état, appels API et noms de variables d'environnement (jamais leurs valeurs).

## Tests

Repérer les frameworks et commandes, la séparation unitaires/intégration/E2E, les rapports de couverture et les étapes de test présentes en CI.

## CI/CD et exploitation

Repérer les workflows CI, étapes de build et déploiement, conteneurs, scripts de migration, services requis et références à des secrets. Ne pas exposer de valeurs sensibles.

## Autres stacks

Déduire les technologies depuis les manifestes et les imports. Si les indices sont insuffisants ou contradictoires, décrire ce qui est établi et marquer le reste « À confirmer ».

