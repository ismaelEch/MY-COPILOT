@workspace utilise .github/copilot/agent-ba-back.md

Analyse l’intégralité du backend NestJS monolithique.

Objectifs :
- comprendre l’architecture globale,
- identifier les modules métier,
- extraire les règles de gestion implicites,
- analyser les workflows métier,
- documenter les composants techniques,
- cartographier les dépendances inter-modules,
- analyser les relations TypeORM et la structure MySQL,
- identifier les permissions, guards et mécanismes de sécurité,
- documenter les APIs et les flux de données.

Analyse en priorité :
- services,
- controllers,
- entities,
- DTO,
- validators,
- guards,
- repositories,
- interceptors,
- workflows,
- routes API,
- cron jobs,
- queues,
- providers.

Génère la documentation complète dans /docs.

Produis notamment :

- /docs/architecture/backend-overview.md
- /docs/modules
- /docs/business-rules
- /docs/workflows
- /docs/api
- /docs/database
- /docs/dependencies

Pour chaque module métier, documenter :
- l’objectif métier,
- les responsabilités,
- les endpoints API,
- les entités utilisées,
- les règles métier,
- les workflows,
- les permissions,
- les dépendances techniques,
- les risques techniques.

Pour chaque règle métier :
- fournir un identifiant,
- expliquer la condition,
- expliquer le comportement attendu,
- expliquer les exceptions,
- citer les sources techniques exactes :
  - fichiers,
  - services,
  - méthodes,
  - validators,
  - guards,
  - DTO.

Toujours relier les conclusions au code réel.
Ne jamais inventer de comportements non observés dans le codebase.

Identifier également :
- les couplages forts,
- les circular dependencies,
- les composants critiques,
- les zones sensibles,
- les risques de dette technique.

Utilise uniquement des caractères UTF-8 standards.
Ne jamais générer :
- de caractères Unicode invisibles,
- de caractères de contrôle,
- de caractères cachés,
- de texte corrompu.

Le niveau de détail attendu est très poussé.
La documentation doit être exploitable par :
- Tech Leads,
- Business Analysts,
- développeurs,
- QA,
- Product Owners.