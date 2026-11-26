# showcase-angular-v16-platforms

> A multi-platform showcase collection of 10 enterprise Angular 16 applications spanning Progressive Web Apps (PWA), Electron desktop, Capacitor mobile, SSR, Scully SSG, and Nx NgRx monorepos.

**Inception (First Commit):** `2023-12-26` • **Batch / Horizon:** `batch-2023` • **Architecture Domain:** `Multi-Target Workspace / Angular 16, Ionic & PWA`

---

## 📌 Architecture & Overview

`angular-V16-projects` is an exhaustive enterprise showcase and architectural reference demonstrating the multi-platform capabilities of Angular 16. It collects 10 distinct, fully functional project implementations that explore different deployment targets, state management paradigms, and build tools.

The repository spans web, desktop, mobile, component packaging, and developer tooling:

```
angular-V16-projects/
├── 01_basic-app                   # Core Angular 16: Standalone components, signals & reactivity
├── 02_spa-ssg-blog                # Jamstack / SSG: Pre-rendered static blog engine via Scully
├── 03_issue-tracker               # Reactive Forms: Dynamic validation, form arrays & UI controls
├── 04_pwa-weather                 # PWA: Service Worker offline caching & Web App Manifest
├── 05_electron-editor             # Desktop Native: Cross-platform rich text editor via Electron
├── 06_mobile-phototag             # Mobile Hybrid: Capacitor runtime, native camera API & Ionic UI
├── 07_ssr-gh-portfolio            # Server-Side Rendering: Angular Universal with GitHub API
├── 08_nx-monorepo-ngrx-tour       # Enterprise Monorepo: Nx workspace with NgRx Store & Effects
├── 09_cdk-component               # Component Packaging: UI control library via ng-packagr & CDK
└── 10_cli-schematics              # Developer Tooling: Custom Angular CLI scaffolding schematics
```

* **Context:** Comprehensive multi-target architectural reference evaluating Angular 16 across desktop (Electron), mobile (Capacitor), serverless static sites (Scully), and enterprise monorepos (Nx + NgRx).
* **Key Patterns:**
  * **Standalone Component Architecture:** Modernizing Angular without `NgModule` boilerplate using standalone components and injected dependency functions.
  * **Cross-Platform Compilation:** Packaging identical TypeScript and HTML templates into native Electron binaries and Capacitor iOS/Android bundles.
  * **Offline-First Service Workers:** Progressive Web App caching strategies enabling offline functionality and background synchronization.
  * **Enterprise State Modeling:** Unidirectional data architecture using NgRx (Actions, Reducers, Effects, Selectors) inside an Nx monorepo.

---

## 🛠 Tech Stack

* **Framework & Core:** Angular 16.x (`@angular/core`, `@angular/common`, `@angular/forms`)
* **State Management:** NgRx 16 (`@ngrx/store`, `@ngrx/effects`, `@ngrx/entity`)
* **Monorepo & Build Tooling:** Nx Workspace, Angular CLI 16, `ng-packagr`, Scully SSG
* **Cross-Platform Runtimes:** Electron 25+, Capacitor 5+, Ionic 7+
* **Component Libraries:** Angular Material, Angular CDK, Tailwind CSS
* **Testing:** Karma, Jasmine, Jest, Cypress

---

## ✨ Features & Project Index

* **Desktop Application (`05_electron-editor`):** Electron IPC communication, native filesystem read/write dialogs.
* **Hybrid Mobile Application (`06_mobile-phototag`):** Native hardware access (Camera, Geolocation) orchestrated via Capacitor plugins.
* **PWA Weather Station (`04_pwa-weather`):** Offline asset caching, push notification hooks, and installable PWA manifest.
* **CLI Code Generator (`10_cli-schematics`):** Custom schematics automating component and service code generation via `ng generate`.

### Project Matrix & Deployment Targets

| Project | Target Runtime | Key Technologies | Architectural Pattern |
|---|---|---|---|
| `01_basic-app` | Web Browser | Standalone Components | Modern Standalone Angular |
| `02_spa-ssg-blog` | Static Hosting | Scully, Markdown | Static Site Generation (SSG) |
| `03_issue-tracker`| Web Browser | Reactive Forms, FormArray | Declarative Form Validation |
| `04_pwa-weather` | PWA / Mobile Web | `@angular/pwa`, Service Workers | Offline-First Cache |
| `05_electron-editor`| Desktop (Win/macOS/Linux) | Electron, Node.js IPC | Native Desktop Shell |
| `06_mobile-phototag`| iOS & Android | Capacitor, Ionic UI, Camera | Hybrid Mobile App |
| `07_ssr-gh-portfolio`| Node.js Server | Angular Universal, TransferState | Server-Side Rendering (SSR) |
| `08_nx-monorepo-ngrx-tour`| Enterprise Web | Nx, NgRx, Router Store | Redux Unidirectional Store |
| `09_cdk-component`| NPM Package | Angular CDK, `ng-packagr` | Shared UI Design System |
| `10_cli-schematics`| Angular CLI | `@angular-devkit/schematics` | Code Automation Tooling |

---

## 🚀 Getting Started

### Prerequisites

* Node.js `>= 18.14.0`
* Angular CLI 16 (`npm install -g @angular/cli@16`)
* Nx CLI (optional, `npm install -g nx`)

### Running Individual Projects

Each sub-directory operates as an autonomous project. Navigate into the desired directory to install dependencies and run:

```bash
# Clone the repository
git clone https://github.com/fabogit/showcase-angular-v16-platforms.git
cd showcase-angular-v16-platforms

# Example 1: Run PWA Weather application
cd 04_pwa-weather
npm install
npm start

# Example 2: Run Electron Desktop Text Editor
cd ../05_electron-editor
npm install
npm run electron:serve

# Example 3: Run Nx NgRx Tour application
cd ../08_nx-monorepo-ngrx-tour/packt
npm install
npx nx serve
```

---

## 📄 License & Author

Developed by [@fabogit](https://github.com/fabogit).
