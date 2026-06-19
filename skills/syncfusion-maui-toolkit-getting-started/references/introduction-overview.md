# Introduction to Syncfusion® .NET MAUI Toolkit

## Table of Contents
- [What is Syncfusion® .NET MAUI Toolkit](#what-is-syncfusion-net-maui-toolkit)
- [Cross-Platform Capabilities](#cross-platform-capabilities)
- [Component Ecosystem Overview](#component-ecosystem-overview)
- [Supported Platforms](#supported-platforms)
- [System Requirements](#system-requirements)
- [Framework Compatibility](#framework-compatibility)
- [Development Environment Setup](#development-environment-setup)
- [How to Use This User Guide](#how-to-use-this-user-guide)

---

## What is Syncfusion® .NET MAUI Toolkit

Syncfusion® .NET MAUI Toolkit is a comprehensive collection of .NET MAUI components designed for building modern mobile and desktop applications from a single shared codebase. Built on Microsoft's .NET Multi-platform App UI (.NET MAUI) framework, it provides high-performance, feature-rich UI controls that work seamlessly across multiple platforms.

### Key Features

- **20+ Professional Components:** Complete suite of buttons, editors, calendars, and more
- **Single Codebase:** Write once, deploy to Android, iOS, macOS (Mac Catalyst), and Windows (WinUI 3)
- **Native Performance:** Platform-specific optimizations ensure smooth, responsive user experiences
- **Modern Design:** Material Design with automatic light/dark mode support
- **Enterprise-Ready:** Production-tested, WCAG-compliant, with comprehensive documentation and support

### Why Choose Syncfusion® .NET MAUI Toolkit

- **Accelerated Development:** Pre-built, production-ready components reduce development time
- **Consistent Design:** Uniform look-and-feel across all platforms with theme support
- **Extensive Customization:** Flexible APIs, styling options, and templating capabilities
- **Professional Support:** Access to knowledge base, forums, and dedicated support team
- **Regular Updates:** Frequent releases with new features, improvements, and bug fixes

---

## Cross-Platform Capabilities

### Supported Platforms

Syncfusion® .NET MAUI Toolkit components support development for:

1. **Android** - Native Android applications (API 21+)
2. **iOS** - Native iOS applications (iOS 12.2+)
3. **macOS** - Mac desktop applications via Mac Catalyst (macOS 12+)
4. **Windows** - Windows desktop applications via WinUI 3 (Windows 10 1809+, Windows 11)

### Architecture

.NET MAUI uses a single project system where:
- **Shared Code:** Business logic, UI layouts, and component usage in one codebase
- **Platform-Specific:** Platform-specific code when needed (handled by .NET MAUI)
- **Resource Management:** Unified resource system for images, fonts, and assets
- **Native APIs:** Access to platform-specific APIs when required

### Cross-Platform Development Benefits

- **Code Reusability:** 90%+ code sharing across platforms
- **Faster Time-to-Market:** Build for all platforms simultaneously
- **Consistent UX:** Uniform user experience with platform-specific adaptations
- **Easier Maintenance:** Single codebase reduces maintenance overhead
- **Cost-Effective:** One development team can target multiple platforms

---

## Component Ecosystem Overview

### Data Visualization Components

**Data Visualization**
- Cartesian Charts (Line, Bar, etc.)
- Circular Charts (Pie, Doughnut, Radial Bar)
- Funnel and Pyramid Charts
- Polar Charts
- Sunburst Charts
- Spark Charts

### Editors

**DatePicker** - Date selection control  
**TimePicker** - Time selection control  
**DateTimePicker** - Select date ranges  
**NumericEntry** - Numeric input with formatting  
**NumericUpDown** - Adjust values with Up/Down button
**OTP input** - Secure input field for one-time password
**Picker** - Option selection control

### Calendars

**Calendar** - Month/day/year view with selection  

### Navigation

**TabView** - Tabbed navigation  
**NavigationDrawer** - Slide-out navigation menu 
**BottomSheet** - Slide-up from the bottom of the screen  

### Buttons

**Button** - Customizable buttons with icons, styles 
**SegmentedControl** - Segmented button group
**Chips** - Material chips/tags 

### Layout

**TextInputLayout** - Material-design text input with floating labels  
**Accordion** - Organizes content into multiple expandable sections
**Cards** - Create dismissible cards
**Carousel** - Smooth, touch-enabled sliding galleries for showcasing images 
**Expander** - Expand or collapse content dynamically
**Popup** - Display an alert message with customizable buttons

### Notification

**Circular Progressbar** - Represents task progression through a circular visualization.
**Linear Progressbar** - Represents task progression through a linear visualization.
**Pull To Refresh** - refresh live data by pulling down

### Additional Components

**EffectsView** - Visual effects (blur, shadow, glow) 
**Shimmer** - Indicates loading content with customizable wave directions 
---

## Supported Platforms

### Platform Details

| Platform | Minimum Version | Recommended Version | Notes |
|----------|----------------|---------------------|-------|
| **Android** | API 21 (Android 5.0) | API 31+ (Android 12+) | Targets Android devices |
| **iOS** | iOS 12.2 | iOS 15+ | Targets iPhones, iPads |
| **macOS** | macOS 12 (Monterey) | macOS 13+ (Ventura) | Via Mac Catalyst |
| **Windows** | Windows 10 1809 | Windows 11 | Via WinUI 3 |
|  | Windows Server 2016+ | Windows Server 2022 | Server applications |

### Platform Support Matrix

All Syncfusion® .NET MAUI Toolkit components support all four platforms (Android, iOS, Mac Catalyst, WinUI) unless otherwise specified in component-specific documentation.

### Platform-Specific Considerations

**Android:**
- Requires Android SDK installed
- Min API level 21 (Lollipop)
- Supports all Android form factors (phone, tablet)

**iOS:**
- Requires macOS with Xcode for building
- Supports iPhone and iPad
- iOS 12.2+ required

**macOS:**
- Mac Catalyst translates iOS apps to macOS
- macOS 12+ (Monterey or later)
- Full desktop capabilities

**Windows:**
- Windows 10 version 1809 or higher
- WinUI 3 (Windows App SDK)
- Windows 11 recommended for best performance

---

## System Requirements

### Hardware Requirements

**Minimum:**
- Processor: x86 or x64
- RAM: 4 GB
- Hard disk: 210 GB free space (for full development environment)

**Recommended:**
- Processor: x64 multi-core
- RAM: 16 GB
- Hard disk: SSD with 250 GB+ free space
- Graphics: Dedicated GPU for emulator performance

### Operating System Requirements

**Windows Development:**
- Windows 11 version 21H2 or higher (Home, Pro, Enterprise, Education)
- Windows 10 version 1909 or higher (Home, Professional, Enterprise, Education)
- Windows Server 2022 (Standard, Datacenter)
- Windows Server 2019 (Standard, Datacenter)
- Windows Server 2016 (Standard, Datacenter)

**macOS Development:**
- macOS 12 (Monterey) or higher
- Xcode 13+ (for iOS/macOS development)

### Development Tools

**Visual Studio 2022 (Windows/Mac):**
- Visual Studio 2022 17.8.0 or later
- .NET MAUI workload installed
- Android SDK (for Android development)
- Xcode (macOS only, for iOS/macOS development)

**Visual Studio 2026:**
- Visual Studio 2026 18.0.0 or later
- Latest .NET MAUI tooling

**Visual Studio Code:**
- VS Code with .NET MAUI extension
- .NET SDK 6.0+ installed
- Platform SDKs installed separately

---

## Framework Compatibility

### Supported .NET Versions

Syncfusion® .NET MAUI Toolkit components support:
- **.NET 9.0** - Current recommended version
- **.NET 10.0** - Latest version

### Version Compatibility Matrix

| Syncfusion Version | .NET 9.0 | .NET 10.0 |
|--------------------|----------|-----------|
| >= v1.0.1          |     Yes  |    No     |
| >= v1.0.8          |    Yes   |  Yes      |

### Recommendations

- **Use .NET 9.0 or .NET 10.0:** Latest Syncfusion® versions target current .NET releases
- **Match Versions:** Ensure Syncfusion® package version aligns with your .NET SDK version
- **LTS Support:** For long-term projects, use .NET LTS (Long-Term Support) versions
- **Stay Updated:** Newer .NET versions provide performance improvements and new features

---

## Development Environment Setup

### Windows Setup

1. **Install Visual Studio 2022 (17.8.0+):**
   - Download from visualstudio.microsoft.com
   - Select ".NET Multi-platform App UI development" workload during installation
   - Include Android SDK and Android emulators

2. **Install .NET SDK:**
   - .NET 9.0 or .NET 10.0 SDK
   - Verify installation: `dotnet --version`

3. **Configure Android Development:**
   - Install Android SDK via Visual Studio
   - Set up Android emulator or connect physical device
   - Enable USB debugging on device

4. **Install Syncfusion® Components:**
   - Via NuGet Package Manager
   - Or install full Syncfusion® installer

### Visual Studio Code Setup

1. **Install VS Code:**
   - Download from code.visualstudio.com

2. **Install .NET MAUI Extension:**
   - Open Extensions panel (Ctrl+Shift+X / Cmd+Shift+X)
   - Search for ".NET MAUI"
   - Install official .NET MAUI extension

3. **Install .NET SDK:**
   - .NET 9.0 or .NET 10.0 SDK

4. **Install Platform SDKs:**
   - Android SDK for Android development
   - Xcode for iOS/macOS development (macOS only)

5. **Install Syncfusion® Components:**
   - Via .NET CLI: `dotnet add package Syncfusion.Maui.Toolkit`

---

## How to Use This User Guide

### For New Users

1. **Start Here:** Read this introduction to understand Syncfusion® .NET MAUI Toolkit capabilities
2. **Installation:** Follow installation guides to set up NuGet packages or installers
4. **Themes:** Apply Material themes to your application
5. **Component-Specific Documentation:** Navigate to specific component skills for implementation details

### For Experienced Developers

- **Search:** Use semantic search to find specific features and APIs quickly
- **Quick Reference:** Jump directly to component-specific documentation
- **API Reference:** Detailed class and member documentation available
- **Code Examples:** Sample browser contains real-world usage examples

### Best Practices for Reading

- **Getting Started Sections:** Always read component-specific "Getting Started" sections end-to-end
- **Integration:** Use provided code examples to accelerate integration
- **Search for Features:** Use search to find detailed information on specific features
- **API Reference:** Consult API docs for detailed technical information

---

## Quick Start Checklist

✅ Verify system meets minimum requirements  
✅ Install Visual Studio 2022 17.8.0+ with .NET MAUI workload  
✅ Install .NET 9.0 or .NET 10.0 SDK  
✅ Install platform-specific SDKs (Android SDK, Xcode)  
✅ Install Syncfusion® NuGet packages  
✅ Apply theme (MaterialLight/MaterialDark)  
✅ Start building with Syncfusion® components!

For detailed installation instructions, see the following reference files:
- [dotnet-cli-installation.md](dotnet-cli-installation.md) – Install via .NET CLI
- [nuget-package-manager-ui.md](nuget-package-manager-ui.md) – Install via Visual Studio NuGet Package Manager UI
- [package-manager-console.md](package-manager-console.md) – Install via Package Manager Console