
#### avant ce prompt il faut exécuter git diff --name-only develop...HEAD puis predre le resultat 


@workspace utilise :
- .github/copilot/agent-ba-back.md
- .github/copilot/agent-code-review-back.md

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
1. une revue technique,
2. une revue fonctionnelle.

Vérifie :
- la qualité du code,
- le respect des conventions du projet,
- le respect de l’architecture existante,
- les validations,
- la sécurité,
- la performance,
- les tests JUnit/Mockito,
- la couverture du besoin métier,
- les risques de régression.

Prioriser l’analyse :
- des fichiers modifiés,
- des tests modifiés,
- des composants impactés.

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