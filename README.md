# Tony Schietroma

[![LinkedIn](https://img.shields.io/badge/LinkedIn-tonyschietroma-0A66C2?style=flat)](https://linkedin.com/in/tonyschietroma)
![Paris](https://img.shields.io/badge/📍-Paris-555?style=flat)

Sales & Business Development chez **D'Or et de Vins**, agence de distribution B2B
de vins indépendants auprès des restaurants, cavistes et business clubs.

En parallèle de la vente, je conçois et développe **le logiciel tout-en-un de l'agence** :
CRM, catalogue, tarifs, commandes, facturation, commissions et pilotage dans un seul outil,
de la fiche domaine jusqu'à la relance de paiement.

## 🍷 Le logiciel de l'agence

[agence-doretdevins.com](https://agence-doretdevins.com) · dépôt privé · en production

`89 tables` · `45 Edge Functions` · `RLS sur 100 % des tables (225 politiques)` · `388 PR fusionnées`

| Pôle | Ce qu'il couvre |
|---|---|
| **Commercial** | CRM comptes et contacts avec carte, pipeline d'opportunités en kanban, devis validés en ligne par le client, objectifs par domaine, commissions mensuelles par commercial |
| **Catalogue & prix** | 32 domaines, 975 références, grilles CHR et caviste, paliers, franco, promotions, allocations par cuvée |
| **Commandes & facturation** | Commandes saisies, collées en texte libre ou passées depuis l'espace client · factures · synchro Qonto · relances automatiques par stade de retard |
| **Pilotage** | Reporting par client, domaine, commercial, produit et zone, export Excel |
| **Équipe** | Planning, rendez-vous avec rappels, absences, flux iCal |
| **Site & marketing** | Site vitrine et catalogue public avec pré-rendu SEO, synchro Brevo, posts Instagram planifiés |

Quatre rôles (admin, commercial, client pro, vigneron) avec des espaces séparés.

### 🤖 IA intégrée (Claude API)
- Lecture des catalogues et grilles tarifaires PDF des domaines
- Commandes collées en texte libre, transformées en commandes structurées
- Lecture et classement des factures
- Agent mail qui propose relances et notes d'échange, validées par un humain

### ⚙️ Automatisations
- **n8n** : chaîne des factures (mails → Drive → logiciel, Qonto → Drive), alertes d'erreur
- **pg_cron** : 10 tâches planifiées, dont la synchro nocturne des contacts vers Brevo
- **GitHub Actions** : sauvegarde quotidienne de la base, récap hebdomadaire

### Ce qu'il a remplacé
- Notion pour les commandes et les fiches clients, avec reprise de l'historique depuis 2023
- Les tableurs Excel de tarifs
- Le classement manuel des factures et les relances de paiement à la main

### Architecture
- **Front** : React 18, TypeScript, Vite, Tailwind, shadcn/ui, React Query
- **Back** : Supabase (PostgreSQL, Auth, Storage), Edge Functions en Deno, pg_cron
- **Intégrations** : Qonto, Brevo, Resend, Claude API, Google Drive et Maps, Meta Graph API
- **Déploiement** : Vercel

## Stack

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Deno](https://img.shields.io/badge/Deno-000000?style=for-the-badge&logo=deno&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-336791?style=for-the-badge)
![Claude API](https://img.shields.io/badge/Claude_API-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![Brevo](https://img.shields.io/badge/Brevo-0B996E?style=for-the-badge&logo=brevo&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
