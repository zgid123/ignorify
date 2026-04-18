# git-ignore

A lightweight CLI to generate `.gitignore` from selected tech-stack templates.

## Install

```bash
npm install -g git-ignore
```

## Usage

Run:

```bash
git-ignore init
```

The CLI will show an interactive list of tech stacks.  
After you choose, it generates a `.gitignore` file in your current directory.

## Output Format

The generated file is grouped by selected tech stack:

```gitignore
#
# TechStack: Node.js
#
node_modules
.env
```

## Development Mode

Set `GIT_IGNORE_DEV=true` to use local templates from `templates/` instead of fetching from GitHub.

In development mode:
- output file is `.gitignore-local`
- template source is local files under `templates/`

Run locally:

```bash
pnpm local:run init
```

## Available Tech Stacks

- Node.js
- OSX
- TypeScript
- Vitest

## Development

```bash
pnpm install
pnpm build
pnpm test
```

## License

MIT
