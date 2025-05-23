# API de raccourcisseur d’URL

## Objectif

Créer une API simple qui permet de raccourcir une URL et de la rediriger vers l’originale.
---

## Stack technique

Langage : TS (Node.js)

Framework : Express.js

Base de données : In-memory

Tests : Jest

---

## Fonctionnalités

### 1. POST /shorten

Prend une URL longue et retourne un code court.

**Requête :**

```
json
POST /shorten
{
  "url": "https://example.com"
}
```

**Réponse :**

```
json
{
  "short": "abc123"
}
```

---

### 2. GET /:short

Redirige vers l’URL d’origine.

**Exemple :**

GET /abc123
→ redirection vers https://example.com
