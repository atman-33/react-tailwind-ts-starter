# React Tailwind CSS and TypeScript Starter

This is a starter project for building a web application using React with TypeScript and Tailwind CSS, powered by Vite.

## Features

- **React**: Fast and flexible UI library for building user interfaces. (v. 19)
- **TypeScript**: Strongly typed JavaScript for better development experience. (v. 5)
- **Tailwind CSS**: Utility-first CSS framework for rapid UI development. (v. 4)
- **Vite**: Lightning-fast build tool for modern web projects. (v. 7)
- **ESLint**: Linting for maintaining code quality. (v. 9)
- **Prettier**: Code formatting for consistent style. (v. 3)
- **Husky**: Git hooks for enforcing pre-push checks. (v. 9)
- **pnpm**: Package manager for managing dependencies. (v. 10)

## Prerequisites

1. Install [Node.js](https://nodejs.org/en/download) (LTS version recommended).
2. Enable Corepack to use a stable version of pnpm:

```sh
corepack enable pnpm
```

## Getting Started

1. Clone the repository:

```sh
git clone https://github.com/jhordyess/react-tailwind-ts-starter.git
```

2. Navigate to the project folder:

```sh
cd react-tailwind-ts-starter
```

3. Install dependencies:

```sh
pnpm i
```

4. Start the development server:

```sh
pnpm dev
```

5. Open your browser and visit [http://localhost:5173](http://localhost:5173) to see your project.

## Project Structure

```md
react-tailwind-ts-starter/
├── .gitignore              # List of files and directories to be ignored by version control.
├── .prettierrc.json        # Prettier configuration file.
├── eslint.config.js        # ESLint configuration file.
├── index.html              # Entry point HTML file.
├── package.json            # Project configuration and dependencies.
├── pnpm-lock.yaml          # pnpm lock file for dependency versions.
├── pnpm-workspace.yaml     # pnpm workspace configuration file.
├── README.md               # Project documentation.
├── tsconfig.app.json       # TypeScript configuration file for the application.
├── tsconfig.json           # TypeScript configuration file.
├── tsconfig.node.json      # TypeScript configuration file for Node.js.
├── vite.config.ts          # Vite configuration file.
├── .husky/                 # Directory for Git hooks managed by Husky.
│   ├── pre-push            # Pre-push hook to run linting and TypeScript checks.
├── src/
│   ├── App.tsx             # Main application component.
│   ├── index.css           # Global CSS file.
│   ├── main.tsx            # Main entry point of the application.
│   ├── vite-env.d.ts       # Vite types file.
```

## Commands

### Start the development server

```sh
pnpm dev
```

### Build the project for production

```sh
pnpm build
```

### Preview the project before production

```sh
pnpm start
```

### Run TypeScript checks

```sh
pnpm ts-check
```

### Lint the code

```sh
pnpm lint
```

### Validate the project (lint + TypeScript checks)

```sh
pnpm validate
```

### Format the code

```sh
pnpm format
```

## Contributing

Contributions are welcome! If you find any issues or want to enhance the project, feel free to submit a pull request.

---

Happy coding!
