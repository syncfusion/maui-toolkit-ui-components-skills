# Quick Start Example & Migration Patterns

## Quick Start Example

Here's how a typical XAML migration looks. The component usage itself doesn't change—only the namespace:

### Before (Syncfusion® .NET MAUI)

**XAML:**
```xml
<ContentPage xmlns="http://schemas.microsoft.com/dotnet/2021/maui"
             xmlns:button="clr-namespace:Syncfusion.Maui.Buttons;assembly=Syncfusion.Maui.Buttons">
    <VerticalStackLayout>
        <button:SfButton Text="Click Me" Clicked="OnButtonClicked" />
    </VerticalStackLayout>
</ContentPage>
```

**C# (MauiProgram.cs):**
```csharp
using Syncfusion.Maui.Core.Hosting;

var builder = MauiApp.CreateBuilder();
builder
    .UseMauiApp<App>()
    .ConfigureFonts(fonts => fonts.AddFont("OpenSans-Regular.ttf", "OpenSansRegular"))
    .ConfigureSyncfusionCore();

return builder.Build();
```

**C# (Code-Behind):**
```csharp
using Syncfusion.Maui.Buttons;

namespace MigrationApp;

public partial class MainPage : ContentPage
{
    public MainPage()
    {
        InitializeComponent();
    }

    private void OnButtonClicked(object sender, EventArgs e)
    {
        DisplayAlert("Success", "Button clicked!", "OK");
    }
}
```

### After (Syncfusion® Toolkit for .NET MAUI)

**XAML:**
```xml
<ContentPage xmlns="http://schemas.microsoft.com/dotnet/2021/maui"
             xmlns:button="clr-namespace:Syncfusion.Maui.Toolkit.Buttons;assembly=Syncfusion.Maui.Toolkit">
    <VerticalStackLayout>
        <button:SfButton Text="Click Me" Clicked="OnButtonClicked" />
    </VerticalStackLayout>
</ContentPage>
```

**C# (MauiProgram.cs):**
```csharp
using Syncfusion.Maui.Toolkit.Hosting;

var builder = MauiApp.CreateBuilder();
builder
    .UseMauiApp<App>()
    .ConfigureFonts(fonts => fonts.AddFont("OpenSans-Regular.ttf", "OpenSansRegular"))
    .ConfigureSyncfusionToolkit();

return builder.Build();
```

**C# (Code-Behind):**
```csharp
using Syncfusion.Maui.Toolkit.Buttons;

namespace MigrationApp;

public partial class MainPage : ContentPage
{
    public MainPage()
    {
        InitializeComponent();
    }

    private void OnButtonClicked(object sender, EventArgs e)
    {
        DisplayAlert("Success", "Button clicked!", "OK");
    }
}
```

**Summary of Changes:**
- ✅ XAML namespace: `Syncfusion.Maui.Buttons` → `Syncfusion.Maui.Toolkit.Buttons`
- ✅ XAML assembly: `Syncfusion.Maui.Buttons` → `Syncfusion.Maui.Toolkit`
- ✅ C# using: `Syncfusion.Maui.Buttons` → `Syncfusion.Maui.Toolkit.Buttons`
- ✅ Configuration: `ConfigureSyncfusionCore()` → `ConfigureSyncfusionToolkit()`
- ✅ MauiProgram.cs using: `Syncfusion.Maui.Core.Hosting` → `Syncfusion.Maui.Toolkit.Hosting`
- ✅ Component usage: **No changes** - `SfButton` behavior is identical

## Common Migration Patterns

### Pattern 1: Multiple Components in One Page

When your page uses multiple Syncfusion® components, update all namespace declarations:

**Before:**
```xml
<ContentPage xmlns="http://schemas.microsoft.com/dotnet/2021/maui"
             xmlns:button="clr-namespace:Syncfusion.Maui.Buttons;assembly=Syncfusion.Maui.Buttons"
             xmlns:calendar="clr-namespace:Syncfusion.Maui.Calendar;assembly=Syncfusion.Maui.Calendar"
             xmlns:cards="clr-namespace:Syncfusion.Maui.Cards;assembly=Syncfusion.Maui.Cards">
```

**After:**
```xml
<ContentPage xmlns="http://schemas.microsoft.com/dotnet/2021/maui"
             xmlns:button="clr-namespace:Syncfusion.Maui.Toolkit.Buttons;assembly=Syncfusion.Maui.Toolkit"
             xmlns:calendar="clr-namespace:Syncfusion.Maui.Toolkit.Calendar;assembly=Syncfusion.Maui.Toolkit"
             xmlns:cards="clr-namespace:Syncfusion.Maui.Toolkit.Cards;assembly=Syncfusion.Maui.Toolkit">
```

### Pattern 2: Code-Behind Multi-Component Usage

When using components in code-behind, update all using statements:

**Before:**
```csharp
using Syncfusion.Maui.Buttons;
using Syncfusion.Maui.Calendar;
using Syncfusion.Maui.Cards;

namespace MyApp;

public partial class ComplexPage : ContentPage
{
    public ComplexPage()
    {
        InitializeComponent();
        var button = new SfButton { Text = "Dynamic" };
        var calendar = new SfCalendar();
    }
}
```

**After:**
```csharp
using Syncfusion.Maui.Toolkit.Buttons;
using Syncfusion.Maui.Toolkit.Calendar;
using Syncfusion.Maui.Toolkit.Cards;

namespace MyApp;

public partial class ComplexPage : ContentPage
{
    public ComplexPage()
    {
        InitializeComponent();
        var button = new SfButton { Text = "Dynamic" };
        var calendar = new SfCalendar();
    }
}
```

### Pattern 3: Conditional Component Usage

When using components conditionally or in view models, ensure all namespace declarations are updated:

**Before:**
```csharp
using Syncfusion.Maui.Buttons;

namespace MyApp.ViewModels;

public class ButtonViewModel
{
    public SfButton CreateButton()
    {
        return new SfButton 
        { 
            Text = "Action",
            BackgroundColor = Colors.Blue
        };
    }
}
```

**After:**
```csharp
using Syncfusion.Maui.Toolkit.Buttons;

namespace MyApp.ViewModels;

public class ButtonViewModel
{
    public SfButton CreateButton()
    {
        return new SfButton 
        { 
            Text = "Action",
            BackgroundColor = Colors.Blue
        };
    }
}
```

## Key Migration Principles

### 1. Namespace-Based Migration
All changes center around namespaces. Component APIs, properties, and event signatures remain virtually identical.

### 2. Single Assembly Consolidation
Instead of installing individual component packages (Syncfusion.Maui.Buttons, Syncfusion.Maui.Calendar, etc.), you install the single **Syncfusion.Maui.Toolkit** NuGet package.

### 3. Minimal Code Changes
Existing code logic and implementation patterns require no changes. Only namespace declarations and assembly references are updated.

### 4. One-Time Initialization Update
Update `MauiProgram.cs` once at application startup. All components then use the new toolkit automatically.

### 5. Complete Backward Compatibility
Component functionality, properties, events, and behaviors are fully preserved. No feature changes required.
