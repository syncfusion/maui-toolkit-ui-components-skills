# maui-toolkit-ui-components-skills

Skills for Syncfusion® Toolkit for .NET MAUI components, designed for use with AI coding assistants.

This repository contains 35 AI-ready skill guides for working with Syncfusion® Toolkit for .NET MAUI controls. Each skill includes a `SKILL.md` file that AI coding assistants can read automatically, plus a `references/` subfolder with detailed documentation covering setup, usage patterns, customization, and troubleshooting.

## Quick Start

### Option 1: Using npx (Recommended)

```bash
npx skills add https://github.com/syncfusion/maui-toolkit-ui-components-skills
```

This will automatically add the skills to your workspace.

### Option 2: Manual Installation

**1. Clone this repository**
```bash
git clone https://github.com/syncfusion/maui-toolkit-ui-components-skills.git
```

**2. Add it to your VS Code workspace**

Open your `.code-workspace` file (or create one) and add this repo as a second root folder:
```json
{
  "folders": [
    { "path": "/path/to/your-maui-app" },
    { "path": "/path/to/maui-toolkit-ui-components-skills" }
  ]
}
```

**3. Start asking questions**

Your AI assistant will automatically detect and apply the relevant skill based on your prompt:
```text
How do I allow users to pick dates or highlight important days?
How do I present information in a clean, modern card layout?
How do I apply a dark theme to Syncfusion controls?
```

No configuration required. Skills are loaded automatically from the workspace.

---

## Prerequisites

- An AI coding assistant that supports skills/context files (e.g., GitHub Copilot, Cursor, or similar tools)
- [.NET 9 SDK](https://dotnet.microsoft.com/download/dotnet/9.0)

## How These Skills Work

Each `SKILL.md` file contains a `description` field in its YAML frontmatter. AI coding assistants read this description to decide when to automatically apply a skill during a conversation. When you ask about a specific Syncfusion control — for example, "How do I add items to my SegmentedControl?" — the AI assistant detects the match and loads the corresponding skill to guide its response.

You can also reference a skill explicitly by mentioning the component or control by name in your prompt.

### Example Prompts

```text
How do I bind data to the Syncfusion SegmentedControl in .NET MAUI?
```
→ The AI assistant loads the SegmentedControl skill and uses its get-started and data-binding reference docs.

```text
Help me migrate my Xamarin.Forms app to .NET MAUI.
```
→ The AI assistant loads the Migration skill.

### Using Reference Files

Each `references/` subfolder contains deeper implementation guides. When the AI assistant loads a skill, it can also pull in these files when you ask follow-up questions:

```text
Show me how to use auto-scroll, programmatic scrolling, and proper layout in .NET MAUI Accordion?.
```
→ The AI assistant uses `references/advanced-features.md` from the Accordion skill for the detailed answer.

## Skill File Structure

Every skill folder follows this layout:

```text
skills/
└── syncfusion-maui-toolkit-<control>/
    ├── SKILL.md                  ← Loaded by AI assistant; contains When to Use, Component Overview, and navigation links
    └── references/
        ├── getting-started.md    ← Installation, setup, NuGet packages, MauiProgram.cs
        ├── advanced-features.md  ← In-depth feature guides and code samples
        └── ...                   ← Additional reference files per control
```

`SKILL.md` sections:
- **When to Use This Skill** — trigger phrases and scenarios that activate this skill
- **Component Overview** — NuGet package, namespace, key capabilities at a glance
- **Documentation and Navigation Guide** — links to all reference files in the skill

## Repository Structure

```text
README.md
skills/
    syncfusion-maui-toolkit-getting-started/
    syncfusion-maui-toolkit-migration/
    syncfusion-maui-toolkit-theming/
    syncfusion-maui-toolkit-accordion/
    syncfusion-maui-toolkit-shimmer/
    ... (one folder per control, 32 total)
```

## Skill Index

> **Tip:** Start with [Getting Started](skills/syncfusion-maui-toolkit-getting-started/SKILL.md) if you are setting up a new project, and [Migration](skills/syncfusion-maui-toolkit-migration/SKILL.md) if upgrading from Syncfusion® .NET MAUI. For all other tasks, find the skill that matches the specific control below.

### Foundation

- [Getting Started](skills/syncfusion-maui-toolkit-getting-started/SKILL.md) — installation, themes
- [Migration](skills/syncfusion-maui-toolkit-migration/SKILL.md) — Syncfusion® .NET MAUI to Syncfusion® Toolkit for .NET MAUI migration guide
- [Theming](skills/syncfusion-maui-toolkit-theming/SKILL.md) — Material themes, dark mode, custom styling

### Data Visualization

- [Cartesian Charts](skills/syncfusion-maui-toolkit-cartesian-charts/SKILL.md)
- [Circular Charts](skills/syncfusion-maui-toolkit-circular-charts/SKILL.md)
- [Funnel Charts](skills/syncfusion-maui-toolkit-funnel-charts/SKILL.md)
- [Polar Charts](skills/syncfusion-maui-toolkit-polar-charts/SKILL.md)
- [Pyramid Charts](skills/syncfusion-maui-toolkit-pyramid-charts/SKILL.md)
- [Spark Charts](skills/syncfusion-maui-toolkit-spark-charts/SKILL.md)
- [Sunburst Charts](skills/syncfusion-maui-toolkit-sunburst-charts/SKILL.md)

### Calendars

- [Calendar](skills/syncfusion-maui-toolkit-calendar/SKILL.md)

### Editors

- [Date Picker](skills/syncfusion-maui-toolkit-date-picker/SKILL.md)
- [Date Time Picker](skills/syncfusion-maui-toolkit-date-time-picker/SKILL.md)
- [Numeric Entry](skills/syncfusion-maui-toolkit-numericentry/SKILL.md)
- [Numeric Up Down](skills/syncfusion-maui-toolkit-numeric-updown/SKILL.md)
- [OTP Input](skills/syncfusion-maui-toolkit-otp-input/SKILL.md)
- [Picker](skills/syncfusion-maui-toolkit-picker/SKILL.md)
- [Time Picker](skills/syncfusion-maui-toolkit-time-picker/SKILL.md)

### Navigation

- [Bottom Sheet](skills/syncfusion-maui-toolkit-bottom-sheet/SKILL.md)
- [Navigation Drawer](skills/syncfusion-maui-toolkit-navigation-drawer/SKILL.md)
- [Tab View](skills/syncfusion-maui-toolkit-tabview/SKILL.md)

### Layout

- [Accordion](skills/syncfusion-maui-toolkit-accordion/SKILL.md)
- [Cards](skills/syncfusion-maui-toolkit-cards/SKILL.md)
- [Carousel](skills/syncfusion-maui-toolkit-carousel/SKILL.md)
- [Expander](skills/syncfusion-maui-toolkit-expander/SKILL.md)
- [Popup](skills/syncfusion-maui-toolkit-popup/SKILL.md)
- [Text Input Layout](skills/syncfusion-maui-toolkit-text-input-layout/SKILL.md)
- [Grid Splitter](skills/syncfusion-maui-toolkit-grid-splitter/SKILL.md)

### Buttons

- [Button](skills/syncfusion-maui-toolkit-button/SKILL.md)
- [Chips](skills/syncfusion-maui-toolkit-chips/SKILL.md)
- [Segmented Control](skills/syncfusion-maui-toolkit-segmented-control/SKILL.md)

### Notification

- [Circular Progress Bar](skills/syncfusion-maui-toolkit-circular-progressbar/SKILL.md)
- [Linear Progress Bar](skills/syncfusion-maui-toolkit-linear-progressbar/SKILL.md)
- [Pull to Refresh](skills/syncfusion-maui-toolkit-pull-to-refresh/SKILL.md)

### Miscellaneous

- [Effects View](skills/syncfusion-maui-toolkit-effects-view/SKILL.md)
- [Shimmer](skills/syncfusion-maui-toolkit-shimmer/SKILL.md)