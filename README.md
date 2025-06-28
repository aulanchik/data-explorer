# Data Explorer

This repository contains a foundational front-end application for exploring data, built with React, TypeScript, and Vite.
It is designed to serve as a starting point for visualizing and interacting with datasets, and includes a sample dataset of applications with associated spending and business capabilities.
Main goal of this project is to test react memoization and react context API capabilities.

## Tech Stack
- **Framework:** React 18
- **Language:** TypeScript
- **Build Tool:** Vite
- **Styling:** Sass (setup)
- **Linting:** ESLint
- **Formatting:** Prettier

## Project Structure

The project follows a standard Vite/React structure. Key files and directories include:

```
data-explorer/
├── src/
│   ├── data/
│   │   └── applications.json # Sample application dataset
│   ├── App.tsx            # Main application component
│   └── main.tsx           # React application entry point
├── package.json           # Project dependencies and scripts
├── tsconfig.json          # TypeScript compiler options
└── vite.config.ts         # Vite configuration
```

## Data Model

The application uses a sample dataset located at `src/data/applications.json`. The data is an array of objects, where each object represents an application with the following structure:

```json
{
  "id": "app-1",
  "name": "Application 1",
  "spend": 29822,
  "BCAP1": "Business Capability 1",
  "BCAP2": "Business Capability 1.2",
  "BCAP3": "Business Capability 1.2.3"
}
```

- **`id`**: A unique identifier for the application.
- **`name`**: The display name of the application.
- **`spend`**: A numerical value representing application spend.
- **`BCAP1`, `BCAP2`, `BCAP3`**: A hierarchical representation of the application's business capability.

## Getting Started

To get the project running on your local machine, follow these steps.

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or newer)
- [npm](https://www.npmjs.com/) (included with Node.js) or [yarn](https://yarnpkg.com/)

### Installation & Setup

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/aulanchik/data-explorer.git
    ```

2.  **Navigate to the project directory:**
    ```sh
    cd data-explorer
    ```

3.  **Install dependencies:**
    ```sh
    npm install
    ```

## Available Scripts

In the project directory, you can run the following commands:

### `npm run dev`

Runs the app in development mode. Open [http://localhost:5173](http://localhost:5173) (or the port specified in your terminal) to view it in the browser. The page will reload if you make edits.

### `npm run build`

Builds the app for production to the `dist` folder. It correctly bundles React in production mode and optimizes the build for the best performance.

### `npm run lint`

Lints the project's source files using ESLint to check for code quality and style issues.

### `npm run preview`

Starts a local static web server that serves the files from the `dist` directory. This is useful for previewing the production build before deployment.
