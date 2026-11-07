---
title: User-Facing Tools
sidebar_position: 4
description: Overview of the tscircuit CLI, Registry, Dev Server, React Fiber Renderer, and Web Viewers.
---

# tscircuit User-Facing Tools

tscircuit provides a suite of developer tools for designing, previewing, testing, and sharing electronic circuits using React and TypeScript.

## 1. `@tscircuit/cli` (`tsci`)

The **tscircuit CLI** (`tsci`) is the command-line tool for creating, developing, building, and publishing tscircuit projects and packages.

- `tsci init` — Scaffolds a new tscircuit project with TypeScript and circuit preview configuration.
- `tsci dev` — Launches the local development server with live schematic, PCB, and 3D previews.
- `tsci build` — Compiles your circuit into Circuit JSON, Gerber files, and fabrication outputs.
- `tsci publish` — Publishes reusable circuit footprints and modules to the tscircuit Registry.

## 2. Dev Server (`@tscircuit/cli` / `@tscircuit/runframe`)

The **Dev Server** watches your local `.tsx` circuit files, evaluates changes in real time, and serves an interactive browser environment where you can inspect schematics, PCB layouts, 3D views, and DRC errors side by side.

## 3. tscircuit Registry (`tscircuit.com`)

The **tscircuit Registry** (hosted at [tscircuit.com](https://tscircuit.com)) is the package registry and online playground for sharing and discovering reusable subcircuits, footprints, and component models:

- Import published circuits directly via `tsci add @tsci/<author>.<package>`.
- Edit, fork, and preview circuits directly in the browser without local setup.

## 4. `@tscircuit/core` (React Fiber Renderer)

`@tscircuit/core` provides the custom React reconciler (`RootCircuit` / `Circuit`) that renders JSX circuit elements (`<board>`, `<resistor>`, `<capacitor>`, `<chip>`, `<trace>`) into standardized **Circuit JSON** (`@tscircuit/soup`), executing autorouting and design rule checks automatically.

## 5. Interactive Viewers (`@tscircuit/schematic-viewer`, `@tscircuit/pcb-viewer`, `@tscircuit/3d-viewer`)

tscircuit provides standalone React viewer components that render Circuit JSON in any web application:

- **`@tscircuit/schematic-viewer`** — Interactive pan-and-zoom schematic diagram viewer.
- **`@tscircuit/pcb-viewer`** — Multi-layer 2D PCB layout, pad, silkscreen, and trace viewer.
- **`@tscircuit/3d-viewer`** — 3D CAD board and component model viewer powered by Three.js / JSCAD.
