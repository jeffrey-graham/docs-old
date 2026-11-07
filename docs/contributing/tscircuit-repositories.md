---
title: tscircuit Repositories for Contributors
sidebar_position: 1
---

# Contributing to tscircuit Repositories

The tscircuit ecosystem is modular and split across specialized open-source repositories. Below is a guide to the primary repositories where you can contribute and claim bounties.

## Core & Compiler

| Repository | Description |
| --- | --- |
| [`tscircuit/core`](https://github.com/tscircuit/core) | Core React reconciler and circuit JSON generator that turns `<board>`, `<chip>`, `<resistor>`, and `<trace>` into Circuit JSON. |
| [`tscircuit/circuit-json`](https://github.com/tscircuit/circuit-json) | TypeScript definitions and Zod schemas for the Intermediate Representation (`AnyCircuitElement`) shared across all tools. |
| [`tscircuit/props`](https://github.com/tscircuit/props) | Prop types and Zod validators for all tscircuit JSX components. |
| [`tscircuit/eval`](https://github.com/tscircuit/eval) | Sandboxed execution runtime for evaluating tscircuit TSX snippets in the browser and CLI. |

## Viewers & UI

| Repository | Description |
| --- | --- |
| [`tscircuit/pcb-viewer`](https://github.com/tscircuit/pcb-viewer) | 2D interactive PCB layout viewer built with React, Canvas, and WebGPU. |
| [`tscircuit/schematic-viewer`](https://github.com/tscircuit/schematic-viewer) | Interactive schematic diagram renderer for Circuit JSON. |
| [`tscircuit/3d-viewer`](https://github.com/tscircuit/3d-viewer) | Three.js 3D PCB and CAD model viewer (` CadViewer `). |
| [`tscircuit/runframe`](https://github.com/tscircuit/runframe) | Unified embeddable UI frame combining PCB, Schematic, 3D, BOM, and Error tabs. |

## CLI, Footprints & Converters

| Repository | Description |
| --- | --- |
| [`tscircuit/cli`](https://github.com/tscircuit/cli) | Command-line tool (`tsci`) for developing, building, testing, and publishing tscircuit packages. |
| [`tscircuit/footprinter`](https://github.com/tscircuit/footprinter) | Parametric footprint generator (`0402`, `soic8`, `qfp32`, etc.) from string definitions. |
| [`tscircuit/dsn-converter`](https://github.com/tscircuit/dsn-converter) | Converts Circuit JSON to/from Specctra DSN/SES files for autorouting. |
| [`tscircuit/circuit-to-svg`](https://github.com/tscircuit/circuit-to-svg) | Converts PCB and Schematic Circuit JSON into static SVG images. |
