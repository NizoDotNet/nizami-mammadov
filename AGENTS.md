# AGENTS.md

## Commands
- Install: `npm install` (package-lock.json present)
- Dev: `npm run dev` (Nuxt dev on http://localhost:3000)
- Build: `npm run build`
- Preview: `npm run preview`
- Generate static: `npm run generate`
- Type preparation: `npm run postinstall` runs `nuxt prepare` (auto-runs after install)

## Stack / structure
- Nuxt 4 (type=module), Vue 3.5, Vue Router 5
- Modules: `@nuxt/ui`, `@nuxt/fonts` (see `nuxt.config.ts`)
- CSS: `~/assets/style.css` imported via `nuxt.config.ts`
- App directory: `app/` contains `app.vue`, `pages/` (`index.vue`, `blog/`, `projects/`, `tools/`), `layouts/`, `components/`, `assets/`
- TS config uses project references to `.nuxt/tsconfig.*.json` (generated)

## Notes
- `.nuxt/` exists (generated types/artifacts). `nuxt prepare` (postinstall) regenerates types; if types look stale, run `npm run postinstall`.
- Devtools enabled in `nuxt.config.ts`.
- No lint/test scripts defined in `package.json`.
