---
name: syncfusion-maui-toolkit-numeric-updown
description: Implement the Syncfusion® .NET MAUI NumericUpDown control for numeric input with validation, formatting, and increment/decrement buttons. Use this skill when building forms requiring numeric entry with up-down buttons, currency formatting, percentage values, decimal precision, custom formats, input validation, or placeholder text.
metadata:
  author: "Syncfusion Inc"
  version: "1.0.0"
---

# Syncfusion .NET MAUI NumericUpDown

The **SfNumericUpDown** control provides a user-friendly numeric input experience with built-in validation, formatting options, and convenient increment/decrement buttons. Perfect for building professional forms that require validated numeric entry.

## When to Use This Skill

Use this skill when you need to:

- **Build numeric input fields** in .NET MAUI applications
- **Format numbers** as currency (C2), percentages (P2), or decimals (N2)
- **Restrict input** to valid ranges (Minimum/Maximum values)
- **Provide quick value adjustments** with up/down arrow buttons or keyboard controls
- **Display placeholders** for empty numeric fields
- **Handle validation** automatically with OnKeyFocus or OnLostFocus modes
- **Customize appearance** of buttons, colors, borders, and fonts
- **Support cultural formats** with culture-aware number display

## Component Overview

The **SfNumericUpDown** (or NumericUpDown) control is a specialized input field designed for entering and editing numeric values in .NET MAUI applications. It combines three interaction patterns:

**What It Does:**
- Accepts numeric input with optional text field for direct entry
- Provides increment/decrement buttons (up/down arrows) for quick value adjustment
- Supports keyboard navigation (arrow keys, Page Up/Down, Tab, Return)
- Enforces validation with configurable ranges (Minimum/Maximum)
- Formats numbers according to culture, currency, or custom specifications
- Displays placeholder text when no value is set

**Key Characteristics:**
- **Smart Validation:** OnKeyFocus (real-time) or OnLostFocus (deferred) validation modes
- **Flexible Formatting:** Currency (C2), percentages (P2), decimals (N2), or custom formats
- **Customizable Buttons:** Placement modes (Inline, InlineVertical), alignment (Left, Right, Both), color, and custom templates
- **Constraint Support:** Min/Max ranges, null handling (AllowNull), text-only mode (IsEditable=false)
- **Event Driven:** ValueChanged, Completed, Focused/Unfocused events for form integration
- **Accessible:** Support for WCAG compliance, screen readers, and keyboard-only navigation

**When to Choose NumericUpDown:**
- Need a professional numeric input with built-in increment buttons
- Want automatic validation and formatting without custom code
- Building financial forms (prices, discounts, percentages)
- Creating inventory systems (quantities, stock levels)
- Implementing settings or preference screens
- Need culture-aware number formatting

## Documentation and Navigation Guide

### Getting Started
📄 **Read:** [references/getting-started.md](references/getting-started.md)
- Installation and NuGet package setup
- Registering handlers in MauiProgram.cs
- Adding a basic NumericUpDown control
- XAML and C# initialization patterns
- First render and validation modes

### Value Management & Constraints
📄 **Read:** [references/value-management.md](references/value-management.md)
- Setting and binding numeric values
- Minimum and Maximum value restrictions
- Null value handling with AllowNull property
- Default values and initial setup
- Preventing manual text editing with IsEditable

### Formatting & Display Options
📄 **Read:** [references/formatting-display.md](references/formatting-display.md)
- Custom number formats (currency, percentage, decimal)
- Placeholder text and placeholder color customization
- Culture-aware number display
- Maximum decimal digits management
- Percentage display modes (Value vs Compute)
- Custom format specifiers (0, #, C, P, N)

### Validation & Events
📄 **Read:** [references/validation-events.md](references/validation-events.md)
- ValueChanged event with OldValue and NewValue
- Completed event when editing is finished
- Focused and Unfocused events
- ValueChangeMode (OnKeyFocus vs OnLostFocus)
- Programmatic focus management
- Return key commands

### Up/Down Button Control
📄 **Read:** [references/buttons-updown.md](references/buttons-updown.md)
- SmallChange and LargeChange increments
- Keyboard shortcuts (Arrow keys, Page Up/Down)
- Mouse scroll wheel support
- Up/Down button placement modes (Inline, InlineVertical)
- Button alignment (Left, Right, Both)
- Button color customization
- Custom button templates
- Auto-reverse behavior

### Customization & UI Features
📄 **Read:** [references/customization.md](references/customization.md)
- Border visibility and stroke color
- Text color and alignment customization
- Font family, size, and attributes
- Clear button visibility and customization
- Cursor position and text selection
- Return key types and keyboard behavior
- Advanced styling patterns
- Common gotchas and troubleshooting