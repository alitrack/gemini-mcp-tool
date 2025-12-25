# GEMINI.md

## Project Overview

This project is a Model Context Protocol (MCP) server that integrates the Gemini CLI with AI assistants. It allows the assistant to leverage Gemini's capabilities for tasks like code analysis, searching, and running code in a sandbox.

The project is a Node.js application written in TypeScript. It uses the `@modelcontextprotocol/sdk` to create an MCP server that communicates with the AI assistant over standard I/O.

The server exposes several tools to the AI assistant, including:
*   `ask-gemini`: To ask questions to Gemini.
*   `sandbox-test`: To run code in a sandboxed environment.
*   `Ping`: A simple test tool.
*   `Help`: To show the Gemini CLI help text.

## Building and Running

### Prerequisites

*   Node.js (v16.0.0 or higher)
*   npm

### Installation

Install the dependencies using npm:
```bash
npm install
```

### Building

To compile the TypeScript code, run the following command:
```bash
npm run build
```
This will create a `dist` directory with the compiled JavaScript files.

### Running

To run the server, use the following command:
```bash
npm start
```
This will start the MCP server, which will listen for requests on standard I/O.

### Development

For development, you can use the `dev` script, which will compile the code and then run the server:
```bash
npm run dev
```

## Development Conventions

### Linting

The project uses the TypeScript compiler for linting. To check for any type errors, run:
```bash
npm run lint
```

### Testing

There are currently no tests for this project. The `test` script is a placeholder:
```bash
npm test
```

### Code Style

The codebase is written in TypeScript and follows standard TypeScript conventions. It uses ES modules (`"type": "module"` in `package.json`).
The code is organized into several directories:
*   `src/tools`: Contains the definitions of the tools exposed by the server.
*   `src/utils`: Contains utility functions for logging, command execution, etc.
*   `src/scripts`: Contains scripts for the project.
*   `src/constants.ts`: Contains the project's constants.

### Contribution

The `README.md` file mentions a `CONTRIBUTING.md` file, which should be consulted for contribution guidelines.
