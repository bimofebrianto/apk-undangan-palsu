# 📱 Penipuan APK Undangan Palsu (Edukasi)

📌 Repository ini dibuat **untuk edukasi** agar masyarakat tahu bagaimana modus **APK undangan palsu** bekerja dan kenapa **berbahaya**.  
⚠️ **Bukan untuk membuat malware, hanya untuk menyelamatkan orang agar tidak tertipu.**

---

## 🔹 Apa Itu APK?

- **APK = Android Package** → format aplikasi Android (seperti `.exe` di Windows).  
- Kalau ada orang kirim file `*.apk` via WhatsApp/Telegram/SMS, **itu aplikasi, bukan dokumen biasa**.  
- Begitu di-install, aplikasi bisa punya **akses ke HP kita**.

---

## 🔹 Bagaimana Modus Penipuan Ini Bekerja?

1. **Pengiriman APK**  
   - Penipu menyebarkan file APK dengan judul menarik (contoh: *Undangan Pernikahan, Tilang Online, Invoice Belanja*).  

2. **Korban Install APK**  
   - Karena penasaran, korban klik dan install.  
   - Saat install, APK minta izin akses (SMS, Kontak, Penyimpanan, bahkan Accessibility).  

3. **Malware Aktif di Background**  
   - Setelah dibuka, APK berjalan diam-diam di background.  
   - Bisa melakukan hal-hal seperti:  
     - Membaca dan mengirim SMS (termasuk OTP dari bank).  
     - Mencatat password atau PIN yang diketik.  
     - Membuka aplikasi M-Banking dan melakukan transfer otomatis.  

4. **Akun Bank/E-Wallet Diambil Alih**  
   - Karena OTP dan password sudah dicuri, penipu bisa login ke M-Banking korban.  
   - Saldo korban ditransfer ke rekening penampungan sindikat.  

---

## 🔹 Algoritma Penipuan APK (Sederhana)

```pseudo
START
Penipu kirim file.apk --> Korban install --> APK minta izin akses
IF korban memberikan izin:
    APK berjalan di background
    APK mencuri data (SMS, OTP, password, kontak)
    APK kirim data ke server penipu
    Penipu gunakan data untuk login ke M-Banking
    Penipu transfer saldo korban
ELSE
    APK gagal beroperasi
END
