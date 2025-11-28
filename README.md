# 🏭 ERP Flask

<div align="center">

![ERP Flask](https://img.shields.io/badge/ERP-Flask-blue?style=for-the-badge&logo=flask)
![React](https://img.shields.io/badge/React-18.x-61DAFB?style=for-the-badge&logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript)
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python)
![TailwindCSS](https://img.shields.io/badge/Tailwind-3.x-06B6D4?style=for-the-badge&logo=tailwindcss)

**Sistem ERP modern yang dibangun dengan Flask + React**

*Dikembangkan berdasarkan bisnis proses PT. Gratia Makmur Sentosa*

[Fitur](#-fitur-utama) • [Screenshot](#-screenshot) • [Instalasi](#-cara-install) • [Tech Stack](#-tech-stack)

</div>

---

## 👋 Halo!

Gue **Mochammad Bayu Adhie Nugroho**, solo developer yang bikin sistem ERP ini dari nol. Project ini awalnya dikembangkan buat memenuhi kebutuhan operasional **PT. Gratia Makmur Sentosa**, tapi sekarang udah gue open-source biar bisa dipake dan dikembangin bareng-bareng.

Kenapa bikin ERP sendiri? Karena software ERP yang ada di pasaran seringkali:
- 💸 Mahal banget license-nya
- 🔒 Susah di-customize sesuai kebutuhan
- 📚 Ribet dan overwhelming fiturnya

Jadi gue bikin yang **simpel, modern, dan sesuai kebutuhan bisnis lokal**.

---

## ✨ Daftar Fitur Lengkap

### 📊 Dashboard & Analytics
- **Dashboard Utama** - Overview bisnis dalam satu halaman
- **Statistik Real-time** - Total penjualan, pembelian, stok, dll
- **Grafik Interaktif** - Chart penjualan harian/mingguan/bulanan
- **Top Selling Products** - Produk terlaris
- **Recent Activities** - Log aktivitas terbaru
- **Quick Actions** - Shortcut ke fitur yang sering dipake
- **Notification Center** - Notifikasi real-time
- **Multi-language** - Support Bahasa Indonesia & English

---

### 💼 Sales Management

#### Lead Management
- Capture & tracking leads
- Lead scoring (rating bintang)
- Lead source tracking (website, referral, cold call, social media, dll)
- Status management (New → Contacted → Qualified → Converted/Lost)
- Konversi lead ke opportunity
- Bulk actions (update status, delete, assign)
- Filter & search
- Grid view & table view

#### Opportunity Management
- Sales pipeline visualization
- Probability tracking
- Expected revenue calculation
- Activity timeline
- Stage management
- Win/Loss tracking

#### Quotation / Penawaran
- Buat penawaran harga
- Multi-item quotation
- Diskon per item & total
- Quotation versioning
- Convert to Sales Order
- PDF generation
- Email quotation

#### Sales Order
- Order processing workflow
- Status: Draft → Confirmed → In Progress → Ready → Shipped → Delivered
- Priority level (Low, Medium, High, Urgent)
- Multi-item orders
- Diskon & pajak
- Delivery scheduling
- Partial delivery support
- Order history

#### Customer Management
- Database pelanggan lengkap
- Contact information (multiple contacts)
- Alamat pengiriman (multiple addresses)
- Credit limit management
- Payment terms
- Transaction history
- Customer grouping/category

---

### 🛒 Purchasing

#### Purchase Request
- Internal requisition
- Approval workflow
- Budget checking
- Request status tracking
- Convert to PO

#### Purchase Order
- Vendor selection
- Price comparison
- Terms & conditions
- PO approval workflow
- Status tracking
- Partial receiving support
- PO history

#### Goods Receiving
- Receiving notes
- Quality inspection on receive
- Partial receiving
- Discrepancy handling
- Auto update stock

#### Supplier Management
- Vendor database
- Contact information
- Payment terms
- Bank account info
- Performance rating
- Transaction history

---

### 📦 Inventory Management

#### Product Master
- SKU management
- Product categories & sub-categories
- Product variants (size, color, dll)
- Barcode support
- Product images
- Unit of measure (UoM)
- Multiple UoM conversion
- Min/Max stock level
- Reorder point

#### Stock Control
- Real-time stock levels
- Multi-warehouse support
- Stock per location/bin
- Stock valuation (FIFO, LIFO, Average)
- Minimum stock alerts
- Stock aging report

#### Warehouse Management
- Multiple warehouse
- Location/bin management
- Zone management
- Warehouse transfer

#### Stock Movements
- **Stock Adjustment** - Koreksi stok
- **Stock Transfer** - Mutasi antar gudang
- **Stock Opname** - Stok opname/cycle count
- Movement history
- Audit trail

---

### 🏭 Production / Manufacturing

#### Bill of Materials (BOM)
- Multi-level BOM
- Component management
- By-product handling
- Cost calculation
- BOM versioning
- Formula/recipe management

#### Work Order
- Production scheduling
- Material requirements planning
- Labor tracking
- Machine/resource allocation
- Progress monitoring
- Status: Draft → Released → In Progress → Completed
- Partial completion

#### Manufacturing Plan
- Production planning
- Capacity planning
- Resource allocation
- Schedule optimization

#### Quality Control
- Inspection points
- Quality parameters
- Pass/Fail criteria
- Defect tracking
- QC reports

---

### 💰 Finance & Accounting

#### Chart of Accounts
- Flexible account structure
- Account types (Asset, Liability, Equity, Revenue, Expense)
- Sub-accounts
- Account grouping
- Opening balance

#### Journal Entry
- Double-entry bookkeeping
- Recurring entries
- Entry templates
- Auto-reverse entries
- Attachment support

#### Accounts Receivable (AR)
- Customer invoicing
- Payment tracking
- Payment allocation
- Aging report
- Statement of account
- Dunning/reminder

#### Accounts Payable (AP)
- Vendor bills
- Payment scheduling
- Payment processing
- Aging report
- Payment history

#### Bank & Cash
- Bank account management
- Bank reconciliation
- Cash management
- Bank transfer

#### Financial Reports
- Profit & Loss Statement
- Balance Sheet
- Cash Flow Statement
- Trial Balance
- General Ledger
- Custom reports

---

### 📄 Document Management

#### Visual Template Designer
Fitur andalan! Editor visual mirip Accurate 5:
- **Band-based Layout** - Title, Page Header, Detail, Summary, Page Footer
- **Drag & Drop** - Seret field ke canvas
- **Resize Handles** - 8 titik untuk resize element
- **Grid Overlay** - Grid 5mm untuk alignment
- **Snap to Grid** - Element otomatis snap ke grid
- **Rulers** - Penggaris horizontal & vertikal (dalam mm)
- **Layer Control** - Bring to front / Send to back
- **Undo/Redo** - History sampai 50 langkah
- **Copy/Paste/Cut** - Duplikasi element
- **Keyboard Shortcuts** - Power user friendly
- **Export/Import** - Template dalam format JSON
- **Preview Mode** - Lihat hasil dengan data real
- **PDF Generation** - Generate PDF langsung

#### Tipe Dokumen (40+ jenis)

**Penjualan:**
- Surat Penawaran Penjualan
- Pesanan Penjualan
- Surat Jalan / Pengiriman Penjualan
- Faktur Penjualan
- Retur Penjualan
- Penerimaan Penjualan
- Uang Muka Penjualan
- Klaim Garansi Penjualan
- Target Penjualan

**Pembelian:**
- Permintaan Pembelian
- Pesanan Pembelian
- Penerimaan Pembelian
- Faktur Pembelian
- Retur Pembelian
- Pembayaran Pembelian
- Uang Muka Pembelian
- Klaim Garansi Pembelian

**Persediaan:**
- Pemindahan Barang
- Penyesuaian Persediaan
- Stok Opname
- Pengepakan Barang
- Pindah Aset Tetap

**Produksi:**
- Formula Produk
- Perintah Kerja Produksi
- Penyelesaian Produksi
- Penambahan Bahan Baku
- Pengambilan Bahan Baku
- Rencana Produksi
- Tahapan Produksi

**Keuangan:**
- Penerimaan Lainnya
- Pembayaran Lainnya
- Transfer Bank
- Jurnal Umum
- Beban Dibayar Dimuka
- Anggaran
- Tukar Faktur
- Penagihan Penjualan

**Pekerjaan:**
- Pekerjaan Pesanan
- Penyelesaian Pesanan

**HR:**
- Slip Gaji

---

### 👥 Human Resources

#### Employee Management
- Database karyawan
- Personal information
- Employment history
- Document storage (KTP, NPWP, dll)
- Emergency contact
- Department & position

#### Attendance
- Clock in/out
- Overtime tracking
- Late/early tracking
- Attendance reports
- Leave integration

#### Leave Management
- Leave types (cuti tahunan, sakit, dll)
- Leave balance
- Leave request
- Approval workflow
- Leave calendar

#### Payroll
- Salary components
- Allowances & deductions
- Tax calculation (PPh 21)
- BPJS calculation
- Payslip generation
- Payroll reports

---

### ⚙️ System & Settings

#### User Management
- User accounts
- Role-based access control (RBAC)
- Permission management
- User groups
- Password policy

#### Security
- JWT Authentication
- Session management
- Password encryption
- Login history
- IP whitelist (optional)

#### Audit Trail
- Activity logging
- Change tracking
- User action history
- Data versioning

#### Settings
- Company profile
- Multi-company support
- Number series/format
- Tax settings
- Currency settings
- Email settings
- Backup & restore

#### Integration
- RESTful API
- Webhook support
- Export (PDF, Excel, CSV)
- Import data
- API documentation

---

## 🎨 Template Designer Detail

```
┌─────────────────────────────────────────────────────────┐
│  📐 Ruler (mm)    0   10   20   30   40   50   60  ... │
├─────────────────────────────────────────────────────────┤
│  ┌───────────────────────────────────────────────────┐  │
│  │  TITLE BAND                                       │  │
│  │  ┌─────────────┐ ┌─────────────────────────────┐  │  │
│  │  │ Company Logo│ │ SURAT JALAN                 │  │  │
│  │  └─────────────┘ │ No: $F{deliveryNumber}      │  │  │
│  │                  └─────────────────────────────┘  │  │
│  ├───────────────────────────────────────────────────┤  │
│  │  PAGE HEADER                                      │  │
│  │  Customer: $F{customer.name}                      │  │
│  │  Alamat: $F{customer.address}                     │  │
│  ├───────────────────────────────────────────────────┤  │
│  │  DETAIL (loop untuk setiap item)                  │  │
│  │  ┌────┬────────────────┬───────┬─────────────┐    │  │
│  │  │ No │ Nama Barang    │ Qty   │ Satuan      │    │  │
│  │  ├────┼────────────────┼───────┼─────────────┤    │  │
│  │  │ 1  │ $F{item.name}  │ $F{}  │ $F{item.uom}│    │  │
│  │  └────┴────────────────┴───────┴─────────────┘    │  │
│  ├───────────────────────────────────────────────────┤  │
│  │  SUMMARY                                          │  │
│  │  Total Items: $F{totalItems}                      │  │
│  ├───────────────────────────────────────────────────┤  │
│  │  PAGE FOOTER                                      │  │
│  │  Diterima oleh: ____________  Dikirim: ________   │  │
│  └───────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────┘
```

**Keyboard Shortcuts:**
| Shortcut | Fungsi |
|----------|--------|
| `Ctrl+C` | Copy element |
| `Ctrl+V` | Paste element |
| `Ctrl+X` | Cut element |
| `Ctrl+D` | Duplicate element |
| `Ctrl+Z` | Undo |
| `Ctrl+Y` | Redo |
| `Ctrl+S` | Save template |
| `Ctrl+P` | Preview dengan data |
| `Delete` | Hapus element |
| `Arrow Keys` | Geser element 1mm |
| `Shift+Arrow` | Geser element 5mm |

---

## 📸 Screenshot

> *Coming soon - lagi nyiapin screenshot yang bagus* 😅

---

## 🚀 Cara Install

### Yang Dibutuhin
- Python 3.10+
- Node.js 18+
- Database (SQLite/PostgreSQL)

### Backend

```bash
# Clone repo
git clone https://github.com/baymngrh/erpflask2.git
cd erpflask2

# Bikin virtual environment
python -m venv venv
venv\Scripts\activate  # Windows
source venv/bin/activate  # Mac/Linux

# Install dependencies
cd backend
pip install -r requirements.txt

# Jalanin server
python app.py
```

### Frontend

```bash
cd frontend
npm install
npm run dev
```

### Akses Aplikasi
- Frontend: http://localhost:5173
- Backend: http://localhost:5000

---

## 🔧 Konfigurasi

Bikin file `.env` di folder backend:

```env
DATABASE_URL=sqlite:///erp_database.db
JWT_SECRET_KEY=ganti-dengan-secret-key-lo
FLASK_ENV=development
```

---

## 🏗️ Tech Stack

**Backend:**
- Flask (Python web framework)
- SQLAlchemy (ORM)
- JWT Authentication
- WeasyPrint (PDF generation)

**Frontend:**
- React 18 + TypeScript
- Redux Toolkit
- TailwindCSS
- React Router
- Axios

---

## 📁 Struktur Project

```
erpflask2/
├── backend/
│   ├── app.py           # Entry point
│   ├── models/          # Database models
│   ├── routes/          # API endpoints
│   └── utils/           # Helper functions
│
├── frontend/
│   ├── src/
│   │   ├── components/  # Reusable components
│   │   ├── pages/       # Halaman-halaman
│   │   ├── store/       # Redux store
│   │   └── utils/       # Utilities
│   └── package.json
│
└── README.md
```

---

## 🤝 Kontribusi

Open for contribution! Kalo mau nambahin fitur atau fix bug:

1. Fork repo ini
2. Bikin branch baru (`git checkout -b fitur-keren`)
3. Commit changes (`git commit -m 'Nambahin fitur keren'`)
4. Push (`git push origin fitur-keren`)
5. Bikin Pull Request

---

## 📄 Lisensi

MIT License - bebas dipake, dimodif, dan didistribusiin.

---

## 👨‍💻 Developer

**Mochammad Bayu Adhie Nugroho**

[![GitHub](https://img.shields.io/badge/GitHub-@baymngrh-181717?style=flat-square&logo=github)](https://github.com/baymngrh)

---

## 🙏 Credits

- Terinspirasi dari Accurate 5
- Dikembangkan untuk PT. Gratia Makmur Sentosa
- Built with ❤️ di Indonesia

---

<div align="center">

**Kalo project ini membantu, jangan lupa kasih ⭐ ya!**

*Solo project by Bayu - 2024*

</div>
