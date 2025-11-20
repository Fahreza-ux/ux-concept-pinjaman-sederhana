# Wireframe Description (Text-Based)

## Screen 1: Home/Dashboard

### Layout
- **Header**: Logo app + profile icon
- **Main Content**: 
  - Saldo overview (jika sudah ada pinjaman)
  - Quick action: "Ajukan Pinjaman Baru"
  - Loan calculator widget
- **Bottom Navigation**: Home, My Loans, Calculator, Profile

### Content
- Welcome message dengan nama user
- Progress bar untuk pinjaman aktif (jika ada)
- CTA button besar "Ajukan Pinjaman"

## Screen 2: Loan Calculator

### Layout
- **Header**: Back button + "Hitung Pinjaman"
- **Interactive Elements**:
  - Slider untuk jumlah pinjaman (1-50 juta)
  - Slider untuk tenor (3-24 bulan)
  - Toggle untuk jenis bunga
- **Result Section**:
  - Angsuran per bulan
  - Total pembayaran
  - Total bunga

### User Flow
User bisa adjust slider dan langsung lihat hasil perhitungan

## Screen 3: Step-by-Step Application

### Step 1: Personal Information
- Nama, email, phone (basic info)
- Progress: 25%

### Step 2: Employment & Income
- Pekerjaan, penghasilan bulanan
- Progress: 50%

### Step 3: Loan Details
- Jumlah & tenor (pre-filled dari calculator)
- Tujuan pinjaman
- Progress: 75%

### Step 4: Review & Submit
- Summary semua informasi
- Checkbox persetujuan
- Progress: 100%

## Screen 4: Application Status

### States
- **Submitted**: "Pengajuan diterima"
- **Processing**: "Sedang diproses" + progress bar
- **Approved**: "Disetujui" + dana transfer timeline
- **Rejected**: "Tidak disetujui" + alasan jelas
