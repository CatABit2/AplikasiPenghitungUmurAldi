# AplikasiPenghitungUmurAldi
Latihan 2 - M. Aldi Ripandi (2210010610)

---

# Aplikasi Penghitung Umur (NetBeans, Java Swing)

Aplikasi desktop sederhana untuk menghitung umur berdasarkan tanggal lahir. Dibuat menggunakan Java Swing dan struktur proyek NetBeans (Ant).

## Fitur

* Input tanggal lahir
* Hasil umur dalam format Tahun, Bulan, Hari
* Tombol Hitung dan Bersihkan
* Validasi input dasar dan pesan kesalahan yang jelas
* Antarmuka sederhana berbasis JFrame (Java Swing)

## Prasyarat

* JDK 8 atau lebih baru (disarankan 11/17)
* NetBeans IDE (atau IDE lain yang mendukung proyek Ant)
* OS: Windows, macOS, atau Linux

## Cara Menjalankan (NetBeans)

1. Clone repo ini atau download ZIP:

   * `git clone https://github.com/CatABit2/AplikasiPenghitungUmurAldi.git`
2. Buka NetBeans → File → Open Project → arahkan ke folder `AplikasiPenghitungUmurAldi`.
3. Pastikan JDK sudah terdeteksi NetBeans.
4. Klik kanan proyek → Run.

## Cara Build via Ant (opsional)

* Di root proyek tersedia `build.xml`.
* Jalankan:

  * `ant clean`
  * `ant jar`
* Hasil JAR akan muncul di folder `dist/`.

## Struktur Proyek (ringkas)

```
AplikasiPenghitungUmurAldi/
├─ nbproject/           # metadata NetBeans
├─ src/                 # kode sumber Java (JFrame, event, logika)
├─ build.xml            # skrip Ant
├─ manifest.mf          # manifest untuk JAR
└─ build/, dist/        # hasil build (tergenerate)
```

## Penjelasan Teknis Singkat

* **UI**: JFrame + komponen Swing (label, text field/tanggal, tombol).
* **Logika**: ambil tanggal lahir, bandingkan dengan tanggal hari ini, hitung selisih sebagai tahun, bulan, dan hari.
* **Validasi**:

  * Tanggal tidak boleh kosong.
  * Tanggal lahir tidak boleh di masa depan.
  * Tampilkan dialog/informasi kesalahan jika input tidak valid.

## Panduan Penggunaan

1. Masukkan tanggal lahir pada field yang tersedia.
2. Tekan tombol **Hitung**.
3. Aplikasi menampilkan umur dalam Tahun, Bulan, dan Hari.
4. Tekan **Bersihkan** untuk reset input dan output.

## Troubleshooting

* **NetBeans tidak mendeteksi JDK**: periksa Tools → Java Platforms, tambahkan path JDK.
* **Build gagal**: jalankan `ant clean` lalu `ant jar`, atau `Clean and Build` dari NetBeans.
* **Font/UI tidak konsisten**: itu hanya tampilan; fungsi tetap berjalan.

## Lisensi

Untuk keperluan pembelajaran/akademik.

## Kredit

* Penulis: M. Aldi Ripandi

---
