# Changelog

All notable changes to this project will be documented in this file.

## [1.0.0] - 2024-11-28

### Added
- 🎨 **Visual Template Designer**
  - Band-based layout (Title, Header, Detail, Summary, Footer)
  - Drag & drop field placement
  - 8-point resize handles
  - Grid overlay with snap-to-grid
  - Horizontal & vertical rulers (mm)
  - Layer controls (bring to front/send to back)
  - Undo/Redo with 50 state history
  - Copy/Paste/Cut/Duplicate elements
  - Keyboard shortcuts
  - Export/Import template to JSON
  - PDF generation with real data
  - Preview mode with database data

- 📄 **Document Management**
  - 40+ document types (like Accurate 5)
  - Categorized document selection
  - Template library
  - PDF/Excel export

- 💼 **Sales Module Upgrade**
  - Modern Lead Management UI
  - Enhanced Sales Order list
  - Improved opportunity tracking

- 🔧 **Backend Enhancements**
  - `/api/documents/render-pdf` - PDF generation endpoint
  - `/api/documents/preview-data` - Sample data for preview
  - Template CRUD operations

### Fixed
- Unused imports cleanup
- TypeScript type errors
- Component optimization

---

## [0.9.0] - 2024-11-15

### Added
- Initial ERP system release
- Core modules: Sales, Purchasing, Inventory, Production, Finance, HR
- Dashboard with analytics
- User authentication & authorization
- Multi-language support (EN/ID)

---

## Roadmap

### Planned Features
- [ ] Mobile responsive improvements
- [ ] Advanced reporting module
- [ ] Email integration
- [ ] Barcode/QR code scanning
- [ ] API documentation (Swagger)
- [ ] Unit tests
- [ ] Docker deployment
- [ ] Cloud hosting guide
