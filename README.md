# Custom Profiles for VS Code & Google Cloud Workstations (Code-OSS)

A curated collection of custom **Visual Studio Code (VS Code)** and **Code-OSS** profiles designed to tailor the IDE experience on **Google Cloud Workstations** (and local environments) for diverse roles beyond traditional software engineering.

---

## Overview & Vision

While **Google Cloud Workstations** (powered by **Code-OSS** by default) and **VS Code** are widely known as developer tools, their secure, pre-configured cloud environments, AI agents, and built-in browser capabilities make them powerful workspaces for the entire organization.

However, a default developer IDE can feel overwhelming to non-engineering roles due to complex toolbars, debugging panels, Git indicators, and code-centric popups.

**The goal of this repository** is to expand the reach of Google Cloud Workstations and VS Code by providing ready-to-use, role-specific `.code-profile` configurations that adapt the workspace, extensions, and UI layout to match how different personas work:

- **Business Analysts & Data Explorers** — Clean workspaces focused on AI-assisted analysis, reporting, and task automation without code clutter.
- **Product Owners & Product Managers** — Streamlined environments for rapid web app prototyping, reviewing live previews with the built-in browser, and collaborating with AI agents.
- **QA & Testers** — Focused layouts for running, inspecting, and validating applications and automated test workflows.
- **Non-Developers & Citizen Automators** — Simplified, distraction-free interfaces that put natural-language AI agents front and center.

---

## Available Profiles

| Profile | Target Personas | Description |
| :--- | :--- | :--- |
| **[Google Antigravity for Non-Developers & Business Users](./google-antigravity-non-developers-users/)** | Business Users, Product Owners, Analysts, Non-Developers | Simplifies the IDE by hiding developer-focused UI elements, automatically focusing the **Google Antigravity** agent chat, and enabling the built-in browser in the title bar for task automation and live web app prototyping. |

> *More role-specific profiles (e.g., for QA/Testers, Product Owners, Data Analysts, and specialized workflows) will be added to this repository over time.*

---

## How to Use a Profile

Every profile in this repository is packaged as a standard `.code-profile` file that works in both **Code-OSS on Google Cloud Workstations** and **Visual Studio Code**.

### Quick Import Steps

1. Browse the [Available Profiles](#available-profiles) table above and download the `.code-profile` file from the profile's folder.
2. Open **Code-OSS** (on your Google Cloud Workstation) or **VS Code**.
3. Click the **Manage** gear icon (⚙️) in the bottom-left corner → **Profiles** (or run **Profiles: Import Profile...** from the Command Palette via `Cmd+Shift+P` / `Ctrl+Shift+P`).
4. Select **Import Profile...**, choose the downloaded `.code-profile` file, and click **Create**.

Each profile folder includes its own `README.md` with screenshots and detailed information about the extensions, settings, and UI customizations included.

---

## Repository Structure

Each profile lives in its own dedicated directory containing the exported `.code-profile` file, documentation, and preview screenshots:

```text
vscode-profiles/
├── google-antigravity-non-developers-users/
│   ├── antigravity-non-developers.code-profile
│   ├── images/
│   └── README.md
└── README.md
```

---

## Contributing New Profiles

To add a new role-specific profile to this repository:

1. Configure and test the layout, extensions, and settings in **VS Code** or **Code-OSS**.
2. Export the profile via **Profiles: Export Profile...** as a `.code-profile` file.
3. Create a new folder named after the target role or workflow, include a screenshot in an `images/` subfolder, and document its purpose and customizations in a local `README.md`.
4. Add the new profile to the [Available Profiles](#available-profiles) table in this root `README.md`.
