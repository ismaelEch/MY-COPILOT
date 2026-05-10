# Skills globaux recommandés pour un projet Java Spring Boot / Angular avec GitHub Copilot

Ces skills sont des règles globales transverses qui améliorent fortement :

* la qualité du code,
* la cohérence du projet,
* la stabilité des agents,
* les reviews,
* les tests,
* les performances,
* la maintenabilité.

L’objectif est d’éviter :

* les dérives de conventions,
* les hallucinations,
* les architectures incohérentes,
* les patterns contradictoires,
* les régressions qualité.

---

# Structure recommandée

```txt
.github/copilot/
   agents/
   prompts/
   skills/
```

---

# 1. skill-global-architecture.md

## Objectif

Définit les règles globales d’architecture du projet.

---

## Contenu recommandé

* architecture hexagonale ou layered,
* séparation controller/service/repository,
* responsabilités,
* conventions modules,
* dépendances autorisées,
* conventions packages,
* conventions Angular,
* conventions state management,
* conventions API,
* conventions DTO,
* règles SOLID,
* règles Clean Architecture.

---

## Usage

À utiliser avec :

* agent-develop,
* agent-code-review,
* agent-ba.

---

## Exemple

```txt
@workspace utilise :
- .github/copilot/skills/skill-global-architecture.md
- .github/copilot/agent-develop-back.md
```

---

# 2. skill-clean-code.md

## Objectif

Centraliser les standards Craft.

---

## Contenu recommandé

* SOLID,
* DRY,
* KISS,
* YAGNI,
* conventions naming,
* taille méthodes,
* taille classes,
* conventions exceptions,
* conventions logs,
* conventions validations,
* conventions mapping.

---

## Usage

Très utile pour :

* développement,
* review,
* tests.

---

# 3. skill-testing-standards.md

## Objectif

Uniformiser les tests.

---

## Contenu recommandé

## Backend

* JUnit 5,
* Mockito,
* AAA,
* edge cases,
* boundary conditions,
* conventions mocks,
* conventions assertions,
* tests services,
* tests validators.

---

## Frontend

* Angular Testing,
* Jasmine/Jest,
* RxJS tests,
* tests formulaires,
* tests workflows.

---

## Usage

À utiliser avec :

* agent-unit-test,
* agent-code-review,
* agent-develop.

---

# 4. skill-security.md

## Objectif

Imposer des standards sécurité.

---

## Contenu recommandé

* validation inputs,
* SQL injection,
* XSS,
* auth,
* rôles,
* permissions,
* JWT,
* secrets,
* logs sensibles,
* OWASP,
* protections API,
* validation backend,
* validation frontend.

---

## Usage

Très utile avec :

* review,
* développement,
* query builder.

---

# 5. skill-performance.md

## Objectif

Éviter les problèmes performance.

---

## Contenu recommandé

## Backend

* N+1,
* lazy/eager loading,
* pagination,
* batch processing,
* cache,
* index DB,
* optimisations SQL.

---

## Frontend

* change detection,
* subscriptions RxJS,
* lazy loading,
* renders inutiles,
* optimisation Angular.

---

## Usage

Très utile pour :

* review,
* query builder,
* développement.

---

# 6. skill-api-standards.md

## Objectif

Uniformiser les APIs.

---

## Contenu recommandé

* conventions REST,
* conventions endpoints,
* conventions DTO,
* pagination,
* sorting,
* filtering,
* gestion erreurs,
* codes HTTP,
* versioning,
* Swagger/OpenAPI.

---

## Usage

À utiliser avec :

* develop,
* review,
* BA.

---

# 7. skill-angular-standards.md

## Objectif

Centraliser les standards Angular.

---

## Contenu recommandé

* structure modules,
* smart/dumb components,
* RxJS,
* formulaires,
* guards,
* interceptors,
* state management,
* routing,
* conventions services,
* conventions composants.

---

## Usage

Très utile pour :

* frontend develop,
* frontend review,
* frontend tests.

---

# 8. skill-springboot-standards.md

## Objectif

Centraliser les standards Spring Boot.

---

## Contenu recommandé

* conventions services,
* conventions repositories,
* conventions transactions,
* conventions exceptions,
* conventions DTO,
* validation Bean Validation,
* conventions JPA,
* conventions JPQL,
* conventions logs,
* conventions sécurité.

---

## Usage

Très utile pour :

* develop backend,
* review backend,
* query builder JPA.

---

# 9. skill-git-pr-review.md

## Objectif

Standardiser les reviews Git/PR.

---

## Contenu recommandé

* checklist PR,
* checklist sécurité,
* checklist performance,
* checklist tests,
* checklist architecture,
* checklist régression,
* checklist UX.

---

## Usage

À utiliser avec :

* agent-code-review.

---

# 10. skill-encoding-and-output.md

## Objectif

Éviter les problèmes de génération IA.

---

## Contenu recommandé

Toujours utiliser :

* UTF-8 standard.

Ne jamais générer :

* emojis,
* caractères Unicode invisibles,
* caractères de contrôle,
* caractères cachés,
* texte corrompu.

Toujours produire :

* du texte lisible,
* du code propre,
* des sorties maintenables.

---

## Usage

À utiliser globalement partout.

---

# Workflow recommandé

## Développement backend

```txt
@workspace utilise :
- .github/copilot/skills/skill-global-architecture.md
- .github/copilot/skills/skill-clean-code.md
- .github/copilot/skills/skill-springboot-standards.md
- .github/copilot/skills/skill-security.md
- .github/copilot/skills/skill-performance.md
- .github/copilot/skills/skill-encoding-and-output.md
- .github/copilot/agent-develop-back.md
```

---

# Développement frontend

```txt
@workspace utilise :
- .github/copilot/skills/skill-global-architecture.md
- .github/copilot/skills/skill-clean-code.md
- .github/copilot/skills/skill-angular-standards.md
- .github/copilot/skills/skill-performance.md
- .github/copilot/skills/skill-encoding-and-output.md
- .github/copilot/agent-develop-front.md
```

---

# Review backend

```txt
@workspace utilise :
- .github/copilot/skills/skill-clean-code.md
- .github/copilot/skills/skill-security.md
- .github/copilot/skills/skill-performance.md
- .github/copilot/skills/skill-git-pr-review.md
- .github/copilot/agent-code-review-back.md
```

---

# Tests backend

```txt
@workspace utilise :
- .github/copilot/skills/skill-testing-standards.md
- .github/copilot/skills/skill-clean-code.md
- .github/copilot/agent-unit-test-back.md
```

---

# Query Builder SQL/JPQL

```txt
@workspace utilise :
- .github/copilot/skills/skill-performance.md
- .github/copilot/skills/skill-security.md
- .github/copilot/skills/skill-springboot-standards.md
- .github/copilot/agent-jpa-query-builder.md
```

---

# Recommandation importante

Ne pas charger tous les skills systématiquement.

Toujours charger uniquement les skills utiles au workflow courant.

Sinon :

* contexte dilué,
* réponses moins précises,
* coût contexte plus élevé,
* comportements moins stables.

---

# Architecture idéale finale

```txt
.github/copilot/
   agents/
   prompts/
   skills/
   docs/
```

---

# Répartition idéale

## agents/

Responsabilité métier et comportement IA.

---

## prompts/

Workflows réutilisables.

---

## skills/

Standards transverses globaux.

---

## docs/

Contexte métier et technique du projet.
