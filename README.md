# Portfólio

Astro + TypeScript, com Home, blog Markdown e projetos do GitHub. Tema escuro com acentos violeta e azul. Geração estática para GitHub Pages, sem backend.

```sh
npm ci
npm run dev
```

`npm run build` valida os tipos e gera `dist/`. `npm run preview` serve a versão de produção.

- Informações pessoais: `src/data/profile.ts`.
- Foto: `public/images/profile.jpg` (reconstruir o site após adicionar).
- Artigos: `src/content/blog/*.md`.
- Papéis dos agentes: `AGENTS.md` e `.agents/`.

A integração usa a API pública do GitHub no navegador. Sem usuário configurado, mostra estado vazio. Selecione até seis nomes em `featuredRepos`; sem seleção, exibe os seis repositórios próprios, não arquivados, com mais estrelas. Falhas ou limites de API exibem uma mensagem e mantêm o link para o perfil.

O guia de configuração pessoal é `CONFIGURACAO.local.md`, ignorado pelo Git. Variáveis disponíveis estão em `.env.example`. A publicação usa `.github/workflows/deploy.yml` e detecta automaticamente domínio e subdiretório com a configuração do Pages.

## Novo artigo

```markdown
---
title: "Meu artigo"
description: "Uma descrição curta."
date: 2026-10-28
tags: ["Desenvolvimento"]
draft: false
---
Seu texto em Markdown.
```

Artigos com `draft: true` não são publicados. A data ordena os artigos, mas não agenda publicação. O artigo inicial é demonstrativo.

Documentação: https://docs.astro.build/en/guides/deploy/github/
