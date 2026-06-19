---
name: syncfusion-maui-toolkit-numericentry
description: Implement numeric input with Syncfusion® .NET MAUI NumericEntry (SfNumericEntry). Supports currency, percentage, and decimal formatting with validation, min/max restrictions, placeholder text, custom styling, and culture-specific formats. Includes value change modes, events, and accessibility features for professional numeric data entry.
metadata:
  author: "Syncfusion Inc"
  version: "1.0.0"
---

# Implementing .NET MAUI Numeric Entry

The Syncfusion .NET MAUI Numeric Entry control is designed to deliver a user-friendly and advanced input experience for numeric data. It supports a broad range of numeric formats, including currency, percentages, decimals, and other configurable number types. With its rich set of features, the control enhances the overall user experience while simplifying numeric input validation and formatting.

## When to Use This Skill

Use this skill when users need to:
- Financial applications requiring currency input
- Forms with percentage or decimal number fields
- Data entry scenarios with min/max value constraints
- Applications requiring culture-specific number formatting
- Scientific or calculator-style numeric inputs
- Budget, pricing, or quantity input fields

## Component Overview

The **Syncfusion .NET MAUI Numeric Entry (SfNumericEntry)** is a specialized input control designed for numeric data entry with advanced features:

### Key Capabilities

- Automatic numeric validation with customizable validation modes
- Rich formatting options (currency, percentage, decimal, custom patterns)
- Value restrictions (min/max ranges, null handling)
- Culture-specific number formatting and localization
- Real-time or on-blur validation modes
- Extensive styling and customization options
- Built-in events for value changes, focus, and completion
- Accessibility support with keyboard navigation

---

## Documentation and Navigation Guide

### Getting Started
📄 **Read:** [references/getting-started.md](references/getting-started.md)

When the user needs to set up NumericEntry for the first time:
- Installing and configuring the Syncfusion MAUI Toolkit package
- Registering handlers in MauiProgram.cs
- Adding namespace imports for XAML and C#
- Creating a basic NumericEntry control
- Understanding value editing and validation modes (OnKeyFocus vs OnLostFocus)
- Applying basic number formats (currency, percentage, decimal)
- Configuring null value behavior with AllowNull

### Basic Features and Configuration
📄 **Read:** [references/basic-features.md](references/basic-features.md)

When the user wants to customize appearance and interaction:
- Setting placeholder text and color for empty states
- Showing/hiding and styling the clear button
- Configuring value change modes (real-time vs on-blur updates)
- Customizing borders and strokes
- Aligning text horizontally and vertically
- Customizing fonts (color, size, family, attributes)
- Configuring keyboard return type and commands
- Managing cursor position and text selection
- Creating custom clear button icons

### Value Formatting
📄 **Read:** [references/formatting.md](references/formatting.md)

When the user needs to format numeric values:
- Using CustomFormat property with standard format specifiers (C, P, N)
- Formatting currency values with culture-specific symbols
- Formatting percentages with Value or Compute display modes
- Formatting decimal numbers with precision control
- Controlling integer digit display with zero placeholders
- Controlling fractional digit precision
- Creating custom format patterns with # and 0 placeholders
- Supporting multiple cultures and localization
- Limiting decimal places with MaximumNumberDecimalDigits

### Value Restrictions
📄 **Read:** [references/restrictions.md](references/restrictions.md)

When the user needs to restrict or validate input:
- Allowing or preventing null values with AllowNull
- Setting minimum and maximum value ranges
- Understanding validation behavior for out-of-range values
- Preventing text editing with IsEditable
- Configuring read-only numeric displays
- Handling edge cases (null vs zero, minimum value behavior)

### Events and Methods
📄 **Read:** [references/events-and-methods.md](references/events-and-methods.md)

When the user needs to respond to user interactions:
- Handling value changes with ValueChanged event
- Responding to Enter key press with Completed event
- Detecting focus gained/lost with Focused and Unfocused events
- Programmatically setting focus with Focus() method
- Removing focus with Unfocus() method
- Accessing old and new values in event arguments
- Implementing form submission and navigation patterns

---
