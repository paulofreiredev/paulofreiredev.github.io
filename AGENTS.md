# Agentes do portfólio

Projeto Astro estático, TypeScript, CSS e conteúdo Markdown. Público: leitores de português brasileiro. Destino: GitHub Pages.

## Fluxo

Use as definições em `.agents/` conforme o papel solicitado. São instruções de atuação para assistentes, sem dependência de um serviço de agentes. Fluxo recomendado: refinador → desenvolvedor → reviewer. Delegue somente quando solicitado pelo usuário.

- Refinador: `.agents/refinador.md`.
- Desenvolvedor: `.agents/desenvolvedor.md`.
- Reviewer: `.agents/reviewer.md`.

## Convenções

- Não invente informações pessoais, experiências ou métricas.
- Centralize dados pessoais em `src/data/profile.ts`.
- Use `url()` de `src/lib/paths.ts` para caminhos internos; suporte publicação em subdiretórios.
- Preserve HTML semântico, navegação por teclado, contraste e responsividade.
- Não exponha tokens no frontend; integração GitHub utiliza apenas dados públicos.
- Não versione `.env` nem `CONFIGURACAO.local.md`.
- Execute `npm run build` após mudanças de código; descreva limites de validação.
