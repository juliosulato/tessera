<p align="center">
  <img src="docs/assets/logo.svg" height="60" alt="Tessera logo" />
</p>

<h1 align="center">Tessera</h1>
<p align="center">
  Your life, one piece at a time — an open-source, plugin-first personal management platform.
</p>

<p align="center">
  🚧 <strong>Early development</strong> · Live demo coming soon
</p>

---

## What is Tessera?

A *tessera* is a single tile in a mosaic. Tessera treats your personal life the same way:
finances, calendar, notes, workouts, diet — each one is a plugin, and you compose
only the pieces you actually use.

## Principles

- **Everything is a plugin.** Even the built-in modules can be disabled or replaced.
- **Your data, your machine.** Tessera is not a SaaS. Self-host it, or try the demo,
  which runs entirely in your browser (PGlite) — nothing leaves your device.
- **Built to be extended.** The goal is a plugin ecosystem simple enough for
  non-developers to install and use.

## Roadmap

- [ ] Core: plugin system & host app
- [ ] Plugin SDK
- [ ] 💰 Finance (first official plugin)
- [ ] 📅 Calendar
- [ ] 📝 Notes
- [ ] 🏋️ Workouts
- [ ] 🥗 Diet

## Tech stack

- **Monorepo:** Turborepo + pnpm workspaces
- **Language:** TypeScript (strict)
- **Demo database:** PGlite (Postgres running in the browser)

More to come as the core takes shape.

## Project structure

```
apps/       host applications (web app, demo)
packages/   core, plugin SDK and shared config
plugins/    official plugins — each one a tessera
```

## Development

Requires Node.js 20+.

```bash
corepack enable   # on Node 25+, run `npm install -g corepack` first
pnpm install
pnpm build
```

## Contributing

The project is in its early design phase. Ideas and discussions are welcome in
[Issues](https://github.com/juliosulato/tessera/issues).

## License

Copyright (C) 2026 Julio Cesar Sulato Filho

Tessera is licensed under the [GNU AGPL v3.0](LICENSE) (`AGPL-3.0-only`).
The plugin SDK (`packages/plugin-sdk`, coming soon) will be licensed under MIT,
so plugins can use any license their authors choose.