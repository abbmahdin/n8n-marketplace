# n8n Marketplace

**ThemeForest pour les templates n8n** — marketplace de templates d'automatisation n8n.

## Status

🚧 **Ébauchure / scaffolding** — structure Next.js + Tailwind CSS initialisée, mais aucun composant ou route n'est encore implémenté.

## Stack

- **Frontend** : Next.js 14 + React 18 + TypeScript + Tailwind CSS 3
- **Base de données** : Supabase (PostgreSQL + auth via `@supabase/supabase-js`)
- **Paiements** : Stripe SDK (`stripe`)
- **Tests** : Vitest + React Testing Library

## Prérequis

- Node.js 20+
- npm / yarn
- Compte Supabase
- Clé API Stripe (pour la production)

## Installation

```bash
npm install
```

## Variables d'environnement

```bash
# .env.local
NEXT_PUBLIC_SUPABASE_URL=your-supabase-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-supabase-anon-key
STRPIE_SECRET_KEY=your-stripe-secret-key
```

## Développement

```bash
npm run dev
```

Ouvre [http://localhost:3000](http://localhost:3000).

## Build

```bash
npm run build
npm run start
```

## Tests

```bash
# Tous les tests
npm run test

# Watch mode
npm run test:watch

# Couverture
npm run test:coverage

# UI
npm run test:ui
```

## TODO

- [ ] Pages: marketplace (liste des templates), checkout, dashboard utilisateur
- [ ] Intégration Supabase pour la gestion des comptes et achats
- [ ] Intégration Stripe pour le paiement des templates
- [ ] Structure des templates (upload, preview, catégorisation)
- [ ] Système de review/utilisateur

## Description

n8n Marketplace est un marketplace de templates d'automatisation pour [n8n](https://n8n.io/), inspiré de ThemeForest mais dédié aux workflows. Les utilisateurs peuvent découvrir, acheter et télécharger des templates n8n prêts à l'emploi.

### Fonctionnalités prévues

- Parcourir les templates par catégorie
- Acheter avec Stripe
- Télécharger les fichiers JSON n8n
- Gérer ses achats depuis le dashboard
- Laisser des reviews et notes