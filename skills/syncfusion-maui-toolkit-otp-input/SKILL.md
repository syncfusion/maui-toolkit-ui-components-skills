---
name: syncfusion-maui-toolkit-otp-input
description: Implement Syncfusion® .NET MAUI OTP Input controls for authentication flows. Covers input types (Number, Text, Password), styling modes (Outlined, Filled, Underlined), event handling, value binding, validation patterns, and accessibility. Use this skill when building SMS/email OTP verification, multi-step authentication, or secure login forms.
metadata:
  author: "Syncfusion Inc"
  version: "1.0.0"
---

# .NET MAUI OTP Input (SfOtpInput) Skill

The [OTP Input](https://help.syncfusion.com/cr/maui-toolkit/Syncfusion.Maui.Toolkit.OtpInput.SfOtpInput.html) is a specialized user interface component for collecting one-time passwords (OTPs) in authentication workflows. This skill provides comprehensive guidance for implementing OTP Input controls in .NET MAUI applications with proper configuration, styling, event handling, and validation.

## When to Use This Skill

Use this skill when you need to:

- **Build authentication flows** — Implement SMS or email-based OTP verification systems
- **Create multi-step verification** — Develop secure login processes requiring one-time passwords
- **Design password reset flows** — Build secure account recovery with OTP confirmation
- **Implement account security** — Add two-factor authentication (2FA) with time-limited codes
- **Collect structured numeric/alphanumeric input** — Use OTP Input for any fixed-length code entry
- **Customize input appearance** — Apply different styling modes (Outlined, Filled, Underlined) to match app design
- **Handle input validation** — Real-time validation and completion detection for OTP codes
- **Support accessibility** — Ensure keyboard navigation and screen reader compatibility

**Keywords that should trigger this skill:** OTP, one-time password, authentication, verification code, SMS verification, email verification, 2FA, two-factor authentication, OtpInput, SfOtpInput, security verification, code entry, phone verification, MAUI input

## Component Overview

**Key Features:**
- **Input Types** — Number (numeric-only), Text (alphanumeric), Password (hidden) modes
- **Styling Modes** — Outlined (bordered), Filled (background color), Underlined (underline only) visual variants
- **Configurable Length** — Set the number of input fields (e.g., 4-digit, 6-digit codes)
- **Separator Support** — Add visual separators between input fields for clarity
- **Value Binding** — Retrieve and set OTP values programmatically
- **Event Handling** — ValueChanged event for real-time input monitoring and validation
- **Accessibility** — Keyboard navigation and screen reader support for inclusive design

## Documentation and Navigation Guide

### Getting Started
📄 **Read:** [references/getting-started.md](references/getting-started.md)
- Installation and NuGet package setup
- Handler registration in MauiProgram.cs
- Basic OTP Input implementation
- Setting initial values and field length
- XAML and C# implementation patterns

### Input Types
📄 **Read:** [references/input-types.md](references/input-types.md)
- Number type (default, numeric-only codes)
- Text type (alphanumeric OTP codes)
- Password type (hidden/masked input for privacy)
- Choosing the right type for your use case
- Type conversion and switching behavior

### Styling Modes
📄 **Read:** [references/styling-modes.md](references/styling-modes.md)
- Outlined mode (bordered fields)
- Filled mode (background-filled fields)
- Underlined mode (underline-only fields)
- Styling mode selection guide
- Visual appearance comparison

### Features and Configuration
📄 **Read:** [references/features-and-configuration.md](references/features-and-configuration.md)
- Length property (number of input fields)
- Separator configuration (visual spacing)
- Value retrieval and binding
- Disabled state handling
- Focus and cursor management
- Multi-platform considerations

### Events and Validation
📄 **Read:** [references/events-and-validation.md](references/events-and-validation.md)
- ValueChanged event handling and event args
- Real-time input validation patterns
- OTP completion detection
- Error handling and recovery
- Input sanitization best practices
- Performance optimization tips
