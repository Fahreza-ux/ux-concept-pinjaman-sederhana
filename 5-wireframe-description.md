# Wireframe Descriptions (Text-Based)

## 🏠 Screen 1: Home Dashboard

### Layout Structure
- **Header**: App logo + notification icon + profile avatar
- **Main Content Area**: 
  - Welcome message dengan nama user
  - Quick loan calculator widget
  - Active loan card (jika ada)
  - Action buttons grid
- **Bottom Navigation**: Home, Loans, Help, Profile

### Content Elements
**Welcome Section**:
- "Halo, [Nama]! 👋"
- "Mau pinjam berapa hari ini?"

**Quick Calculator**:
- Amount slider: Rp 1-50 juta
- Tenor selector: 3, 6, 12, 24 bulan
- Instant calculation result: "Angsuran: Rp X/bulan"

**Action Grid**:
- "Ajukan Pinjaman Baru" (primary CTA)
- "Cek Status Pengajuan"
- "Riwayat Transaksi"
- "Bantuan & FAQ"

### User Flow
- User lands here setelah login
- Bisa langsung main dengan calculator
- One-tap access ke loan application

---

## 🧮 Screen 2: Loan Calculator

### Layout Structure
- **Header**: Back button + "Hitung Pinjaman"
- **Interactive Controls**:
  - Loan amount slider dengan visual meter
  - Tenor selector dengan bulan/tahun toggle
  - Interest type radio buttons
- **Result Panel**: Fixed bottom section
- **Action Button**: "Lanjutkan Pengajuan"

### Interactive Features
**Amount Slider**:
- Min: Rp 1,000,000 | Max: Rp 50,000,000
- Visual indicator: "Ringan" ←→ "Besar"
- Real-time calculation update

**Tenor Selector**:
- Options: 3, 6, 9, 12, 18, 24 bulan
- Visual timeline dengan bulan milestones

**Result Display**:
- "Angsuran per Bulan: Rp 1,250,000"
- "Total Pembayaran: Rp 15,000,000"
- "Total Bunga: Rp 1,500,000"

### User Experience
- Instant feedback pada setiap adjustment
- Educational tooltips untuk setiap term
- Clear visual hierarchy

---

## 📝 Screen 3: Step-by-Step Application

### Step 1: Personal Information (25%)
**Form Fields**:
- Nama lengkap (auto-filled dari profile)
- Email (auto-filled)
- Nomor HP (verified)
- Tanggal lahir (date picker)
- Alamat (auto-complete)

**Progress Indicator**: 
- Step 1 of 4 - 25% complete
- Clear navigation: "Kembali" / "Lanjut"

### Step 2: Employment & Income (50%)
**Employment Section**:
- Pekerjaan: Dropdown (Karyawan, Wiraswasta, dll)
- Nama perusahaan
- Lama bekerja
- Penghasilan bulanan: Slider Rp 1-50 juta

**Income Verification**:
- Upload slip gaji (optional)
- Bank statement (optional)

**Progress**: 50% complete

### Step 3: Loan Details (75%)
**Pre-filled dari Calculator**:
- Jumlah pinjaman: Rp 10,000,000 (bisa edit)
- Tenor: 12 bulan (bisa edit)

**Additional Information**:
- Tujuan pinjaman: Dropdown (Education, Business, Emergency, etc.)
- Hubungan dengan pinjaman sebelumnya

**Progress**: 75% complete

### Step 4: Review & Submit (100%)
**Summary Card**:
- Personal information
- Employment details  
- Loan terms
- Payment schedule

**Action Buttons**:
- "Edit" untuk setiap section
- "Setuju & Ajukan" (primary)

**Confirmation**:
- "Pengajuan diterima! Kami akan proses dalam 2 jam"

---

## 📊 Screen 4: Application Status Tracker

### Layout Structure
- **Header**: "Status Pengajuan" + application ID
- **Progress Timeline**: Vertical step indicator
- **Status Card**: Current status dengan details
- **Next Steps**: Clear action items
- **Support Section**: Contact options

### Status States
**State 1: Submitted** (0-30 menit)
```

✓ Diterima
⏳Verifikasi Data
○Analisis Kredit
○Keputusan
○Pencairan Dana

Status: Sedang verifikasi data Anda
Estimasi:30 menit lagi

```

**State 2: Under Review** (30 menit-2 jam)
```

✓ Diterima
✓Verifikasi Data
⏳Analisis Kredit
○Keputusan
○Pencairan Dana

Status: Tim kami sedang menganalisis aplikasi Anda
Estimasi:1-2 jam lagi

```

**State 3: Approved** (2-4 jam)
```

✓ Diterima
✓Verifikasi Data
✓Analisis Kredit
✓Disetujui
⏳Pencairan Dana

Status: Selamat! Pinjaman Anda disetujui
Estimasi:Dana akan cair dalam 2 jam

```
**State 4: Funds Sent** (Complete)
```

✓ Diterima
✓Verifikasi Data
✓Analisis Kredit
✓Disetujui
✓Dana Dicairkan

Status: Rp 10,000,000 telah transfer ke rekening Anda
Lanjutkan:Lihat jadwal angsuran

```
---

## 💳 Screen 5: Repayment Dashboard

### Active Loan Card
**Loan Summary**:
- "Pinjaman Aktif: Rp 10,000,000"
- "Sisa Tenor: 11 bulan"
- "Angsuran Bulanan: Rp 1,250,000"

**Next Payment**:
- "Jatuh Tempo: 15 April 2024"
- "Jumlah: Rp 1,250,000"
- Payment method: BCA •••• 1234

### Payment History
**Monthly Timeline**:
April 2024: ✓ Lunas (15 Apr)
Maret 2024:✓ Lunas (15 Mar)
Februari 2024: ✓ Lunas (15 Feb)
Januari 2024:✓ Lunas (15 Jan)

```

**Statistics**:
- Total paid: Rp 5,000,000 / Rp 15,000,000
- On-time payments: 4/4 months
- Early repayment savings: Rp 150,000

### Action Section
**Quick Actions**:
- "Bayar Sekarang"
- "Ubah Jadwal"
- "Ajukan Pelunasan Awal"
- "Download Laporan"

---

## 🎨 Design System Considerations

### Typography Scale
- **H1**: 24px • Bold • Primary text
- **H2**: 20px • Semibold • Section headers
- **Body**: 16px • Regular • Main content
- **Caption**: 14px • Regular • Secondary text

### Color Usage
- **Primary Actions**: Blue #2563EB
- **Success States**: Green #10B981  
- **Warning/Errors**: Red #DC2626
- **Disabled States**: Gray #9CA3AF

### Component Patterns
- **Cards**: Rounded corners, subtle shadow
- **Buttons**: Primary (filled), Secondary (outline)
- **Forms**: Clear labels, helpful placeholder text
- **Navigation**: Bottom tab bar dengan icons

### Accessibility Features
- **Color Contrast**: Minimum 4.5:1 ratio
- **Text Size**: Scalable tanpa breaking layout
- **Touch Targets**: Minimum 44px height
- **Screen Reader**: Semantic HTML structure

---

## 🔄 User Flow Connections

### Primary Flow: New Loan Application
Home → Calculator → Application (Step 1-4) → Status Tracker → Repayment

```

### Secondary Flows
**Quick Status Check**:

Home → Status Tracker

```
**Payment Management**:

Home → Repayment Dashboard → Payment History

```

**Educational Content**:
Home → Help & FAQ → Financial Education

```

**Next Step**: Usability testing plan untuk validate wireframes
