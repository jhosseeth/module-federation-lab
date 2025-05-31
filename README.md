# 🧪 Microfrontends Federation Lab

> A modern experimental architecture using **Module Federation** to integrate React-based microfrontends with both **Vite** and **Webpack** as build tools.

## 🎯 Purpose

This repository explores advanced frontend architecture by combining:
- 🧩 **Microfrontends** using React
- 🔗 **Module Federation** (Webpack 5 and [vite-plugin-federation](https://github.com/module-federation/vite))
- ⚡ High-performance builds with **Vite**
- 🏗️ Compatibility with **Webpack**

The goal is to build a set of independent micro-apps that:
- Share a single React version across all remotes and hosts
- Dynamically load components between applications
- Test both [OriginJS plugin](https://github.com/originjs/vite-plugin-federation) and the official [@module-federation/vite](https://github.com/module-federation/vite) implementation

---

## 🧱 Architecture

Each microfrontend is set up as an isolated application and uses:
- React + Vite OR Webpack
- Federated modules for shared components
- Version-aligned shared dependencies

This project demonstrates:
- Dynamic remote loading
- Shared state patterns
- Routing between federated apps
- Lazy loading React components across apps

---

## 🗂️ Structure

microfrontends-federation-lab/
├── host-app/ # Main shell hosting remotes
├── mfe-vite-a/ # Microfrontend A (Vite + React)
├── mfe-webpack-b/ # Microfrontend B (Webpack + React)
├── shared-ui/ # Shared federated components
├── README.md
