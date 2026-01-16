# RDL Report Preview

Preview RDL and RDLC reports directly in VS Code! Perfect for Business Central, Dynamics 365, and SSRS report development.

![Preview Example](images/preview-example.png)

## Features

- 📄 **Instant Preview** - See your RDL layout without deploying
- 🔢 **Dummy Data Support** - Use JSON files to populate field placeholders
- 📊 **Table Support** - Renders Tablix, nested tables, and complex layouts
- 🎨 **Styling** - Preserves fonts, colors, borders, and padding
- 📐 **Page Layout** - Shows headers, footers, and page dimensions
- 🔍 **Zoom Controls** - Scale the preview to fit your screen

## Usage

1. Open any `.rdl` or `.rdlc` file
2. Click the **Preview** button in the editor title bar
3. Or right-click the file → **Preview RDL Report**

### Using Dummy Data

Create a JSON file with the same name as your RDL file:

```
MyReport.rdl
MyReport.json  ← dummy data
```

**Example JSON:**
```json
[
    { "CustomerName": "Contoso Ltd", "Amount": 1500.00 },
    { "CustomerName": "Fabrikam Inc", "Amount": 2300.50 }
]
```

Fields are displayed as blue tags: `CustomerName` `Amount`

## Supported Elements

| Element | Support |
|---------|---------|
| Textbox | ✅ Full |
| Tablix (Tables) | ✅ Full |
| Nested Tablix | ✅ Full |
| Rectangle | ✅ Full |
| Image | ⚠️ Placeholder |
| Line | ✅ Basic |
| Chart | ⚠️ Shows placeholder |
| Gauge | ⚠️ Shows placeholder |
| Subreport | ⚠️ Shows placeholder |
| Map | ⚠️ Shows placeholder |

## Limitations

- Charts, Gauges, and Maps are shown as placeholders
- Complex expressions are displayed as field names
- Database-bound images show as placeholders
- Parameters are not supported

## Requirements

- VS Code 1.75.0 or higher

## Release Notes

### 1.0.0

- Initial release
- Full Tablix and nested table support
- Page header/footer rendering
- Zoom controls
- Dummy data support

---

**Enjoy!** If you find this extension useful, please leave a ⭐ rating!
