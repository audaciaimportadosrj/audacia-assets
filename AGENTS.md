# Asset repository rules

This repository is the canonical asset library for the Audácia Importados website and related digital materials.

- Store generated or supplied public-facing assets here by default instead of committing binaries to the application repository.
- Use the category paths documented in README.md.
- Use lowercase kebab-case ASCII filenames.
- Prefer versioned published filenames, e.g. `hero-home-v2.webp`, rather than overwriting a CDN-served file.
- Optimize images for the web before publishing when possible.
- Prefer SVG for custom icons/logos when the source is vector; prefer WebP/AVIF for photographic imagery.
- Do not store secrets, customer data, credentials, private documents, or licensed files that are not allowed to be public.
- When an asset is added or replaced, update the consumer mapping in `audaciaimportadosrj/blank-slate-savings/src/lib/assets.ts` when applicable.
- Default public delivery URL: `https://cdn.jsdelivr.net/gh/audaciaimportadosrj/audacia-assets@main/<path>`.
