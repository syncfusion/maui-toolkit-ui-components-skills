---
name: syncfusion-maui-toolkit-bottom-sheet
description: Implement the Syncfusion® .NET MAUI Bottom Sheet (SfBottomSheet) control with state management, content configuration, gesture support, and customization. Covers setup, content binding, state transitions, styling, events, and interactive patterns for sliding content panels.
metadata:
  author: "Syncfusion Inc"
  version: "1.0.0"
---

# .NET MAUI Bottom Sheet (SfBottomSheet)

**Key Features:**
- Multiple states: FullExpanded, HalfExpanded, Collapsed, Hidden
- Flexible content configuration with data binding support
- Touch gestures: swipe to expand/collapse
- Extensive customization: colors, dimensions, corner radius, padding, grabber styling
- Event handling and state change notifications
- Modal and non-modal display modes
- Programmatic control via IsOpen property and Show/Close methods

---

## When to Use This Skill

Use this skill when you need to:

- **Display supplementary content** without full page navigation (product details, information panels, settings)
- **Create data-driven interactions** that bind list selections to detailed content views
- **Implement modal dialogs** or confirmation sheets that overlay the main content
- **Provide partial reveal patterns** where users gradually expand content (peek-a-boo effect)
- **Enable gesture-based UI** where users swipe to reveal more information
- **Customize appearance** to match application themes (colors, sizes, rounded corners, animations)
- **Handle state transitions** programmatically or through user interaction
- **Manage focus and overlay behavior** in mobile-first applications

---

## Component Overview

The Bottom Sheet is a user interface component that slides up from the bottom of the screen, allowing users to interact with additional information or actions without navigating away from the main screen. The Syncfusion `SfBottomSheet` control provides comprehensive state management, content configuration, gesture support, and extensive customization options for .NET MAUI applications.

## Documentation and Navigation Guide

### Getting Started
📄 **Read:** [references/getting-started.md](references/getting-started.md)
- Project setup and template creation
- NuGet package installation (Syncfusion.Maui.Toolkit)
- Handler registration in MauiProgram.cs
- Basic control initialization
- First working example with ListView integration

### Content Configuration
📄 **Read:** [references/content-configuration.md](references/content-configuration.md)
- Setting main content vs. bottom sheet content
- Data binding with ViewModels
- Layout patterns (VerticalStackLayout, Grid, ListView)
- Dynamic content updates
- Binding context management

### States and State Management
📄 **Read:** [references/states-management.md](references/states-management.md)
- State property values and transitions
- AllowedState configuration (FullExpanded, HalfExpanded, All)
- IsOpen property for programmatic control
- State change scenarios and use cases

### Customization and Styling
📄 **Read:** [references/customization-styling.md](references/customization-styling.md)
- Popup mode (IsModal) and overlay behavior
- Background color and corner radius
- Height adjustments (FullExpandedRatio, HalfExpandedRatio, CollapsedHeight)
- Width modes (Full, Custom)
- Content padding and spacing
- Grabber element customization
- Animation duration configuration

### Gestures, Events, and Methods
📄 **Read:** [references/gestures-events-methods.md](references/gestures-events-methods.md)
- Swipe gesture support (EnableSwiping)
- StateChanged event handling
- CollapseOnOverlayTap for overlay interaction
- Show/Close methods for programmatic control
- Event argument inspection

### Common Patterns and Real-World Scenarios
📄 **Read:** [references/common-patterns.md](references/common-patterns.md)
- Data-driven Bottom Sheet with list selection
- Modal dialogs and confirmation sheets
- Partial reveal and peek patterns
- Dynamic content binding
- Error handling and edge cases
- Best practices and anti-patterns

---
