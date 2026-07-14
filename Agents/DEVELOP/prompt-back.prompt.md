@workspace

Utilise uniquement les instructions présentes dans :

- .github/copilot/agent-ba-back.md
- .github/copilot/agent-develop-back.md

Ces fichiers sont des fichiers de configuration des agents.

Ne jamais les modifier, les régénérer ou proposer leur mise à jour.

Ils servent uniquement de contexte pour réaliser cette tâche.

Implémente la fonctionnalité décrite dans :

/docs/jira/JIRA-123.md

Avant toute modification :

1. Lire le ticket Jira.
2. Comprendre le besoin métier.
3. Identifier les modules impactés.
4. Lire la documentation présente dans /docs.
5. Identifier les implémentations similaires.
6. Identifier les conventions du projet.

Analyser notamment :

- les ressources REST JAX-RS similaires ;
- les services similaires ;
- les interfaces similaires ;
- les DTO similaires ;
- les Mapper MapStruct similaires ;
- les validators similaires ;
- les exceptions similaires ;
- les clients SOAP similaires ;
- les clients HTTP similaires ;
- les tests similaires.

Respecter impérativement :

- l'architecture existante ;
- les conventions Maven ;
- l'organisation actuelle des packages ;
- les patterns déjà utilisés ;
- les conventions de logging ;
- la stratégie de gestion des erreurs ;
- les validations existantes ;
- les règles métier existantes.

Ne jamais :

- introduire un nouveau framework ;
- modifier l'architecture ;
- créer un nouveau pattern ;
- effectuer un refactoring global ;
- modifier des modules non concernés ;
- régénérer la documentation présente dans /docs.

Modifier uniquement les composants impactés.

Créer uniquement si nécessaire :

- ressources REST JAX-RS ;
- services ;
- interfaces ;
- DTO ;
- Mapper MapStruct ;
- validators ;
- exceptions ;
- clients SOAP ;
- clients HTTP ;
- configuration.

Générer également :

- les tests JUnit 5 ;
- les tests Mockito ;
- les tests des cas nominaux ;
- les tests des cas d'erreur ;
- les tests des validations ;
- les tests des cas limites.

Avant de produire le code :

- vérifier les dépendances existantes ;
- vérifier les workflows métier ;
- vérifier les règles métier ;
- vérifier les validations ;
- vérifier les mécanismes de sécurité ;
- rechercher un composant similaire afin d'en reproduire la structure et les conventions.

Le code généré doit donner l'impression d'avoir été écrit par les développeurs historiques du projet.

Toute décision doit être justifiée par le code existant.

Utiliser uniquement des caractères UTF-8 standards.