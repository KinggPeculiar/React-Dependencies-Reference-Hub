# 📚 React Dependencies Reference Hub

Welcome to the personal developer reference guide for React libraries and dependencies. This repository provides quick decision-making frameworks, usage templates, implementation examples, and debugging solutions for common packages across the React ecosystem.

## 🧭 Repository Structure

```
react-dependencies-docs/
├── README.md                  # Central Hub & Decision Matrix (You are here)
├── 01-routing/
│   ├── react-router.md
│   └── wouter.md
├── 02-state-management/
│   ├── zustand.md
│   ├── redux-toolkit.md
│   └── context-api.md
├── 03-data-fetching/
│   ├── tanstack-query.md
│   └── swr.md
├── 04-forms-validation/
│   ├── react-hook-form.md
│   └── zod.md
└── 05-ui-utilities/
    ├── framer-motion.md
    └── clsx-tailwind-merge.md

```

## ⚡ Quick Decision Matrix

Use this cheat sheet to quickly pick the right dependency for your project requirements:

| Category | Lightweight Pick | Full-Featured / Enterprise Pick | Key Decision Criterion | 
| ----- | ----- | ----- | ----- | 
| **Routing** | `wouter` (\~1.5 KB) | `react-router-dom` (\~11 KB) | Sub-2KB footprint vs. Built-in loaders/nested layout hierarchy | 
| **State Management** | `zustand` (\~1.2 KB) | `redux-toolkit` (\~13 KB) | Minimal boilerplate stores vs. Enterprise middleware & strict sync | 
| **Data Fetching** | `swr` (\~4 KB) | `tanstack-query` (\~13 KB) | Simple HTTP revalidation vs. Advanced mutations, offline cache & polling | 
| **Form Handling** | `react-hook-form` (\~9 KB) | `formik` (\~15 KB) | Uncontrolled high-performance inputs vs. Legacy component wrappers | 
| **Schema Validation** | `zod` (\~12 KB) | `yup` (\~15 KB) | Native TypeScript inference & ergonomics vs. Schema string matching | 
| **Class Merging** | `clsx` (\~0.4 KB) | `tailwind-merge` + `clsx` | Simple dynamic conditional classes vs. Resolving Tailwind conflicts | 

## 📑 Standard Document Template

Every dependency file in this repository follows this standard 5-part blueprint to ensure consistency and readability:

```
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

### ⚠️️ Common Gotchas & Solutions
- **Issue:** [Description]
  - **Fix:** [Solution]

```

## 🚀 How to Navigate

1. Consult the **Quick Decision Matrix** above when starting a project to pick the optimal library.

2. Navigate into the relevant category folder (e.g., `01-routing/`) to read deep-dive implementation guides.

3. Reference the **Common Gotchas & Solutions** section inside any package file when debugging runtime errors.
