# Center Button Configuration in .NET MAUI Tab View

## Overview

The center button is an optional action button positioned at the center of the tab bar. It's commonly used for primary actions like adding new items, creating content, or launching key features. This reference covers enabling, customizing, and handling the center button.

---

## Enabling the Center Button

### Step 1: Enable with IsCenterButtonEnabled

Set the `IsCenterButtonEnabled` property to `true` to display the center button:

```xaml
<tabView:SfTabView IsCenterButtonEnabled="True">
    <!-- Your tab items here -->
</tabView:SfTabView>
```

C# Code:
```csharp
SfTabView tabView = new SfTabView();
tabView.IsCenterButtonEnabled = true;
```

### Default Appearance

By default, the center button appears as a simple circular button in the center of the tab bar. The default styling includes:
- Circular shape with automatic sizing
- Platform-specific styling (Material Design on Android, iOS-native style on iOS)
- No text or image by default

---

## Customizing Center Button Appearance

Use the `CenterButtonSettings` property to customize the center button's appearance:

```xaml
<tabView:SfTabView IsCenterButtonEnabled="True">
    <tabView:SfTabView.CenterButtonSettings>
        <tabView:CenterButtonSettings 
            Height="45" 
            Width="45" 
            CornerRadius="50"
            Background="#6750A4"
            Stroke="#3700B3"
            StrokeThickness="2"
            TextColor="White"
            FontSize="14"
            Title="+"
            ImageSize="25"
            DisplayMode="Image"
            ImageSource="add.png" />
    </tabView:SfTabView.CenterButtonSettings>
    
    <!-- Tab items here -->
</tabView:SfTabView>
```

C# Code:
```csharp
SfTabView tabView = new SfTabView();
tabView.IsCenterButtonEnabled = true;

var centerButtonSettings = new CenterButtonSettings()
{
    Height = 45,
    Width = 45,
    CornerRadius = new CornerRadius(50),
    Background = Color.FromArgb("#6750A4"),
    Stroke = Color.FromArgb("#3700B3"),
    StrokeThickness = 2,
    TextColor = Colors.White,
    FontSize = 14,
    Title = "+",
    ImageSize = 25,
    DisplayMode = CenterButtonDisplayMode.Image,
    ImageSource = "add.png"
};

tabView.CenterButtonSettings = centerButtonSettings;
```

---

## CenterButtonSettings Properties

### Size Properties

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| **Height** | double | Auto | Button height in pixels |
| **Width** | double | Auto | Button width in pixels |
| **CornerRadius** | CornerRadius | 0 | Corner radius for rounded edges (use 50 for circle) |

**Example - Circular Button:**
```xaml
<tabView:CenterButtonSettings Height="50" Width="50" CornerRadius="50" />
```

### Appearance Properties

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| **Background** | Color | System default | Button background color |
| **Stroke** | Color | Transparent | Button border color |
| **StrokeThickness** | double | 0 | Button border thickness in pixels |
| **TextColor** | Color | Black | Text color |
| **FontSize** | double | 14 | Text font size |
| **FontAttributes** | FontAttributes | None | Bold, Italic, or None |
| **FontFamily** | string | Default | Font family name |

**Example - Custom Colors:**
```xaml
<tabView:CenterButtonSettings 
    Background="#FF5722"
    Stroke="#D84315"
    StrokeThickness="2"
    TextColor="White"
    FontAttributes="Bold" />
```

### Text Properties

| Property | Type | Default | Description |
| **Title** | string | Empty | Text to display on button |

**Example - Text Button:**
```xaml
<tabView:CenterButtonSettings 
    Title="ADD"
    DisplayMode="Text"
    FontAttributes="Bold" />
```

### Image Properties

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| **ImageSource** | ImageSource | null | Image to display on button |
| **ImageSize** | double | 24 | Image size in pixels |
| **DisplayMode** | CenterButtonDisplayMode | Text | Display mode: Text, Image, or ImageWithTitle |

**Display Mode Options:**

```csharp
public enum CenterButtonDisplayMode
{
    Text,              // Show text only
    Image,             // Show image only
    ImageWithText     // Show image and text together
}
```

**Examples:**

```xaml
<!-- Image only -->
<tabView:CenterButtonSettings 
    ImageSource="add.png"
    ImageSize="25"
    DisplayMode="Image" />

<!-- Text only -->
<tabView:CenterButtonSettings 
    Title="+"
    DisplayMode="Text" />

<!-- Image with text -->
<tabView:CenterButtonSettings 
    ImageSource="add.png"
    ImageSize="20"
    Title="Add"
    DisplayMode="ImageWithText" />
```

---

## Complete Customization Examples

### Example 1: Floating Action Button Style

```xaml
<tabView:SfTabView IsCenterButtonEnabled="True">
    <tabView:SfTabView.CenterButtonSettings>
        <tabView:CenterButtonSettings 
            Height="56" 
            Width="56" 
            CornerRadius="56"
            Background="#FF6F00"
            Stroke="Transparent"
            ImageSize="28"
            DisplayMode="Image"
            ImageSource="plus.png" />
    </tabView:SfTabView.CenterButtonSettings>
    
    <tabView:SfTabView.Items>
        <!-- Tab items -->
    </tabView:SfTabView.Items>
</tabView:SfTabView>
```

C# Code:
```csharp
var settings = new CenterButtonSettings()
{
    Height = 56,
    Width = 56,
    CornerRadius = new CornerRadius(56),
    Background = Color.FromArgb("#FF6F00"),
    ImageSize = 28,
    DisplayMode = CenterButtonDisplayMode.Image,
    ImageSource = "plus.png"
};
```

### Example 2: Material Design Button

```xaml
<tabView:CenterButtonSettings 
    Height="48" 
    Width="48" 
    CornerRadius="48"
    Background="#2196F3"
    TextColor="White"
    Title="+"
    FontSize="28"
    FontAttributes="Bold"
    DisplayMode="Text" />
```

### Example 3: Pill-Shaped Button with Icon and Text

```xaml
<tabView:CenterButtonSettings 
    Height="40" 
    Width="120" 
    CornerRadius="20"
    Background="#4CAF50"
    TextColor="White"
    Title="Create"
    ImageSource="create.png"
    ImageSize="18"
    DisplayMode="ImageWithText"
    FontAttributes="Bold" />
```

### Example 4: Styled with Border

```xaml
<tabView:CenterButtonSettings 
    Height="44" 
    Width="44" 
    CornerRadius="44"
    Background="White"
    Stroke="#1976D2"
    StrokeThickness="2"
    TextColor="#1976D2"
    Title="+"
    FontSize="24"
    FontAttributes="Bold"
    DisplayMode="Text" />
```

---

## Handling Center Button Events

### CenterButtonTapped Event

Subscribe to the `CenterButtonTapped` event to handle button clicks:

```xaml
<tabView:SfTabView 
    IsCenterButtonEnabled="True"
    CenterButtonTapped="OnCenterButtonTapped">
    <!-- Tab items -->
</tabView:SfTabView>
```

C# Event Handler:
```csharp
private void OnCenterButtonTapped(object sender, EventArgs e)
{
    DisplayAlert("Action", "Center button was tapped!", "OK");
}
```

### Event Handler in Code

```csharp
SfTabView tabView = new SfTabView();
tabView.IsCenterButtonEnabled = true;
tabView.CenterButtonTapped += OnCenterButtonTapped;

private void OnCenterButtonTapped(object sender, EventArgs e)
{
    // Handle center button tap
    // Typically used for adding new items, creating content, etc.
}
```

---

## Common Use Cases

### Use Case 1: Add New Item Action

```csharp
private void OnCenterButtonTapped(object sender, EventArgs e)
{
    // Navigate to add new item screen
    Shell.Current.GoToAsync("additem");
}
```

### Use Case 2: Show Action Dialog

```csharp
private async void OnCenterButtonTapped(object sender, EventArgs e)
{
    var action = await DisplayActionSheet(
        "Choose action", 
        "Cancel", 
        null, 
        "Create New", 
        "Import", 
        "Settings");
    
    if (action == "Create New")
    {
        // Create new item
    }
    else if (action == "Import")
    {
        // Import action
    }
}
```

### Use Case 3: Show Modal Dialog

```csharp
private async void OnCenterButtonTapped(object sender, EventArgs e)
{
    var modalPage = new AddItemPage();
    await Shell.Current.Navigation.PushModalAsync(modalPage);
}
```

### Use Case 4: Dynamic Badge or Counter

```xaml
<tabView:SfTabView x:Name="tabView" IsCenterButtonEnabled="True">
    <tabView:SfTabView.CenterButtonSettings>
        <tabView:CenterButtonSettings 
            Height="50"
            Width="50"
            CornerRadius="50"
            Background="#FF5722"
            Title="{Binding BadgeCount}"
            DisplayMode="Text"
            TextColor="White"
            FontSize="16"
            FontAttributes="Bold" />
    </tabView:SfTabView.CenterButtonSettings>
</tabView:SfTabView>
```

---

## Best Practices

1. **Consistent Size** - Keep center button size consistent (typically 40-56 dp)
2. **Clear Icon** - Use recognizable icons for image mode
3. **Accessible Text** - If text is shown, make it short and clear ("+" is ideal)
4. **Color Contrast** - Ensure text and background have sufficient contrast
5. **Responsive Action** - Center button should always have a clear action
6. **Mobile Considerations** - Test tap target size on actual devices (minimum 48x48 dp recommended)
7. **Disable When Not Applicable** - Hide center button when no action is available (`IsCenterButtonEnabled = false`)

---

## Troubleshooting

| Issue | Cause | Solution |
|-------|-------|----------|
| Center button not visible | IsCenterButtonEnabled is false | Set `IsCenterButtonEnabled="True"` |
| Image not showing | Wrong image file path | Verify image exists in project resources |
| Text truncated | Button too small | Increase Width and Height properties |
| Click not registered | Event not subscribed | Add `CenterButtonTapped` event handler |
| Styling not applied | Wrong property names | Verify property names match CenterButtonSettings |

---