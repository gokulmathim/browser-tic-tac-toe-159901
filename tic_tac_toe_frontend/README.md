# Astro Starter Kit: Minimal

```sh
npm create astro@latest -- --template minimal
```

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/withastro/astro/tree/latest/examples/minimal)
[![Open with CodeSandbox](https://assets.codesandbox.io/github/button-edit-lime.svg)](https://codesandbox.io/p/sandbox/github/withastro/astro/tree/latest/examples/minimal)
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/withastro/astro?devcontainer_path=.devcontainer/minimal/devcontainer.json)

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).

## 🎮 Tic Tac Toe App Notes

This project contains a minimal, self‑contained Tic Tac Toe game:
- 3×3 board with player turn indicator
- Win/draw detection with winning cell highlight
- Restart and New Game (alternates starting player) controls
- LocalStorage state persistence across reloads
- Optional theme toggle (light/dark), persisted in LocalStorage

### 🔧 Configuration via .env

Copy `.env.example` to `.env` and customize as needed:

- `PUBLIC_APP_TITLE`: Title text displayed in the page and document title. Default: `Tic Tac Toe`
- `PUBLIC_STARTING_PLAYER`: Initial starting player on first load. Valid values: `X` or `O`. Default: `X`
- `PUBLIC_PRIMARY_COLOR`: Primary color used for buttons and accents (hex or CSS color)
- `PUBLIC_SECONDARY_COLOR`: Secondary color used for hover and subtle accents
- `PUBLIC_ACCENT_COLOR`: Accent color for highlights (e.g., winning cells)

Note: Only `PUBLIC_*` variables are exposed to the client in Astro.

### 🌓 Theme

- Use the floating button to toggle light/dark theme.
- The selected theme is saved in `localStorage` and restored on next load.
- To prevent a flash during load, the theme class is applied early in the `<body>`.

