# Bolain Ajah

Bolain Ajah adalah aplikasi kuis sepak bola berbasis Java Swing. Proyek ini dibuat sebagai tugas Pemrograman Berorientasi Objek dan dipertahankan sebagai bagian dari perjalanan belajar saya membangun aplikasi desktop dengan antarmuka grafis, event handling, dan alur permainan.

Pemain memasukkan nama, membaca peraturan, lalu menjawab sepuluh pertanyaan sepak bola dengan batas waktu. Tersedia bantuan 50:50 satu kali dan halaman hasil yang menampilkan skor akhir.

## Fitur

- Antarmuka desktop menggunakan Java Swing.
- Sepuluh pertanyaan pilihan ganda bertema sepak bola.
- Batas waktu 15 detik untuk setiap pertanyaan.
- Bantuan 50:50 yang dapat digunakan satu kali.
- Perhitungan skor dan pilihan untuk bermain kembali.
- Validasi nama pemain sebelum kuis dimulai.

## Struktur proyek

```text
src/
├── icons/
│   ├── login.jpg
│   ├── quiz.jpg
│   └── score.jpg
└── quiz/application/
    ├── Login.java
    ├── Rules.java
    ├── Quiz.java
    └── Score.java
```

## Menjalankan proyek

Proyek awal dibuat dengan NetBeans dan Ant.

### Melalui NetBeans

1. Buka folder repository sebagai proyek NetBeans.
2. Pastikan JDK telah terpasang.
3. Jalankan class `quiz.application.Login`.

### Melalui terminal

```bash
javac -d out src/quiz/application/*.java
java -cp "out;src" quiz.application.Login
```

Pada macOS/Linux, ganti pemisah classpath `;` menjadi `:`.

## Perbaikan dari versi awal

- Input nama kosong sekarang ditolak sebelum masuk ke halaman peraturan.
- State timer, nomor pertanyaan, dan skor di-reset ketika permainan baru dimulai.
- Jawaban durasi pertandingan disamakan dengan teks pilihan agar jawaban benar dihitung dengan tepat.
- Build output dan pengaturan IDE pribadi tidak lagi disimpan di Git.

## Catatan perjalanan

Struktur dan tampilan Swing dipertahankan agar karakter proyek tugas akhirnya tetap terlihat. Perbaikan difokuskan pada bug permainan, kebersihan repository, dan dokumentasi—bukan mengubahnya menjadi aplikasi dengan framework baru.
