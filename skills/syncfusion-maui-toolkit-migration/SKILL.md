---
name: syncfusion-maui-toolkit-migration
description: Migrate from Syncfusion® .NET MAUI to Syncfusion® Toolkit for .NET MAUI. Covers namespace updates, API changes, configuration methods, and step-by-step migration patterns with minimal code modifications for 20+ components.
metadata:
  author: "Syncfusion Inc"
  version: "1.0.0"
---

# Migration Guide: Syncfusion® .NET MAUI to Syncfusion® Toolkit for .NET MAUI

## When to Use This Skill

Use this skill when the user asks about:

- Migrating from older Syncfusion .NET MAUI libraries to Syncfusion MAUI Toolkit
- Updating namespaces in existing MAUI projects
- Converting ConfigureSyncfusionCore to ConfigureSyncfusionToolkit
- Upgrading or refactoring Syncfusion MAUI code
- Resolving migration-related errors or breaking changes

The Syncfusion® Toolkit for .NET MAUI represents the next generation of Syncfusion® components for MAUI applications. While most APIs and functionality remain the same, components have been consolidated into a single toolkit with updated namespaces. This guide helps you migrate existing Syncfusion® .NET MAUI projects to the new toolkit with minimal code modifications.

## Table of Contents

- [Component Overview](#component-overview)
- [Documentation and Navigation Guide](#documentation-and-navigation-guide)

## Component Overview

The migration from **Syncfusion® .NET MAUI** to **Syncfusion® Toolkit for .NET MAUI** involves three primary changes:

1. **Namespace Updates** - Component namespaces are reorganized under `Syncfusion.Maui.Toolkit.*`
2. **Assembly Consolidation** - Individual component assemblies consolidated into `Syncfusion.Maui.Toolkit`
3. **Configuration Method** - `ConfigureSyncfusionCore()` renamed to `ConfigureSyncfusionToolkit()`

**Good news:** Your existing component implementations work nearly identically. The primary effort is updating namespaces and the initialization method.

## Documentation and Navigation Guide

Choose your migration path based on where you are in the process:

### Getting Started
📄 **Read:** [references/getting-started.md](references/getting-started.md)

Start here if you:
- Are new to the migration process
- Need to understand migration scope and benefits
- Want prerequisites and an overview of what changes
- Are planning your migration timeline

**Covers:**
- Why migrate to the toolkit
- Prerequisites and requirements
- What components are affected
- High-level change summary

### Namespace Updates
📄 **Read:** [references/namespace-updates.md](references/namespace-updates.md)

Read this when you need to:
- Update XAML namespace declarations
- Modify C# using statements
- Find exact namespace mappings for specific components
- Understand assembly changes from NuGet packages
- Get search & replace patterns for your IDE

**Covers:**
- Complete XAML namespace reference (20+ controls)
- Complete C# namespace reference (20+ controls)
- Assembly changes and package structure
- Real-world migration examples with before/after code
- Troubleshooting namespace-related build errors

### Configuration Method Migration
📄 **Read:** [references/method-migration.md](references/method-migration.md)

Use this when you need to:
- Update your MauiProgram.cs initialization
- Change `ConfigureSyncfusionCore()` to `ConfigureSyncfusionToolkit()`
- Understand AppHostBuilder configuration
- See code-behind changes
- Review method signature changes

**Covers:**
- Step-by-step initialization update
- Old vs. new configuration code
- Complete MauiProgram.cs example
- Advanced configuration options
- Troubleshooting initialization issues

### Migration Checklist
📄 **Read:** [references/migration-checklist.md](references/migration-checklist.md)

Use this as your:
- Pre-migration verification checklist
- Step-by-step migration process guide
- Post-migration validation checklist
- Troubleshooting reference for common issues
- Performance validation guide

**Covers:**
- Pre-migration steps and backup procedures
- Component inventory preparation
- Step-by-step numbered migration process
- Build and test verification
- Common issues and solutions with fixes
- Migration completion checklist

**Next Steps:**
1. Read [references/getting-started.md](references/getting-started.md) for prerequisites
2. Use [references/namespace-updates.md](references/namespace-updates.md) to identify all components in your project
3. Follow [references/migration-checklist.md](references/migration-checklist.md) for step-by-step migration
4. Reference [references/method-migration.md](references/method-migration.md) for MauiProgram.cs update
5. See [references/examples-and-patterns.md](references/examples-and-patterns.md) for code examples and migration patterns

Good luck with your migration! The process is straightforward, and most developers complete it in 30-60 minutes depending on project size.