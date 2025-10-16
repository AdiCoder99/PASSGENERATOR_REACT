## Password Generator (React + Vite)

Small, single-page React app that generates secure passwords with configurable options. Built with Vite for fast development and HMR.

## Highlights

- Generate random passwords with options for length and character sets (uppercase, lowercase, numbers, symbols).
- Copy generated password to clipboard with one click.
- Minimal, responsive UI built with Tailwind CSS (see `vite.config.js` and `src/index.css`).

## Requirements

- Node.js 14+ (Node 16+ recommended)
- npm (or yarn)

## Quick start (dev)

Open a PowerShell terminal in the project root and run:

```powershell
npm install
npm run dev
```

Vite starts a dev server (default http://localhost:5173). Follow the terminal output if a different port is used.

## Build and preview (production)

```powershell
npm run build
npm run preview
```

## Project structure

- `index.html` — App entry point
- `src/` — React source files
	- `main.jsx` — React mount and router (if present)
	- `App.jsx` — Main application component (password generator UI)
	- `App.css`, `index.css` — Styles
	- `assets/` — Images/icons
- `public/` — Static public files
- `package.json` — Scripts and dependencies
- `vite.config.js` — Vite configuration

## Available scripts (from `package.json`)

- `npm run dev` — Start development server with fast refresh
- `npm run build` — Create a production build in `dist/`
- `npm run preview` — Serve the production build locally

## Usage notes

- Adjust password length and character sets in the UI and click "Generate".
- Use the copy button to copy the password to clipboard; browsers may prompt for clipboard permissions.

## Troubleshooting

- If `npm install` fails, ensure Node.js is installed and try clearing the npm cache:

```powershell
npm cache clean --force
npm install
```

- If Vite fails to start because of a port conflict, it will suggest an alternate port — open the one shown in the terminal.
- If the UI doesn't update on save, ensure the dev server is running and that HMR is enabled in `vite.config.js`.

## Testing & linting

This project doesn't include automated tests by default. To add tests, consider installing Jest or Vitest and add a basic test runner.

## Contributing

Contributions are welcome. Prefer small, focused pull requests. Add tests for new behavior where possible.

## License

This project is licensed under the MIT License. 

---

