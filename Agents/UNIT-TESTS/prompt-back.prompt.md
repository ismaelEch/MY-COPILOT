@workspace utilise :
- .github/copilot/agent-ba-back.md
- .github/copilot/agent-unit-test-back.md

Analyse le code sélectionné et génère les tests unitaires complets.

Respecter :
- les conventions de tests existantes,
- les patterns Mockito/JUnit existants,
- les pratiques Craft du projet.

Toujours couvrir :
- cas nominaux,
- cas d’erreur,
- edge cases,
- boundary conditions,
- validations métier,
- exceptions,
- comportements critiques.

Générer :
- tests JUnit 5,
- tests Mockito,
- mocks pertinents,
- assertions explicites,
- tests maintenables.

Ne jamais :
- générer des tests redondants,
- générer des mocks inutiles,
- générer des assertions faibles,
- générer des tests fragiles.

Utilise uniquement des caractères UTF-8 standards.
Ne jamais générer :
- d’emojis,
- de caractères Unicode invisibles,
- de caractères de contrôle,
- de caractères cachés,
- de texte corrompu.