@workspace utilise :
- .github/copilot/agent-ba-front.md
- .github/copilot/agent-develop-front.md

Implémente la fonctionnalité décrite dans le ticket Jira suivant :
/docs/jira/JIRA-123.md

Avant de développer :

1. Analyser le ticket Jira.
2. Comprendre le besoin fonctionnel et UX.
3. Identifier les modules frontend impactés.
4. Lire la documentation existante dans /docs.
5. Identifier les implémentations similaires déjà présentes dans le projet.
6. Identifier :
   - les conventions Angular,
   - les patterns d’architecture frontend,
   - les conventions de composants,
   - les pratiques de formulaires,
   - les validations UI,
   - les conventions de state management,
   - les conventions d’appels API,
   - les pratiques de tests frontend,
   - les conventions de routing,
   - les pratiques UX/UI déjà en place.

Respecter strictement :
- l’architecture frontend existante,
- les patterns Angular déjà utilisés,
- les conventions du projet,
- les pratiques Craft déjà en place.

Ne jamais :
- introduire une nouvelle architecture frontend,
- créer des patterns non utilisés dans le projet,
- faire un refactoring global non demandé,
- modifier des modules non impactés,
- régénérer la documentation existante dans /docs.

Modifier uniquement :
- les composants nécessaires,
- les services impactés,
- les formulaires concernés,
- les routes concernées,
- les tests associés.

Générer :
- les composants Angular,
- les services frontend,
- les formulaires,
- les validations UI,
- les guards si nécessaire,
- les interceptors si nécessaire,
- les appels API,
- les modèles/interfaces,
- la gestion des erreurs frontend,
- les messages utilisateur cohérents,
- les tests unitaires frontend,
- les tests des composants,
- les tests des services,
- les tests des formulaires.

Les tests doivent :
- couvrir les cas nominaux,
- couvrir les cas d’erreur,
- couvrir les validations,
- couvrir les comportements conditionnels,
- couvrir les workflows utilisateur,
- respecter les conventions de tests existantes.

Toujours :
- privilégier du code lisible,
- respecter SOLID,
- respecter Clean Code,
- éviter la duplication,
- privilégier des composants réutilisables,
- limiter le couplage,
- respecter la séparation des responsabilités,
- respecter les patterns Angular existants.

Avant de générer du code :
- vérifier les composants similaires existants,
- vérifier les workflows UI existants,
- vérifier les validations existantes,
- vérifier les permissions frontend existantes,
- vérifier les appels API existants,
- vérifier les patterns de formulaires existants.

Utilise la documentation existante dans /docs comme source principale de contexte fonctionnel et technique.

Ne jamais inventer :
- de workflows UI inexistants,
- de comportements métier non présents,
- de validations non prévues,
- de comportements backend supposés.

Le code généré doit :
- être cohérent avec le reste du projet,
- être prêt pour une Pull Request,
- être maintenable,
- être testable,
- être aligné avec les pratiques frontend existantes.

Utilise uniquement des caractères UTF-8 standards.
Ne jamais générer :
- d’emojis,
- de caractères Unicode invisibles,
- de caractères de contrôle,
- de caractères cachés,
- de texte corrompu.