---
theme: default
title: AI-Augmented Software Engineering
info: |
  Contrôler l’IA plutôt que “vibe coder”
class: text-center
drawings:
  persist: false
transition: fade
mdc: true
---

# AI-Augmented Software Engineering
## Contrôler l’IA plutôt que “vibe coder”

<br>

### Une approche pragmatique pour intégrer les agents IA dans un workflow de développement classique

---

# Le problème

<div class="grid grid-cols-2 gap-8">

<div>

## Ce que l’IA fait très bien

- Produire vite
- Générer du boilerplate
- Explorer des solutions
- Écrire des tests
- Accélérer l’itération

</div>

<div>

## Ce qu’elle fait mal

- Respecter implicitement les conventions
- Maintenir une architecture cohérente
- Comprendre le contexte métier tacite
- Anticiper les impacts globaux
- Garantir la qualité seule

</div>

</div>

<br>

## Risque principal

### Laisser l’agent produire du code sans cadre explicite

---

# L’idée générale

<div class="text-center text-2xl mt-12">

## On ne contrôle pas directement le modèle.

## On contrôle :

</div>

<br>

<div class="grid grid-cols-2 gap-12 text-xl">

<div>

### 1. Les entrées

- Les spécifications
- Les conventions
- Les règles
- Le contexte fourni

</div>

<div>

### 2. Les sorties

- Les tests
- Les reviews
- Les pull requests
- Les validations humaines

</div>

</div>

---

# Stack méthodologique

<div class="text-center text-3xl mt-10">

OpenSpec (léger)

<span class="text-4xl">+</span>

Superpowers / Skills

<span class="text-4xl">+</span>

Workflow Git/PR classique

<span class="text-4xl">+</span>

Tests automatisés forts

<span class="text-4xl">+</span>

Review humaine obligatoire

</div>

---

# Vue d’ensemble

```mermaid {scale: 1.6}
flowchart LR

A[Feature Request] --> B[OpenSpec]
B --> C[Technical Specification]

C --> D[Claude Code / Agent]
D --> E[Implementation]

E --> F[Automated Tests]
F --> G[Pull Request]

G --> H[Human Review]

H -->|Approved| I[Merge]
H -->|Rejected| D
```
