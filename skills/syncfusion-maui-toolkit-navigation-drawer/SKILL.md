---
name: syncfusion-maui-toolkit-navigation-drawer
description: Implement the Syncfusion® .NET MAUI Navigation Drawer (SfNavigationDrawer) control for creating navigation panes that slide from screen edges. Covers positioning (left, right, top, bottom), content configuration, animations, events, gestures, and customization. Use this skill whenever implementing drawer navigation in MAUI apps.
metadata:
  author: "Syncfusion Inc"
  version: "1.0.0"
---

# Syncfusion .NET MAUI Navigation Drawer Implementation

The **Syncfusion Navigation Drawer** (`SfNavigationDrawer`) is a flexible component that creates a sliding navigation pane in your .NET MAUI applications. It supports positioning from all four directions, animated transitions, swipe gestures, and comprehensive event handling.

## When to Use This Skill

Use this skill when you need to:

- **Implement drawer navigation** in .NET MAUI applications that display a sliding pane
- **Position navigation panes** from left, right, top, or bottom edges of the screen
- **Handle drawer interactions** including open/close events, animations, and gesture support
- **Configure drawer content** with main content areas, headers, and drawer pane layouts
- **Customize appearance** with animations, sizing, and styling options
- **Add mobile-friendly navigation** that responds to swipes or programmatic toggles
- **Manage complex navigation flows** where a drawer provides contextual menu or additional options

**Specific scenarios:** Hamburger menus, side navigation panels, bottom sheet navigation, app drawers, overlay menus, and any slide-out navigation patterns in MAUI applications.

---

## Component Overview

The `SfNavigationDrawer` consists of two main areas:

- **ContentView** - Always-visible main content area
- **Drawer Pane** - Hidden pane that slides in from the screen edge (positioned as Left, Right, Top, or Bottom)

**Key features:**
- Four directional positioning (Left, Right, Top, Bottom)
- Animated transitions (SlideOnTop, Push, Reveal)
- Swipe gesture support for opening/closing
- Comprehensive event handling (Opening, Opened, Closing, Closed, Toggled)
- Configurable drawer width/height and animations
- Support for complex drawer content layouts

---

## Documentation and Navigation Guide

Read the reference files below in order based on your implementation needs:

### Getting Started with Navigation Drawer
📄 **Read:** [references/getting-started.md](references/getting-started.md)
- Installing Syncfusion MAUI Toolkit package
- Registering handlers in MauiProgram.cs
- Creating your first Navigation Drawer
- Setting ContentView (mandatory)
- Basic XAML and C# implementation

### Content Configuration & Layout
📄 **Read:** [references/drawer-content.md](references/drawer-content.md)
- Configuring main content (ContentView property)
- Setting up drawer pane content
- Header and layout configuration
- Dynamic content switching
- Best practices for content organization

### Positioning & Sizing the Drawer
📄 **Read:** [references/positioning-sizing.md](references/positioning-sizing.md)
- Drawer positioning (Left, Right, Top, Bottom)
- DrawerSettings configuration
- Setting drawer width and height
- Drawer header sizing
- Responsive drawer sizing patterns

### Events & Interaction Handling
📄 **Read:** [references/events-interaction.md](references/events-interaction.md)
- Event types (DrawerOpening, DrawerOpened, DrawerClosing, DrawerClosed, DrawerToggled)
- Handling drawer state changes
- Canceling drawer operations
- Event-based navigation patterns
- User interaction workflows

### Animations & Transitions
📄 **Read:** [references/animations-transitions.md](references/animations-transitions.md)
- Animation types (SlideOnTop, Push, Reveal)
- Duration configuration and timing
- Toggle animation settings
- Smooth transition patterns
- Performance considerations

### Gestures & Accessibility
📄 **Read:** [references/gestures-accessibility.md](references/gestures-accessibility.md)
- Swipe gesture support for opening/closing
- Programmatic drawer toggling
- Keyboard interaction and accessibility
- Screen reader support
- Best practices for inclusive design

---
