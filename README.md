# Dashboard Gerencial — Halwa AI

Painel web gerencial para transportadoras. Produto replicável da Halwa AI.
Cliente piloto: Transportadora Valência (Transvalen).

## Como funciona
- Site estático (um único `index.html`) hospedado na Vercel.
- Deploy automático: todo commit na branch `main` publica sozinho em produção.
- Fonte da verdade do código: este repositório. O que está no ar reflete sempre o `main`.

## Status atual (protótipo de design)
Dados fictícios, para validar visual e experiência — ainda não conectado ao banco real.
Painéis prontos: Visão Geral, Comercial, Leads (Atendimento IA).
Próximas fases: Tráfego (Google Ads), Custos & Frota.

## Multi-cliente (revenda)
Marca, cores e nome do cliente vivem no objeto `TENANT`, no topo do `index.html`.
Para uma nova transportadora, editar apenas esse bloco — sem tocar no resto do código.

## Stack (produto final)
Next.js + Tailwind + Recharts + PostgreSQL (lido pelo dashboard); dados alimentados por automações n8n.

## Como atualizar
Editar o `index.html` na branch `main` → a Vercel republica automaticamente.
