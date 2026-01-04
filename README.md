# SPA Development Environment
A minimal scaffolding tool for building a Single Page Application (SPA) with a clear, fully controllable build pipeline.

This project favors simple, well-understood tools over opaque all‑in‑one frameworks, so you can understand *exactly* how your project is built and shipped.


## Features
- **Gulp**: Task runner for an explicit, readable build pipeline
- **Vue.js**: Reactive HTML templating without unnecessary abstractions
- **Rollup**: Efficient JavaScript bundling with incremental build support
- **Less**: CSS preprocessing with syntax close to vanilla CSS
- **BrowserSync**: Development server with live reload


## Getting Started
You don't need to `npm install` this package. Instead, just run:

```sh
npm init spade my_project
```

This command creates a new directory called `my_project` with the following structure:

- `package.json`: Preconfigured with all required `devDependencies`
- `gulpfile.js`: Predefined build and development tasks
- `src/`: Starter files for HTML, CSS, JavaScript, and Vue components

After the initialization:

```sh
cd my_project
npm install
npm run dev
```


## Why Gulp?
Unlike many modern build systems, Gulp gives you **full control** over your build process.

Its API is intentionally small and is based on straightforward file stream manipulation. This means:

- No proprietary configuration DSLs
- No hidden conventions
- No need to memorize framework‑specific magic

What you write is what runs.


## Why Vue.js?
Reactive HTML templates are genuinely useful, and Vue.js excels at this role without getting in your way.

- **Routing?** Use [Vue Router](https://router.vuejs.org/guide/)
- **Single File Components?** Fully supported and bundled by Rollup
- **State management?** Optional, add only what you actually need

Vue works pretty well as a *view layer*, nothing more, nothing less.


## Why Rollup?
Rollup produces clean, efficient bundles and integrates naturally with modern ES modules.

It focuses on JavaScript bundling and does that one job extremely well, which makes it a good match for a Gulp‑driven workflow.


## Why BrowserSync?
BrowserSync provides a lightweight development server with quality‑of‑life features:

- Built‑in HTTP server
- Automatic reload on file changes
- Scroll and interaction syncing across multiple devices, which makes it easier to debug on phone browsers

No additional backend is required during development.


## Why Less?
Less is designed to be largely compatible with standard CSS syntax, which keeps stylesheets readable and predictable.

Additional benefits:

- Minimal syntactic overhead compared to other preprocessors
- Written in JavaScript, so it runs directly in Node.js
- No extra native processes when used via Gulp

If you know CSS, you already know most of Less.


## Philosophy
This scaffold is intentionally **not** an all‑in‑one framework.

It is meant for developers who:

- Prefer transparent build pipelines
- Want to minimize vendor lock‑ins
- Value long‑term maintainability over trend‑driven tooling

Simple tools, composed carefully.

## License
MIT © 2026 [Satoshi Soma](https://github.com/amekusa)

