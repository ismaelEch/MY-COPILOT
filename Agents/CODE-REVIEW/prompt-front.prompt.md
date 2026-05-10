@workspace utilise :
- .github/copilot/agent-ba-front.md
- .github/copilot/agent-code-review-front.md

Analyse UNIQUEMENT les fichiers suivants,
correspondant au diff Git entre la branche courante et develop :

#### Fichiers modifiés
- src/main/java/com/example/user/UserService.java
- src/main/java/com/example/user/UserController.java
- src/test/java/com/example/user/UserServiceTest.java

Compare les implémentations actuelles avec :
- les patterns déjà présents dans develop,
- les conventions existantes du projet,
- les implémentations similaires existantes.


Utilise le ticket Jira suivant :
/docs/jira/JIRA-123.md

Effectue :
1. une revue technique frontend,
2. une revue fonctionnelle UX/UI.

Vérifie :
- la qualité du code Angular,
- le respect des conventions frontend,
- le respect de l’architecture existante,
- les workflows UI,
- les validations frontend,
- les formulaires,
- les appels API,
- les permissions frontend,
- les tests frontend,
- la couverture du besoin fonctionnel,
- les risques de régression.

Prioriser l’analyse :
- des composants modifiés,
- des services modifiés,
- des tests modifiés,
- des workflows impactés.

Comparer les implémentations modifiées avec les patterns déjà présents dans develop.

Génère un rapport structuré avec :
- remarques techniques,
- remarques fonctionnelles,
- classification des problèmes :
  - CRITIQUE,
  - MAJEUR,
  - MINEUR,
  - SUGGESTION,
- validation finale.

Utilise uniquement des caractères UTF-8 standards.
Ne jamais générer :
- d’emojis,
- de caractères Unicode invisibles,
- de caractères de contrôle,
- de caractères cachés,
- de texte corrompu.