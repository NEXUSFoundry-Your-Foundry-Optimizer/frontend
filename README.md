# NEXUS-Foundry — Frontend
> **A Cross-Stage Cognitive Digital Twin & AI-Driven Analytics Ecosystem for Foundry Operations**

## 🌐 Live URLs & Quick Links

- **Live Production URL:** [https://frontend-kappa-nine-87.vercel.app/](https://frontend-kappa-nine-87.vercel.app/)
- **GitHub Repository:** [https://github.com/NEXUSFoundry-Your-Foundry-Optimizer/frontend.git](https://github.com/NEXUSFoundry-Your-Foundry-Optimizer/frontend.git)

---

## 📘 Comprehensive Platform Overview

### 1. The Industrial Problem
High-precision metal casting is one of the most physically demanding and thermally volatile manufacturing environments in modern heavy industry. Metal casting foundries encounter three deep-seated systemic bottlenecks:

1. **Catastrophic Furnace Lining Failures:** Induction furnace refractory linings erode invisibly beneath molten iron baths reaching temperatures in excess of 1500°C. Unplanned lining punctures or burn-throughs cause catastrophic downtime, safety hazards, and losses exceeding tens of lakhs per incident.
2. **Severely Delayed Defect Discovery:** Castings undergo hours of cooling, shakeout, shot blasting, and machining before non-destructive testing (NDT) or optical quality checks occur. By the time blowholes, gas porosity, cold shuts, or shrinkage defects are caught (typically **15+ hours after pouring**), hundreds of defective parts have already consumed non-recoverable electrical energy and labor.
3. **Loss of Tacit Diagnostic Expertise:** Foundry operations rely heavily on veteran metallurgists and senior furnace operators. As this workforce retires, their intuitive domain knowledge disappears, leaving newer crews without rapid diagnostic guidance during high-stress operational anomalies.

---

### 2. The NEXUS-Foundry Solution
**NEXUS-Foundry** is an end-to-end, predictive digital twin platform that replaces traditional post-mortem scrap reporting with proactive, physics-validated intervention across the **four fundamental stages** of foundry manufacturing:

```
[ Melting Twin ]  ───►  [ Molding Twin ]  ───►  [ Pouring Twin ]  ───►  [ Quality Twin ]
 (Induction Furnace)      (Green Sand Mold)       (Ladle & Flow)         (NDT / Inspection)
        │                       │                       │                       │
        ▼                       ▼                       ▼                       ▼
  LSTM-AE & TFT            Sand Kinetics           XGBoost + PINN          ResNet-50 + PCA
  Degradation (48h)       Compactability          Pre-Pour Risk           Defect Classifier
        └───────────────────────┴───────────────────────┴───────────────────────┘
                                                │
                                                ▼
                         [ Unified Operations Dashboard ]
                                                │
                                                ▼
                         [ Cognitive RAG Expert Assistant ]
```

### 3. The Closed-Loop Cyber-Physical Paradigm
NEXUS-Foundry operates as a **closed cyber-physical feedback loop**:
- **Physical Sensing:** Thermocouples, load cells, vibration accelerometers, infrared pyrometers, and optical cameras continuously stream real-time telemetry.
- **Stateful Digital Twins:** Independent, stateful digital replicas mirror physical furnace health, mold compactability, ladle thermal drop, and defect probabilities.
- **Cross-Stage Risk Propagation:** If the Melting Twin detects anomalous temperature spikes or lining thinning, it propagates early warning flags downstream to the Pouring Twin before the ladle is even tapped.
- **Physics-Informed Simulation:** Operators can run what-if simulations using Physics-Informed Neural Networks (PINN) governed by heat transfer equations before committing physical actions.
- **Operator Action:** Actionable recommendations and cited SOP guidance are surfaced via the real-time React dashboard and LLM cognitive assistant.

---

## 🖼️ Application Preview & Page Screenshots

> *Add your platform screenshots below or link them to your `/docs/screenshots/` folder.*

### 1. Landing Page & Hero Section
*Animated interactive 3D induction furnace preview, platform value propositions, problem statements, and four-stage foundry workflow.*

```markdown
![Landing Page & 3D Hero](https://via.placeholder.com/1280x720.png?text=NEXUS-Foundry+Landing+Page+%26+Interactive+3D+Hero)
```

---

### 2. Cross-Stage Digital Twins (Melting, Molding, Pouring, Quality)
*Stage-specific telemetry, live sensor gauges, 48-hour degradation curves, compactability envelopes, and ladle fill percentages.*

```markdown
![Digital Twins View](https://via.placeholder.com/1280x720.png?text=Digital+Twins+Live+State+%28Melting+%7C+Molding+%7C+Pouring+%7C+Quality%29)
```

---

### 3. Unified Real-Time Foundry Operations Dashboard
*Plant-wide operational KPIs, live sensor telemetry streams, cross-stage anomaly alerts, and active furnace operating states.*

```markdown
![Operations Dashboard](https://via.placeholder.com/1280x720.png?text=Foundry+Operations+Dashboard+%26+Live+Sensor+Streams)
```

---

### 4. Final Analytics & Defect Root-Cause Intelligence
*Multi-stage parameter correlation, SHAP feature attribution rankings, scrap reduction heatmaps, and defect classification distributions.*

```markdown
![Final Analytics](https://via.placeholder.com/1280x720.png?text=Predictive+Analytics+%26+SHAP+Defect+Attribution+Breakdown)
```

---

### 5. Cognitive RAG Assistant & PINN Simulation Studio
*Interactive domain assistant citing foundry SOPs and live twin states, alongside physics-constrained what-if simulation sliders.*

```markdown
![Cognitive Assistant & PINN](https://via.placeholder.com/1280x720.png?text=Cognitive+RAG+Assistant+%26+PINN+Simulation+Studio)
```

---

## ✨ Key Platform Features

- **Interactive 3D Factory Visualization:** Real-time Three.js / React Three Fiber renderers for the coreless induction furnace, sand mold cavities, and pouring ladles.
- **Sub-Second Anomaly Detection:** Visual indicators for LSTM Autoencoder reconstruction errors (threshold ~0.78) tracking furnace lining deterioration.
- **48-Hour Quantile Degradation Forecasting:** Multi-horizon P10, P50, and P90 forecast bands predicting lining failure hours ahead of time.
- **Cross-Stage Correlation Engine:** Visualized causality chains showing how upstream melt bath temperature deviations impact downstream mold gas porosity.
- **Explainable AI (XAI) Attribution:** SHAP bar charts highlighting exact feature contributions (sand moisture, pour speed, carbon equivalent) to defect probabilities.
- **Foundry Cognitive Assistant:** Natural-language conversational interface grounded in live sensor data, twin states, and foundry metallurgy SOP manuals.
- **Physics-Informed What-If Simulation:** Sliders to adjust pour temperature, ladle velocity, and mold moisture with instant PINN simulation results validated against thermal transfer physics.

---

## 🧭 Application Routes & Navigation

| Route | View Name | Description |
|---|---|---|
| `/` | **Landing Page** | Overview, interactive 3D hero model, foundry challenges, and stage walkthrough |
| `/dashboard` | **Operations Dashboard** | Plant-wide live telemetry, cross-stage status indicators, and operational alert feeds |
| `/twins/melting` | **Melting Twin** | Real-time melt temperature, power kW, coil vibration, lining health, and TFT forecasts |
| `/twins/molding` | **Molding Twin** | Green sand mold analytics: moisture %, permeability, green compression strength |
| `/twins/pouring` | **Pouring Twin** | Pour temperature, velocity, ladle fill percentage, and pre-pour defect risk estimation |
| `/twins/quality` | **Quality Twin** | Optical defect classification, ResNet-50 visual confidence, and defect distribution |
| `/analytics` | **Final Analytics** | SHAP feature rankings, scrap reduction trends, and multi-stage parameter correlations |
| `/agent/rag` | **Cognitive Assistant** | Multi-source RAG assistant referencing live twin state and standard operating procedures |
| `/agent/pinn` | **PINN Simulation** | Physics-informed what-if parameter modification with heat equation verification |

---

## 📦 Dependencies & System Prerequisites

### Minimum System Requirements
- **Node.js**: `v20.19.0` or `v22.12.0+` *(Required for Vite 8 and TanStack Start)*
- **Package Manager**: `npm` (v10+), `bun` (v1.3+), or `pnpm`
- **Hardware/Browser**: WebGL2-enabled browser for 3D factory visualizations (Chrome, Edge, Firefox, Brave, Safari)

### Primary Dependency Breakdown
```json
{
  "dependencies": {
    "react": "^19.2.0",
    "react-dom": "^19.2.0",
    "@tanstack/react-start": "1.168.32",
    "@tanstack/react-router": "1.170.18",
    "@tanstack/react-query": "^5.101.1",
    "@react-three/fiber": "^9.7.0",
    "@react-three/drei": "^10.7.8",
    "three": "^0.185.1",
    "tailwindcss": "^4.2.1",
    "@tailwindcss/vite": "^4.2.1",
    "recharts": "^2.15.4",
    "zustand": "^5.0.15",
    "lucide-react": "^0.575.0",
    "motion": "^13.2.0",
    "sonner": "^2.0.7",
    "clsx": "^2.1.1",
    "tailwind-merge": "^3.5.0"
  }
}
```

---

## 🚀 Local Development Setup

### 1. Clone the Repository
```bash
git clone https://github.com/NEXUSFoundry-Your-Foundry-Optimizer/frontend.git
cd frontend
```

### 2. Install Project Dependencies
```bash
npm install
```
*(Or if using Bun: `bun install`)*

### 3. Run the Development Server
```bash
npm run dev
```
Navigate to [http://localhost:8080](http://localhost:8080) to access the live development environment with Hot Module Replacement (HMR).

### 4. Production Build & Local Preview
```bash
npm run build
npm run preview
```


## 📂 Project Directory Structure

```text
pixel-perfect-revival-main/
├── public/                     # Static assets, 3D textures, favicons, manifests
├── src/
│   ├── components/             # Reusable UI component architecture
│   │   ├── common/             # Navbar, Footer, StatusPill, Shell Layouts
│   │   ├── 3d/                 # Three.js 3D visualizers (Furnace, Sand Mold, Ladle)
│   │   ├── charts/             # Real-time sensor charts, TFT bands, SHAP plots
│   │   └── ui/                 # Radix UI and shadcn styled UI primitives
│   ├── hooks/                  # Custom React hooks (real-time timers, sensor polling)
│   ├── lib/                    # Helper utilities, class name merge helpers (cn)
│   ├── routes/                 # TanStack Start file-system route tree
│   │   ├── __root.tsx          # Root layout shell with navigation and toast provider
│   │   ├── index.tsx           # Landing Page with 3D furnace hero
│   │   ├── dashboard.tsx       # Plant-wide operations dashboard
│   │   ├── analytics.tsx       # Predictive analytics & SHAP defect attribution
│   │   ├── twins/
│   │   │   └── $twin.tsx       # Dynamic twin route (Melting, Molding, Pouring, Quality)
│   │   └── agent/
│   │       ├── index.tsx       # Agent hub overview
│   │       ├── rag.tsx         # Cognitive RAG assistant interface
│   │       └── pinn.tsx        # Physics-informed simulation studio
│   ├── store/                  # Zustand client stores for simulation & twin states
│   ├── styles.css              # Tailwind CSS v4 design tokens and industrial styling
│   ├── server.ts               # Nitro SSR server entry point & error handler
│   ├── start.ts                # TanStack Start client bootstrapping
│   └── router.tsx              # Router instantiation with route tree
├── components.json             # shadcn/ui configuration
├── package.json                # Project dependencies, scripts, and overrides
├── tsconfig.json               # TypeScript configuration with path aliases
└── vite.config.ts              # Vite + TanStack Start configuration
```




## 💻 Tech Stack & Usage Architecture

The frontend architecture uses a modern, high-performance web stack tailored for industrial dashboards and real-time 3D telemetry:

```
┌────────────────────────────────────────────────────────────────────────┐
│                          PRESENTATION LAYER                            │
│  React 19  •  Tailwind CSS v4  •  Radix UI  •  Motion  •  Lucide Icons │
├────────────────────────────────────────────────────────────────────────┤
│                     3D GRAPHICS & VISUALIZATION                        │
│         Three.js  •  React Three Fiber (R3F)  •  Drei  •  Recharts     │
├────────────────────────────────────────────────────────────────────────┤
│                       DATA & STATE MANAGEMENT                          │
│          TanStack Query  •  Zustand  •  Zod  •  React Hook Form        │
├────────────────────────────────────────────────────────────────────────┤
│                        ROUTING & RUNTIME ENGINE                        │
│          TanStack Start  •  TanStack Router  •  Vite 8  •  Nitro       │
└────────────────────────────────────────────────────────────────────────┘
```

---



[![Vercel Deployment](https://img.shields.io/badge/Deployed%20on-Vercel-black?style=for-the-badge&logo=vercel)](https://frontend-kappa-nine-87.vercel.app/)
[![GitHub Repository](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github)](https://github.com/NEXUSFoundry-Your-Foundry-Optimizer/frontend.git)
[![React 19](https://img.shields.io/badge/React-19.2.0-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.8.3-3178C6?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-8.1.5-646CFF?style=for-the-badge&logo=vite)](https://vitejs.dev/)
[![Tailwind CSS v4](https://img.shields.io/badge/Tailwind_CSS-v4.2-38B2AC?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com/)
[![Three.js](https://img.shields.io/badge/Three.js-3D_WebGL-000000?style=for-the-badge&logo=three.js)](https://threejs.org/)

---

### Detailed Technology & Exact Usage Breakdown

| Category | Technology | Version | Exact Usage in NEXUS-Foundry |
|---|---|---|---|
| **Core Framework** | **React** | `19.2.0` | Powers the reactive UI, component lifecycles, and concurrent rendering for smooth real-time telemetry updates. |
| **Language** | **TypeScript** | `5.8.3` | Enforces strict end-to-end type safety across twin state payloads, sensor metrics, and simulation parameters. |
| **SSR & Meta-Framework** | **TanStack Start** | `1.168.32` | Provides server-side rendering (SSR), initial page state hydration, and eliminates client-side request waterfalls. |
| **Routing System** | **TanStack Router** | `1.170.18` | Type-safe, file-system-based routing managing transitions between Twins, Dashboards, and Simulation pages. |
| **Bundler & Build Tool** | **Vite** | `8.1.5` | Next-generation fast frontend bundler delivering instant Hot Module Replacement (HMR) during development. |
| **Server Engine** | **Nitro** | `3.0.x` | Universal deployment engine compiling portable server output for Vercel Serverless / Cloudflare / Node runtimes. |
| **Styling & Design System** | **Tailwind CSS** | `4.2.1` | Modern utility-first CSS framework establishing the dark industrial foundry aesthetic, glassmorphism, and responsive grids. |
| **3D Rendering Engine** | **Three.js** | `0.185.1` | WebGL engine powering the realistic 3D renderings of the induction melting furnace, sand molds, and molten metal flows. |
| **React 3D Integration** | **React Three Fiber** | `9.7.0` | Declarative React wrapper for Three.js allowing 3D models to react dynamically to twin temperature and vibration props. |
| **3D Helpers & Controls** | **@react-three/drei** | `10.7.8` | Supplies camera controls, lighting setups, environment maps, and stage controls for the 3D factory viewports. |
| **Time-Series Charts** | **Recharts** | `2.15.4` | Renders multi-stream live sensor graphs, TFT 48-hour quantile forecast envelopes (P10/P50/P90), and SHAP attribution bars. |
| **Server State Caching** | **TanStack Query** | `5.101.1` | Manages asynchronous REST fetching, background polling, automatic re-validation, and caching for twin endpoints. |
| **Global Client State** | **Zustand** | `5.0.15` | Lightweight store managing operator simulation slider overrides, filter selections, and active twin inspection states. |
| **Micro-Animations** | **Motion** | `13.2.0` | Fluid entrance transitions, collapsible telemetry cards, live state changes, and smooth page navigation animations. |
| **Component Primitives** | **Radix UI** | Latest | Unstyled, accessible UI primitives for dropdowns, modals, tabs, sliders, tooltips, and collapsible sidebars. |
| **Iconography** | **Lucide React** | `0.575.0` | Industrial iconography covering temperature gauges, sensors, flame icons, warnings, and navigation markers. |
| **Notifications & Toasts** | **Sonner** | `2.0.7` | High-priority toast notifications alerting operators of anomaly triggers, risk thresholds, and completed simulations. |
| **Form Management** | **React Hook Form + Zod** | `7.71 / 3.24` | Validates operator input fields, what-if simulation parameters, and user profile updates against schema definitions. |

---

## 👥 Frontend Contributors & Core Team

The NEXUS-Foundry frontend application is designed, built, and maintained by:

- **Kanishthika** — *Frontend Lead, Architecture & 3D Visualizations*
- **Pom Gopika** — *Frontend Engineering & UI Component Integration*
- **NEXUS-Foundry Frontend Contributors** ([@NEXUSFoundry-Your-Foundry-Optimizer](https://github.com/NEXUSFoundry-Your-Foundry-Optimizer))

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
