# 0x00. Webpack

This guide will walk you through setting up Webpack for a basic project, covering entry points, output, loaders, plugins, code splitting, and setting up a development server.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Loaders](#loaders)
- [Plugins](#plugins)
- [Code Splitting](#code-splitting)
- [Development Server](#development-server)

## Prerequisites

Before you start, make sure you have Node.js and npm (Node Package Manager) installed on your system. You can download them from the official website: [Node.js](https://nodejs.org/).

## Installation

1. Create a new directory for your project and navigate to it in your terminal:
```
 mkdir my-webpack-project
 cd my-webpack-project
```

2. Initialize a new npm project by running the following command and following the prompts:
```
npm init -y
```

3. Install Webpack and webpack-cli as dev dependencies:
```
npm install webpack webpack-cli --save-dev
```

4. Create a new file named index.html in the root of your project to serve as the entry point for your application.

## Loaders

Webpack uses loaders to process different file types during the bundling process. For example, to bundle JavaScript and CSS files, you can use respective loaders like `babel-loader` and `style-loader`.

Install necessary loaders using npm:
```
npm install babel-loader style-loader css-loader --save-dev
```

## Plugins

Webpack plugins are used to perform various tasks during the bundling process. For example, you can use the `HtmlWebpackPlugin` to automatically generate an HTML file and inject your bundled scripts into it.

## Code Splitting

Code splitting allows you to split your bundle into smaller chunks to improve loading performance. You can use dynamic imports to achieve this.

```
// src/index.js
document.getElementById('btn').addEventListener('click', () => {
  import('./lazy-loaded-module.js').then((module) => {
    // Use the module here
  });
});
```

## Development Server

To set up a development server, you can use `webpack-dev-server`.

Install `webpack-dev-server` using npm:
```
npm install webpack-dev-server --save-dev
```

---
