# 📚 React Dependencies Reference Hub

Welcome to the personal developer reference guide for React libraries and dependencies. This repository provides quick decision-making frameworks, usage templates, implementation examples, and debugging solutions for common packages across the React ecosystem.

## 🧭 Repository Structure

```text
react-dependencies-docs/
├── README.md                         # Central Hub & Decision Matrix (You are here)
├── 01-routing/
│   ├── react-router.md
│   ├── tanstack-router.md
│   └── wouter.md
├── 02-state-management/
│   ├── zustand.md
│   ├── jotai.md
│   ├── redux-toolkit.md
│   └── xstate.md
├── 03-data-fetching/
│   ├── tanstack-query.md
│   ├── swr.md
│   └── trpc.md
├── 04-form-management/
│   ├── react-hook-form.md
│   └── tanstack-form.md
├── 05-schema-validation/
│   ├── zod.md
│   └── valibot.md
├── 06-ui-components/
│   ├── shadcn-ui.md
│   ├── mui.md
│   └── mantine.md
├── 07-headless-primitives/
│   ├── radix-ui.md
│   └── react-aria.md
├── 08-styling-css/
│   ├── tailwindcss.md
│   └── styled-components.md
├── 09-animation-motion/
│   ├── framer-motion.md
│   └── auto-animate.md
├── 10-data-visualization/
│   ├── recharts.md
│   └── visx.md
├── 11-rich-text-editors/
│   ├── tiptap.md
│   └── lexical.md
├── 12-testing-qa/
│   ├── vitest-rtl.md
│   └── playwright.md
├── 13-internationalization/
│   ├── react-i18next.md
│   └── next-intl.md
├── 14-3d-canvas-media/
│   ├── react-three-fiber.md
│   └── xyflow.md
├── 15-authentication/
│   ├── auth-js.md
│   └── clerk.md
└── 16-utilities-helpers/
    ├── clsx-tailwind-merge.md
    └── tanstack-table.md
```

## ⚡ Quick Decision Matrix

Use this cheat sheet to quickly pick the right dependency for your project requirements:

| Category | Lightweight Pick | Full-Featured / Enterprise Pick | Key Decision Criterion |
| ----- | ----- | ----- | ----- |
| **Routing** | `wouter` (\~1.5 KB) | `react-router` (\~11 KB) / `tanstack-router` (\~12 KB) | Sub-2KB footprint vs. Type-safe search params, nested layouts & SSR loaders |
| **State Management** | `zustand` (\~1.2 KB) / `jotai` (\~3 KB) | `redux-toolkit` (\~13 KB) / `xstate` (\~15 KB) | Minimal boilerplate stores or atomic state vs. Redux middleware & complex statecharts |
| **Data Fetching** | `swr` (\~4 KB) | `tanstack-query` (\~13 KB) / `apollo-client` | Simple HTTP revalidation vs. Advanced optimistic updates, offline cache & polling |
| **Form Management** | `react-hook-form` (\~9 KB) | `tanstack-form` (\~11 KB) / `formik` (\~15 KB) | Uncontrolled high-performance inputs vs. Headless multi-framework form state |
| **Schema Validation** | `valibot` (\~1 KB) / `zod` (\~12 KB) | `yup` (\~15 KB) | Modular tree-shakable schemas / TS inference vs. Legacy object validations |
| **UI Components** | `shadcn/ui` (0 KB - copy/paste) | `mui` (\~80+ KB) / `mantine` (\~40 KB) | Customizable Tailwind components vs. Turnkey pre-built design systems |
| **Headless Primitives** | `radix-ui` (\~2-5 KB/comp) | `react-aria` (\~15 KB) | Accessible unstyled primitives vs. Adobe cross-device accessibility hooks |
| **Styling & CSS** | `tailwindcss` (0 KB runtime) | `styled-components` (\~12 KB) / `emotion` (\~11 KB) | Utility-first compile-time CSS vs. Dynamic runtime CSS-in-JS |
| **Animation & Motion** | `auto-animate` (\~2.3 KB) | `framer-motion` (\~30 KB) / `gsap` (\~25 KB) | Zero-config DOM list transitions vs. Physics-based gestures & timeline sequencing |
| **Data Visualization** | `recharts` (\~45 KB) / `tremor` | `visx` (modular) / `nivo` | Declarative composite chart components vs. Low-level D3 React primitives |
| **Rich Text Editors** | `tiptap` (\~35 KB) | `lexical` (\~25 KB) / `slate` (\~30 KB) | Headless ProseMirror wrapper vs. Extensible Meta text editor engine |
| **Testing & QA** | `vitest` + `react-testing-library` | `playwright` / `cypress` | Fast unit/component interaction testing vs. Full end-to-end browser automation |
| **Internationalization** | `paraglide-js` (\~1.5 KB) | `react-i18next` (\~8 KB) / `next-intl` | Compile-time tree-shakable translations vs. Ecosystem-standard i18n runtime |
| **3D & Canvas** | `react-konva` (\~25 KB) | `react-three-fiber` (\~20 KB + Three.js) / `xyflow` | 2D canvas drawing vs. Declarative 3D WebGL scenes & node graphs |
| **Authentication** | `lucia` (\~3 KB) | `next-auth` (Auth.js) / `clerk` | Self-hosted session handler vs. Turnkey managed user management SDKs |
| **Class Merging** | `clsx` (\~0.4 KB) | `tailwind-merge` + `clsx` (\~3.5 KB) | Simple dynamic conditional classes vs. Resolving conflicting Tailwind utility classes |
| **Tables & Grids** | `react-table` (legacy) | `tanstack-table` (\~14 KB) | Basic HTML tables vs. Headless sorting, filtering, pagination & virtualization |
| **Meta-Frameworks** | `astro` (0 KB JS default) | `next.js` / `react-router` (framework mode) | Content-first Islands Architecture vs. Full-stack hybrid SSR/RSC application frameworks |

## 📑 Standard Document Template

Every dependency file in this repository follows this standard 5-part blueprint to ensure consistency and readability:

```markdown
# [Package Name]

- **Category:** [Category]
- **Bundle Size:** [X] KB (gzipped)
- **Primary Alternative(s):** [Package A], [Package B]

---

### 🎯 Primary Use Cases (When to Use)
- [Use Case 1]
- [Use Case 2]

### ⛔ When NOT to Use / Trade-offs
- **Avoid if:** [Scenario]
- **Downsides:** [Drawback]

### ⚡ Quick Setup & Minimal Pattern
\`\`\`jsx
// Minimal working code example
\`\`\`

### ⚠ Common Gotchas & Solutions
- **Issue:** [Description]
  - **Fix:** [Solution]
```

## 🚀 How to Navigate

1. Consult the **Quick Decision Matrix** above when starting a project to pick the optimal library.

2. Navigate into the relevant category folder (e.g., `01-routing/` or `03-data-fetching/`) to read deep-dive implementation guides.

3. Reference the **Common Gotchas & Solutions** section inside any package file when debugging runtime errors.
