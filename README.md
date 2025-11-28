# 🏭 ERP Flask - Enterprise Resource Planning System

<div align="center">

![ERP Flask Banner](https://img.shields.io/badge/ERP-Flask-blue?style=for-the-badge&logo=flask)
![React](https://img.shields.io/badge/React-18.x-61DAFB?style=for-the-badge&logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript)
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python)
![TailwindCSS](https://img.shields.io/badge/Tailwind-3.x-06B6D4?style=for-the-badge&logo=tailwindcss)

**A comprehensive, modern ERP system built with Flask backend and React frontend**

[Features](#-features) • [Demo](#-demo) • [Installation](#-installation) • [Documentation](#-documentation) • [Screenshots](#-screenshots)

</div>

---

## ✨ Features

### 📊 Dashboard & Analytics
- Real-time business metrics and KPIs
- Interactive charts and graphs
- Customizable widgets
- Multi-language support (EN/ID)

### 💼 Sales Management
- **Lead Management** - Track and convert sales leads
- **Opportunity Pipeline** - Visual sales funnel
- **Quotations** - Create and manage quotes
- **Sales Orders** - Order processing workflow
- **Customer Management** - Complete CRM functionality

### 🛒 Purchasing
- **Purchase Requests** - Internal procurement requests
- **Purchase Orders** - Vendor order management
- **Supplier Management** - Vendor database
- **Goods Receiving** - Inventory receiving

### 📦 Inventory Management
- **Product Catalog** - SKU management with variants
- **Stock Control** - Real-time inventory tracking
- **Warehouse Management** - Multi-location support
- **Stock Adjustments** - Inventory corrections
- **Stock Transfers** - Inter-warehouse movements

### �icing Production / Manufacturing
- **Bill of Materials (BOM)** - Product recipes
- **Work Orders** - Production scheduling
- **Manufacturing Plans** - Production planning
- **Quality Control** - Inspection workflows

### 💰 Finance & Accounting
- **Chart of Accounts** - Flexible account structure
- **Journal Entries** - Double-entry bookkeeping
- **Accounts Receivable** - Customer invoicing
- **Accounts Payable** - Vendor payments
- **Financial Reports** - P&L, Balance Sheet, Cash Flow

### 📄 Document Management
- **Visual Template Designer** - Drag & drop document builder
- **40+ Document Types** - Sales, Purchase, Production, Finance
- **PDF Generation** - Professional document output
- **Template Library** - Reusable document templates

### 👥 Human Resources
- **Employee Management** - Personnel database
- **Attendance Tracking** - Time & attendance
- **Leave Management** - PTO requests
- **Payroll** - Salary processing

### ⚙️ System Features
- **Role-Based Access Control** - Granular permissions
- **Audit Trail** - Complete activity logging
- **Multi-Company** - Support multiple entities
- **API Integration** - RESTful API endpoints
- **Real-time Notifications** - WebSocket updates

---

## 🎨 Template Designer

One of the standout features is our **Visual Template Designer** - similar to Accurate 5:

### Features:
- 📐 **Band-based Layout** - Title, Header, Detail, Summary, Footer
- 🖱️ **Drag & Drop** - Intuitive element placement
- 📏 **Resize Handles** - 8-point element resizing
- 📊 **Grid & Snap** - Precise alignment tools
- 📐 **Rulers** - Horizontal & vertical guides (mm)
- ↩️ **Undo/Redo** - 50 state history
- 📋 **Copy/Paste** - Element duplication
- ⌨️ **Keyboard Shortcuts** - Power user features
- 📤 **Export/Import** - JSON template sharing
- 📄 **PDF Generation** - Direct PDF output

### Keyboard Shortcuts:
| Shortcut | Action |
|----------|--------|
| `Ctrl+C` | Copy element |
| `Ctrl+V` | Paste element |
| `Ctrl+X` | Cut element |
| `Ctrl+D` | Duplicate element |
| `Ctrl+Z` | Undo |
| `Ctrl+Y` | Redo |
| `Ctrl+S` | Save template |
| `Ctrl+P` | Preview |
| `Delete` | Remove element |
| `Arrow Keys` | Move element (1mm) |
| `Shift+Arrow` | Move element (5mm) |

---

## 📸 Screenshots

### Dashboard
![Dashboard](./screenshots/dashboard.png)

### Sales Order Management
![Sales Orders](./screenshots/sales-orders.png)

### Template Designer
![Template Designer](./screenshots/template-designer.png)

### Document Preview
![Document Preview](./screenshots/document-preview.png)

### Inventory Management
![Inventory](./screenshots/inventory.png)

---

## 🚀 Installation

### Prerequisites
- Python 3.10+
- Node.js 18+
- PostgreSQL or SQLite

### Backend Setup

```bash
# Clone repository
git clone https://github.com/baymngrh/erpflask2.git
cd erpflask2

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

# Install dependencies
cd backend
pip install -r requirements.txt

# Initialize database
flask db upgrade

# Run backend server
python app.py
```

### Frontend Setup

```bash
# Navigate to frontend
cd frontend

# Install dependencies
npm install

# Start development server
npm run dev
```

### Access Application
- Frontend: http://localhost:5173
- Backend API: http://localhost:5000
- API Docs: http://localhost:5000/api/docs

---

## 🔧 Configuration

### Environment Variables

Create `.env` file in backend folder:

```env
# Database
DATABASE_URL=sqlite:///erp_database.db
# DATABASE_URL=postgresql://user:pass@localhost/erp_db

# JWT Secret
JWT_SECRET_KEY=your-super-secret-key

# Flask
FLASK_ENV=development
FLASK_DEBUG=1

# Email (optional)
MAIL_SERVER=smtp.gmail.com
MAIL_PORT=587
MAIL_USERNAME=your-email@gmail.com
MAIL_PASSWORD=your-app-password
```

---

## 📚 API Documentation

### Authentication
```http
POST /api/auth/login
Content-Type: application/json

{
  "username": "admin",
  "password": "admin123"
}
```

### Sales Orders
```http
GET /api/sales/orders
Authorization: Bearer <token>

POST /api/sales/orders
Authorization: Bearer <token>
Content-Type: application/json

{
  "customer_id": 1,
  "items": [
    {"product_id": 1, "quantity": 10, "unit_price": 50000}
  ]
}
```

### Document Templates
```http
GET /api/documents/templates
POST /api/documents/templates
POST /api/documents/render-pdf
```

---

## 🏗️ Tech Stack

### Backend
- **Flask** - Python web framework
- **SQLAlchemy** - ORM
- **Flask-JWT-Extended** - Authentication
- **WeasyPrint** - PDF generation
- **Flask-CORS** - Cross-origin support

### Frontend
- **React 18** - UI library
- **TypeScript** - Type safety
- **Redux Toolkit** - State management
- **React Router** - Navigation
- **TailwindCSS** - Styling
- **Heroicons** - Icons
- **React Hot Toast** - Notifications
- **Axios** - HTTP client

---

## 📁 Project Structure

```
erpflask2/
├── backend/
│   ├── app.py              # Flask application
│   ├── models/             # SQLAlchemy models
│   ├── routes/             # API endpoints
│   ├── utils/              # Helper functions
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   │   ├── components/     # Reusable components
│   │   ├── pages/          # Page components
│   │   ├── store/          # Redux store
│   │   ├── utils/          # Utilities
│   │   └── App.tsx
│   ├── package.json
│   └── tailwind.config.js
│
└── README.md
```

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Bayu Mangara**
- GitHub: [@baymngrh](https://github.com/baymngrh)

---

## 🙏 Acknowledgments

- Inspired by Accurate 5 ERP
- Built with modern web technologies
- Designed for Indonesian businesses

---

<div align="center">

**⭐ Star this repository if you find it helpful!**

Made with ❤️ in Indonesia

</div>
