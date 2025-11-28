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

## ✨ Fitur Utama

### 📊 Dashboard
Dashboard yang clean dengan statistik real-time, grafik penjualan, dan quick actions. Langsung tau kondisi bisnis dalam sekali lihat.

### 💼 Sales Management
- **Lead Management** - Tracking calon customer dari awal sampai closing
- **Quotation** - Bikin penawaran harga yang rapi
- **Sales Order** - Proses order dari draft sampai delivered
- **Customer Database** - Data pelanggan lengkap dengan history transaksi

### 🛒 Purchasing
- **Purchase Request** - Request pembelian internal
- **Purchase Order** - PO ke supplier
- **Goods Receiving** - Penerimaan barang
- **Supplier Management** - Database supplier

### 📦 Inventory
- **Product Master** - Katalog produk dengan SKU
- **Stock Control** - Stok real-time per gudang
- **Stock Opname** - Penyesuaian stok
- **Transfer Gudang** - Mutasi antar lokasi

### �icing Produksi
- **Bill of Materials** - Resep/formula produk
- **Work Order** - Perintah kerja produksi
- **Manufacturing Plan** - Perencanaan produksi
- **Quality Control** - Inspeksi kualitas

### 💰 Finance
- **Chart of Accounts** - Struktur akun fleksibel
- **Journal Entry** - Jurnal umum
- **AR/AP** - Piutang & hutang
- **Laporan Keuangan** - Laba rugi, neraca, cash flow

### 📄 Document Management
Ini fitur favorit gue! **Visual Template Designer** yang mirip Accurate 5:
- Drag & drop element
- Resize dengan 8 handle
- Grid & snap untuk alignment presisi
- Ruler horizontal & vertikal
- Undo/Redo sampai 50 langkah
- Export/Import template JSON
- Generate PDF langsung

### 👥 HR & Payroll
- Data karyawan
- Absensi
- Cuti
- Slip gaji

---

## 🎨 Template Designer

Fitur andalan yang bikin dokumen bisnis jadi gampang didesain:

```
┌─────────────────────────────────────┐
│  📐 Ruler (mm)                      │
├─────────────────────────────────────┤
│  ┌─────────────────────────────┐    │
│  │     TITLE BAND              │    │
│  ├─────────────────────────────┤    │
│  │     PAGE HEADER             │    │
│  ├─────────────────────────────┤    │
│  │     DETAIL (loop data)      │    │
│  ├─────────────────────────────┤    │
│  │     SUMMARY                 │    │
│  ├─────────────────────────────┤    │
│  │     PAGE FOOTER             │    │
│  └─────────────────────────────┘    │
└─────────────────────────────────────┘
```

**Keyboard Shortcuts:**
| Shortcut | Fungsi |
|----------|--------|
| `Ctrl+C` | Copy |
| `Ctrl+V` | Paste |
| `Ctrl+Z` | Undo |
| `Ctrl+Y` | Redo |
| `Ctrl+S` | Save |
| `Ctrl+P` | Preview |
| `Delete` | Hapus element |
| `Arrow` | Geser 1mm |
| `Shift+Arrow` | Geser 5mm |

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
