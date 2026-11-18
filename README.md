# Tony Schietroma

[![LinkedIn](https://img.shields.io/badge/LinkedIn-tonyschietroma-0A66C2?style=flat)](https://linkedin.com/in/tonyschietroma)
![Paris](https://img.shields.io/badge/📍-Paris-555?style=flat)

Sales & Business Development chez **D'Or et de Vins**, agence de distribution B2B
de vins indépendants auprès des restaurants, cavistes et business clubs.

Je construis des logiciels et des automatisations qui suppriment le travail administratif :
un ERP sur mesure pour l'agence, des packs d'automatisation pour les TPE, des agents IA reliés à de vrais outils métier.

## Projets

### 🍷 Logiciel tout-en-un de l'agence D'Or et de Vins
*Privé · en production · [agence-doretdevins.com](https://agence-doretdevins.com)*

CRM, catalogue, tarifs, commandes, facturation, commissions et pilotage dans un seul outil,
de la fiche domaine jusqu'à la relance de paiement. Il a remplacé Notion et les tableurs de tarifs.

- **Commercial** : CRM avec carte, pipeline d'opportunités, devis validés en ligne, objectifs, commissions par commercial
- **Catalogue & prix** : 32 domaines, 975 références, grilles CHR et caviste, paliers, promotions, allocations
- **Commandes & facturation** : espace client pro, synchro Qonto, relances automatiques par stade de retard
- **Pilotage** : reporting par client, domaine, commercial, produit et zone
- **IA (Claude API)** : lecture des catalogues et grilles PDF, commandes en texte libre, classement des factures
- **Automatisations** : n8n (chaîne des factures), 10 tâches pg_cron, sauvegardes via GitHub Actions

`89 tables` · `45 Edge Functions` · `RLS sur 100 % des tables` · `388 PR fusionnées`

→ React, TypeScript, Vite, Tailwind · Supabase (PostgreSQL, Deno) · Vercel

### 📬 mcp-mail
*Privé · en production pour l'équipe commerciale*

Serveur MCP qui donne à Claude un accès en lecture à une boîte mail IMAP et branche ses outils sur le CRM de l'agence.
Il propose relances et notes d'échange, et classe les factures dans le Drive du domaine.

- **Sécurité d'abord** : aucun code d'envoi, l'IA ne peut qu'écrire des brouillons. Contenu des mails marqué comme non fiable
- **Une instance par boîte mail**, connexion OAuth GitHub limitée à une liste de comptes
- Les actions CRM passent par une Edge Function qui n'accepte que ce qu'un humain valide

→ Python, FastMCP, IMAP, Docker, Clever Cloud

### ⚡ Pivelis
*Privé · en lancement*

Offre d'automatisation pour artisans, commerçants et indépendants : des packs prêts à installer,
reliés aux outils du client (Gmail, Google Sheets, Drive, Agenda).

- **6 packs** : devis et factures, paiements et relances, chantier, factures fournisseurs, rendez-vous, assistant WhatsApp
- **Assistant WhatsApp** : devis dictés par message vocal, transcrits puis rédigés par Claude
- **Infra** : VPS en France déployé en une commande (n8n en HTTPS, pare-feu, sauvegardes chiffrées chaque nuit)
- Workflows n8n générés par script et couverts par des tests

→ n8n, Node.js, Claude API, Docker, Caddy, Google Workspace APIs

### 🔎 job-radar-n8n
*Privé*

Workflow n8n de veille d'offres d'emploi : interroge l'API Greenhouse d'une liste d'entreprises,
déduplique les offres et les pousse dans une base Notion pour tri manuel.

→ n8n, Greenhouse API, Notion API

## Stack

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![Claude API](https://img.shields.io/badge/Claude_API-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=for-the-badge&logo=modelcontextprotocol&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Notion API](https://img.shields.io/badge/Notion_API-000000?style=for-the-badge&logo=notion&logoColor=white)
