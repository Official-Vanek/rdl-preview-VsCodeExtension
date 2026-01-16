# Changelog

All notable changes to "RDL Report Preview" extension.

## [1.0.0] - 2026-01-16

### Added
- Initial release
- RDL/RDLC file preview in webview panel
- Dummy data support via JSON files
- Full Tablix (table) rendering with nested table support
- Rectangle container support
- Textbox rendering with paragraph and text run support
- Page header and footer rendering
- Zoom controls (+, -, Fit)
- Field placeholder display (blue tags)
- Basic styling (fonts, colors, borders, padding)
- Support for unsupported elements as placeholders:
  - Charts (📊)
  - Gauges (🎯)
  - Subreports (📄)
  - Maps (🗺️)
- ColSpan and RowSpan support for table cells
- Page margins support
- Editor title button for quick preview
- Explorer context menu integration
- Info bar showing item and tablix counts

### Known Limitations
- Charts, Gauges, Maps rendered as placeholders only
- Complex expressions show field names instead of evaluated values
- Database-bound images show as placeholders
- Report parameters not supported
