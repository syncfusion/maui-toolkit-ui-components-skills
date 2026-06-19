---
name: syncfusion-maui-toolkit-tabview
description: Implements and customizes tabbed navigation with Syncfusion® .NET MAUI TabView. Covers tab setup, customization, selection events, nested tabs, swiping gestures, and visual state management.
metadata:
  author: "Syncfusion Inc"
  version: "1.0.0"
---

# Syncfusion® .NET MAUI TabView Implementation Guide

### Key Capabilities

- **Nested Tabs:** Support for hierarchical tab structures with nested TabView instances
- **Header Flexibility:** Fixed and scrollable headers with image, text, and custom content support
- **Tab Customization:** Extensive appearance options including colors, fonts, spacing, and positioning
- **Gesture Support:** Built-in swiping gestures for seamless tab switching
- **Event System:** Comprehensive event handling for tab selection and interactions
- **State Management:** Visual state manager support for responsive UI patterns
- **Animation Control:** Smooth content transitions with customizable animation duration and easing

---

## When to Use This Skill

Use this skill when:

- **User wants to create tabbed interfaces** - Implementing multi-section layouts where only one tab is visible at a time
- **User needs tab customization** - Styling tabs with images, icons, text colors, fonts, and custom header content
- **User implements selection and navigation** - Handling tab selection events, programmatic tab switching, and event-driven workflows
- **User implements gestures** - Adding swipe gestures to switch between tabs on mobile devices
- **User needs nested tabs** - Creating hierarchical tab structures (tabs containing tabs)
- **User needs visual state management** - Binding tab properties to view models for responsive designs
- **User implements settings/preferences UI** - Using tabs to organize configuration sections
- **User builds multi-step forms or wizards** - Using tabs to organize workflow steps
- **User needs data dashboard layouts** - Organizing multiple data views in tab panels

---

## Component Overview

The **SfTabView** is Syncfusion's advanced tabbed navigation component for .NET MAUI applications. It provides a simple and intuitive interface for tab navigation in both mobile and desktop applications, allowing users to explore and switch between different tabs efficiently.

## Documentation and Navigation Guide

### Getting Started
📄 **Read:** [references/getting-started.md](references/getting-started.md)
- Installation and package setup with NuGet
- Registering handlers in MauiProgram.cs
- Creating your first TabView (XAML and C# approaches)
- Adding tabs and populating content
- Data binding with ItemsSource, HeaderItemTemplate, and ContentItemTemplate
- Running the application
- Common setup issues and solutions

### Tab Customization & Styling
📄 **Read:** [references/tab-customization.md](references/tab-customization.md)
- Tab item customization (text, icons, badges)
- Header display modes (text, icon, image modes)
- Tab bar appearance and sizing
- Image positioning options (top, bottom, left, right)
- Text color and font customization
- Font family, size, and attributes
- Tab header padding and scroll buttons
- Content transition animations
- Ripple effects and hover behavior

### Selection, Events & Swiping
📄 **Read:** [references/selection-and-swiping.md](references/selection-and-swiping.md)
- Tab selection and the SelectedIndex property
- Selection change events (SelectionChanging, SelectionChanged)
- TabItemTapped event handling
- Programmatic tab switching
- Swipe gestures and EnableSwiping property
- Selection indicator customization
- Disabled tabs
- Event cancellation and event parameters

### Advanced Features
📄 **Read:** [references/advanced-features.md](references/advanced-features.md)
- Nested TabView (creating hierarchical tab structures)
- Event handling in nested tabs
- Visual state managers for responsive designs
- Header placement options (top, bottom, left, right)
- Overflow behavior and scrollable headers
- Performance optimization techniques
- Font auto-scaling

### Center Button Configuration
📄 **Read:** [references/center-button.md](references/center-button.md)
- Enabling the center button with IsCenterButtonEnabled
- CenterButtonSettings property configuration
- Customizing appearance (background, stroke, corner radius)
- Setting button size, text, and images
- Display modes (text, image, or both)
- CenterButtonTapped event handling

### Common Use Cases & Patterns
📄 **Read:** [references/use-cases-and-patterns.md](references/use-cases-and-patterns.md)
- Settings/preferences interface
- Multi-step form wizard
- Data dashboard layout
- Document viewer with tabs
- Best practices and anti-patterns
- Accessibility guidelines (WCAG compliance)
- Keyboard navigation support
- Troubleshooting common issues

---
