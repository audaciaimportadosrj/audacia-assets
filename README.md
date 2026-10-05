# Audácia Assets

Biblioteca oficial de mídia da **Audácia Importados RJ**.

Este repositório é público de propósito: os arquivos publicados aqui são consumidos pelo site e por outros materiais digitais da Audácia através de CDN.

## CDN

Base pública:

```text
https://cdn.jsdelivr.net/gh/audaciaimportadosrj/audacia-assets@main/
```

Exemplo:

```text
https://cdn.jsdelivr.net/gh/audaciaimportadosrj/audacia-assets@main/brand/logo-gold-v1.webp
```

## Estrutura

- `brand/` — logos, símbolos e elementos de identidade.
- `hero/` — imagens de destaque e backgrounds.
- `products/` — fotos e renders de produtos.
- `banners/` — campanhas e peças promocionais.
- `icons/` — SVGs e ícones próprios.
- `social/` — Open Graph, redes sociais e thumbnails.
- `fonts/` — fontes licenciadas para uso web.
- `video/` — vídeos leves e animações exportadas.
- `documents/` — PDFs e materiais públicos.
- `generated/` — assets gerados por ferramentas/IA ainda não classificados.

As pastas são criadas automaticamente quando o primeiro arquivo de cada categoria é publicado.

## Convenções

1. Use nomes em `kebab-case`, ASCII, sem espaços ou acentos.
2. Prefira `.webp` ou `.avif` para imagens de conteúdo e `.svg` para ícones vetoriais.
3. Preserve PNG quando transparência/qualidade exigir.
4. Não armazene segredos, arquivos privados, dados de clientes ou credenciais neste repositório.
5. Para assets publicados no site, prefira nomes versionados (`-v1`, `-v2`) em vez de sobrescrever o mesmo arquivo. Isso evita cache antigo na CDN.
6. Arquivos gerados para o projeto Audácia devem ser publicados aqui por padrão, e o projeto principal deve referenciá-los por CDN.

## Projeto consumidor

Projeto principal:

`audaciaimportadosrj/blank-slate-savings`

A integração de URLs fica centralizada em `src/lib/assets.ts` no projeto principal.
