---
title: Watermark
---

### Add Watermark

The viewer provides functionality to add text watermarks to PDF documents. You can add watermarks to all pages using the `addWatermarkToAllPages` method.

```javascript
// Add a simple watermark with default settings
RxCore.addWatermarkToAllPages("CONFIDENTIAL");

// Add a watermark with custom settings
RxCore.addWatermarkToAllPages("DRAFT", {
    position: "Center",
    rotation: 30,
    opacity: 50
});
```

#### Watermark Options

The watermark function accepts two parameters:
- `text`: The text to display as watermark
- `settings`: An optional object containing watermark configuration

Available settings with their default values:

```javascript
{
    // Watermark Position and Layout
    position: "Center",  // Position of the watermark
    offsetX: 0,         // Horizontal offset from position
    offsetY: 0,         // Vertical offset from position
    scale: 1,           // Scale factor of the watermark
    rotation: 45,       // Rotation angle in degrees
    opacity: 100,       // Opacity percentage (0-100)

    // Text Properties
    font: 2,            // Font identifier
    fontSize: 20,       // Font size in points
    color: 0x000000,    // Text color in hexadecimal
    fontStyle: "normal" // Font style
}
```

---

### Remove Watermark

To remove all watermarks from the current PDF document, you can use the `removeWatermarkFromAllPages` method:

```javascript
// Remove all watermarks from the document
RxCore.removeWatermarkFromAllPages();
```

This will remove any previously added watermarks from all pages in the document.
