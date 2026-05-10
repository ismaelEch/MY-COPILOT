
@workspace utilise :
- .github/copilot/agent-ba-back.md
- .github/copilot/agent-develop-back.md

Implémente la fonctionnalité décrite dans le ticket Jira suivant :
/docs/jira/JIRA-123.md

Avant de développer :

1. Analyser le ticket Jira.
2. Comprendre le besoin métier.
3. Identifier les modules impactés.
4. Lire la documentation existante dans /docs.
5. Identifier les implémentations similaires déjà présentes dans le projet.
6. Identifier :
   - les conventions de nommage,
   - les patterns d’architecture,
   - les pratiques de validation,
   - les pratiques de tests,
   - les conventions DTO/mapping,
   - les conventions de gestion des erreurs.

Respecter strictement :
- l’architecture existante,
- les patterns déjà utilisés,
- les conventions du projet,
- les pratiques Craft déjà en place.

Ne jamais :
- introduire une nouvelle architecture,
- créer des patterns non utilisés dans le projet,
- faire de refactoring global non demandé,
- modifier des modules non impactés,
- régénérer la documentation existante dans /docs.

Modifier uniquement :
- les fichiers nécessaires,
- les composants impactés,
- les tests associés.

Générer :
- le code métier,
- les services,
- les DTO,
- les validators,
- les mappings,
- les repositories si nécessaire,
- les contrôleurs si nécessaire,
- la gestion des erreurs,
- les tests unitaires JUnit 5,
- les tests Mockito,
- les tests de service,
- les tests de validation.

Les tests doivent :
- couvrir les cas nominaux,
- couvrir les cas d’erreur,
- couvrir les validations,
- couvrir les cas limites,
- respecter les conventions de test existantes.

Toujours :
- privilégier du code lisible,
- respecter SOLID,
- respecter Clean Code,
- éviter la duplication,
- privilégier la testabilité,
- limiter le couplage.

Avant de générer du code :
- vérifier les dépendances existantes,
- vérifier les workflows métier existants,
- vérifier les règles métier existantes,
- vérifier les permissions et validations existantes.

Utilise la documentation existante dans /docs comme source principale de contexte métier et technique.

Ne jamais inventer :
- de comportements métier,
- de règles de gestion,
- de workflows,
- de validations inexistantes dans le projet.

Le code généré doit :
- être cohérent avec le reste du projet,
- être prêt pour une Pull Request,
- être maintenable,
- être testable,
- être aligné avec les pratiques existantes.

Utilise uniquement des caractères UTF-8 standards.
Ne jamais générer :
- d’emojis,
- de caractères Unicode invisibles,
- de caractères de contrôle,
- de caractères cachés,
- de texte corrompu.