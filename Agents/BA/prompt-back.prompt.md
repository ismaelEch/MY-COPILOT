@workspace utilise .github/copilot/agent-ba-back.md

Analyse l'intégralité du backend Java.

Le projet est basé sur :

- Java 11
- Maven
- Packaging WAR
- Architecture Java d'entreprise
- JAX-RS
- MapStruct
- Jackson
- Gson
- Apache CXF
- Infinispan
- SLF4J
- Swagger
- socle Covea (jee-*)
- clients SOAP
- clients HTTP

Objectifs :

- comprendre l'architecture globale
- identifier les domaines métier
- identifier les composants techniques
- documenter les APIs REST JAX-RS
- documenter les intégrations SOAP
- analyser les règles métier
- identifier les workflows métier
- cartographier les dépendances entre services
- identifier les validations métier
- documenter les DTO
- documenter les modèles
- documenter les MapStruct Mapper
- documenter les clients HTTP
- documenter les clients SOAP
- documenter le cache Infinispan
- documenter les mécanismes de sécurité
- documenter les configurations Maven
- identifier les dépendances critiques
- identifier la dette technique
- détecter les composants fortement couplés

Analyse en priorité :

- Services
- Interfaces
- Implémentations
- Ressources REST JAX-RS
- DTO
- Modèles
- Mappers
- Validators
- Exceptions
- Clients SOAP
- Clients HTTP
- Cache
- Configuration Maven
- pom.xml
- tests

Génère la documentation dans :

/docs/architecture
/docs/modules
/docs/business-rules
/docs/workflows
/docs/api
/docs/integrations
/docs/cache
/docs/security
/docs/dependencies

Pour chaque domaine métier, documenter :

- objectif métier
- responsabilités
- endpoints REST
- services
- DTO
- modèles
- mappers
- règles métier
- workflows
- intégrations externes
- dépendances
- risques techniques

Pour chaque règle métier :

- générer un identifiant unique
- décrire la règle
- expliquer les conditions
- expliquer le comportement
- documenter les exceptions
- citer les classes Java concernées
- citer les méthodes
- citer les endpoints REST associés
- citer les DTO concernés

Ne jamais inventer une règle métier.

Toute conclusion doit être justifiée par le code source.

Utiliser uniquement des caractères UTF-8 standards.