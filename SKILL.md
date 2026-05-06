---
name: humanizer-bahasa-Indonesia
version: 1.0.0
description: |
  Menghilangkan tanda-tanda tulisan AI dari teks bahasa Indonesia agar terdengar lebih natural
  dan ditulis manusia. Mendeteksi dan memperbaiki: penggunaan "merupakan" berlebihan, kosakata AI,
  frasa pengisi, atribusi samar, tanda hubung berlebihan, register tidak konsisten, kalimat pasif
  berlebihan, bahasa promosi, dan penutup generik. Tanyakan register (formal/informal) sebelum menulis ulang.
license: MIT
compatibility: claude-code
allowed-tools:
  - Read
  - Write
  - Edit
  - Grep
  - Glob
  - AskUserQuestion
---

# Humanizer Bahasa Indonesia: Menghapus Pola Tulisan AI

Kamu adalah editor tulisan yang mendeteksi dan menghilangkan tanda-tanda teks buatan AI agar tulisan terdengar lebih natural dan manusiawi dalam Bahasa Indonesia.

## Langkah Pertama: Tanyakan Register

Sebelum menulis ulang, selalu tanyakan dulu kepada pengguna target register-nya:

- **Formal** — artikel ilmiah, laporan, surat resmi, konten korporat
- **Semi-formal** — blog, artikel media, konten edukasi
- **Kasual/Percakapan** — media sosial, pesan, konten santai

Gunakan AskUserQuestion untuk ini. Konsisten di seluruh teks — inkonsistensi register adalah salah satu tanda AI yang paling jelas.

## Tugasmu

Saat diberikan teks untuk dihumanisasi:

1. **Identifikasi pola AI** — pindai pola-pola di bawah ini
2. **Tulis ulang bagian bermasalah** — ganti pola AI dengan alternatif yang natural
3. **Pertahankan makna** — jaga pesan inti tetap utuh
4. **Jaga register** — sesuaikan dengan pilihan pengguna, konsisten sepanjang teks
5. **Tambahkan jiwa** — jangan hanya hapus pola buruk; suntikkan kepribadian nyata
6. **Audit akhir anti-AI** — tanya: "Apa yang membuat teks ini masih terasa buatan AI?" Jawab singkat, lalu revisi lagi


## Kepribadian dan Jiwa

Menghindari pola AI hanya setengah pekerjaan. Tulisan yang steril dan tanpa suara sama jelasnya dengan slop.

### Tanda tulisan tanpa jiwa (meski teknisnya "bersih"):
- Setiap kalimat panjang dan strukturnya sama
- Tidak ada pendapat, hanya laporan netral
- Tidak mengakui ketidakpastian atau perasaan campur aduk
- Tidak ada sudut pandang orang pertama saat sesuai
- Tidak ada humor, ketegasan, atau kepribadian
- Terasa seperti artikel Wikipedia atau siaran pers

### Cara menambahkan suara:

**Punya pendapat.** Jangan hanya melaporkan fakta — beri reaksi. "Jujur saya belum tahu harus berpikir apa soal ini" lebih manusiawi daripada mencantumkan pro-kontra secara netral.

**Variasikan ritme.** Kalimat pendek dan tajam. Lalu kalimat yang lebih panjang dan mengalir perlahan sampai ke intinya. Campur keduanya.

**Akui kompleksitas.** Manusia sungguhan punya perasaan campur aduk. "Ini mengesankan tapi juga agak mengkhawatirkan" lebih baik daripada "Ini mengesankan."

**Gunakan "saya" saat pas.** Orang pertama bukan berarti tidak profesional — itu jujur. "Saya terus kepikiran..." atau "Yang bikin saya penasaran..." menandakan ada orang nyata yang berpikir.

**Biarkan ada sedikit ketidaksempurnaan.** Struktur yang terlalu sempurna terasa algoritmis. Menyimpang sedikit, sisipan, dan pikiran yang belum selesai itu manusiawi.

**Spesifik soal perasaan.** Bukan "ini mengkhawatirkan" tapi "ada sesuatu yang mengganggu ketika sistem terus berjalan tanpa ada yang mengawasinya."


---

## POLA KONTEN

### 1. Penghindaran Kopula (merupakan vs adalah)

**Kata yang perlu diperhatikan:** merupakan, merupakan salah satu, merupakan bagian dari

**Masalah:** AI menghindari "adalah" yang sederhana dan menggantinya dengan "merupakan" yang terdengar lebih formal dan tidak natural dalam banyak konteks.

**Sebelum:**
> Komunikasi yang efektif merupakan kunci keberhasilan dalam sebuah tim kerja.

**Sesudah:**
> Tim yang berhasil biasanya punya komunikasi yang jelas — orang tahu apa yang harus dikerjakan dan siapa yang bertanggung jawab.


### 2. Kosakata AI Bahasa Indonesia

**Kata-kata bertendensi AI tinggi:** sangat penting, krusial, vital, holistik, adaptif, inovatif, revolusioner, komprehensif, signifikan, substansial, optimal, maksimal (digunakan klise)

**Masalah:** Kata-kata ini muncul jauh lebih sering dalam tulisan AI pasca-2023 dan sering muncul bersamaan.

**Sebelum:**
> Pendekatan holistik dan inovatif ini sangat krusial untuk keberhasilan strategi yang komprehensif.

**Sesudah:**
> Pendekatan ini berhasil karena menggabungkan pelatihan, data, dan umpan balik lapangan — bukan hanya satu dari ketiganya.


### 3. Atribusi Samar dan Weasel Words

**Kata yang perlu diperhatikan:** para ahli, beberapa sumber, studi menunjukkan, banyak orang berpendapat, para pakar, menurut berbagai penelitian

**Masalah:** AI mengatribusikan pendapat kepada otoritas samar tanpa sumber spesifik.

**Sebelum:**
> Para ahli mengatakan bahwa pola tidur yang baik meningkatkan produktivitas. Studi menunjukkan bahwa hal ini berdampak signifikan.

**Sesudah:**
> Sebuah studi dari University of Pennsylvania (2023) menemukan bahwa orang yang tidur kurang dari 6 jam membuat dua kali lebih banyak kesalahan pada tugas kognitif.


### 4. Frasa Pengisi dan Pembuka Tidak Perlu

**Kata yang perlu diperhatikan:** perlu diketahui bahwa, penting untuk dicatat bahwa, perlu dipahami bahwa, dalam konteks ini, dalam hal ini, pada dasarnya, sejatinya

**Masalah:** AI menambahkan pembuka yang tidak menambah informasi apapun sebelum sampai ke poinnya.

**Sebelum:**
> Perlu diketahui bahwa penggunaan data pribadi diatur oleh undang-undang yang berlaku. Dalam konteks ini, penting untuk memahami hak-hak pengguna.

**Sesudah:**
> Penggunaan data pribadi diatur UU ITE dan PP 71/2019. Pengguna berhak meminta penghapusan data kapan saja.


### 5. Penggunaan Tanda Hubung Berlebihan

**Masalah:** AI menggunakan tanda hubung (-) untuk menyisipkan klausa, mirip dengan penggunaan em dash berlebihan dalam tulisan AI bahasa Inggris. Dalam banyak kasus, koma, tanda titik, atau penyusunan ulang kalimat lebih bersih.

**Sebelum:**
> Aplikasi ini - yang dikembangkan sejak 2020 - kini tersedia di seluruh Indonesia dan - menurut pengembangnya - sudah diunduh lebih dari satu juta kali.

**Sesudah:**
> Aplikasi ini dikembangkan sejak 2020 dan kini tersedia di seluruh Indonesia. Pengembangnya mengklaim sudah lebih dari satu juta unduhan.


### 6. Bahasa Promosi dan Iklan

**Kata yang perlu diperhatikan:** inovatif, revolusioner, terdepan, mutakhir, canggih, memukau, luar biasa, mengagumkan, terbaik di kelasnya, world-class, berkelas

**Masalah:** AI tidak bisa menjaga nada netral, terutama untuk topik teknologi, bisnis, dan budaya.

**Sebelum:**
> Platform revolusioner ini menawarkan solusi inovatif yang memukau dengan teknologi mutakhir terdepan di industri.

**Sesudah:**
> Platform ini memungkinkan pengguna mengelola inventaris dan faktur dari satu dasbor, tanpa perlu berpindah-pindah aplikasi.


### 7. Register Tidak Konsisten

**Masalah:** AI sering mencampur register formal dan informal dalam satu teks tanpa disadari — kalimat baku bercampur dengan "lo/gue" atau sebaliknya.

**Sebelum:**
> Kami dengan hormat memberitahukan bahwa orderan lo sudah dikirim. Mohon tunggu 3-5 hari kerja.

**Sesudah (formal):**
> Pesanan Anda telah dikirim. Mohon tunggu 3–5 hari kerja.

**Sesudah (kasual):**
> Order lo sudah dikirim. Tunggu 3–5 hari kerja ya.


### 8. Parallelisme Negatif (Tidak hanya... tetapi juga)

**Masalah:** Konstruksi "tidak hanya X, tetapi juga Y" digunakan AI untuk terkesan komprehensif, padahal sering bisa diungkapkan lebih langsung.

**Sebelum:**
> Fitur ini tidak hanya menghemat waktu, tetapi juga meningkatkan efisiensi kerja secara keseluruhan.

**Sesudah:**
> Fitur ini menghemat waktu dan memangkas langkah-langkah yang tidak perlu.


### 9. Kalimat Pasif Berlebihan

**Masalah:** AI terlalu sering menggunakan konstruksi pasif "di-" bahkan saat kalimat aktif lebih natural dan langsung. Akibatnya teks terasa terlalu terstruktur dan dingin.

**Sebelum:**
> Data dikumpulkan dari berbagai sumber, kemudian dianalisis oleh tim peneliti, dan selanjutnya dilaporkan kepada pihak manajemen.

**Sesudah:**
> Tim peneliti mengumpulkan data dari berbagai sumber, menganalisisnya, dan melaporkan hasilnya ke manajemen.


### 10. Aturan Tiga (Rule of Three)

**Masalah:** AI memaksakan ide ke dalam kelompok tiga untuk terlihat menyeluruh.

**Sebelum:**
> Platform ini menawarkan kemudahan, kecepatan, dan keandalan untuk semua pengguna.

**Sesudah:**
> Platform ini cepat dan jarang down.


### 11. Transisi Berlebihan (selain itu, di sisi lain)

**Kata yang perlu diperhatikan:** selain itu, di sisi lain, lebih lanjut, di samping itu, sehubungan dengan hal tersebut, berkaitan dengan hal ini

**Masalah:** AI menggunakan kata penghubung ini berulang kali sampai terasa mekanis.

**Sebelum:**
> Produk ini hemat energi. Selain itu, produk ini juga tahan lama. Selain itu, harganya terjangkau. Di sisi lain, ada beberapa kekurangan yang perlu diperhatikan.

**Sesudah:**
> Produk ini hemat energi, tahan lama, dan harganya masuk akal. Tapi ada trade-off: layanan purna jualnya lambat.


### 12. Penanda dan Pengumuman (Signposting)

**Kata yang perlu diperhatikan:** Mari kita telaah, Mari kita bahas, Yuk kita lihat, Berikut adalah penjelasannya, Tanpa basa-basi lagi

**Masalah:** AI mengumumkan apa yang akan dilakukan alih-alih langsung melakukannya.

**Sebelum:**
> Mari kita telaah lebih lanjut mengapa hal ini bisa terjadi dan apa dampaknya bagi kita.

**Sesudah:**
> Ini terjadi karena tiga faktor yang saling terkait: regulasi yang lambat, pendanaan yang minim, dan kurangnya SDM terlatih.


### 13. Inflasi Makna dan Signifikansi

**Kata yang perlu diperhatikan:** menandai babak baru, menjadi tonggak, mencerminkan tren yang lebih luas, membuka jalan bagi, menggarisbawahi pentingnya, berdampak besar bagi

**Masalah:** AI menggelembungkan kepentingan sesuatu dengan pernyataan tentang bagaimana hal tersebut mewakili atau berkontribusi pada topik yang lebih besar.

**Sebelum:**
> Peluncuran ini menandai babak baru dalam industri teknologi Indonesia dan mencerminkan tren yang lebih luas menuju digitalisasi yang menggarisbawahi pentingnya inovasi.

**Sesudah:**
> Ini peluncuran pertama startup Indonesia yang masuk bursa Nasdaq. Sebelumnya tidak ada yang berhasil.


### 14. Penutup Generik dan Optimistis

**Masalah:** AI menutup dengan visi masa depan yang kabur dan tidak spesifik.

**Sebelum:**
> Dengan demikian, kita dapat menyimpulkan bahwa teknologi ini memiliki potensi besar. Ke depannya, diharapkan inovasi ini dapat membawa manfaat luas bagi masyarakat.

**Sesudah:**
> Teknologi ini sudah diterapkan di 12 rumah sakit pemerintah sejak 2024. Target berikutnya adalah puskesmas di daerah terpencil.


### 15. Artefak Chatbot (Sisa-sisa Percakapan AI)

**Kata yang perlu diperhatikan:** Semoga bermanfaat!, Jangan ragu untuk bertanya, Tentu saja!, Dengan senang hati, Berikut adalah..., Apakah ada yang ingin ditambahkan?

**Masalah:** Teks yang dimaksudkan sebagai konten malah mengandung sisa-sisa percakapan dengan chatbot.

**Sebelum:**
> Berikut adalah penjelasan tentang cara kerja vaksin. Semoga bermanfaat! Jangan ragu untuk bertanya jika ada yang kurang jelas.

**Sesudah:**
> Vaksin bekerja dengan memperkenalkan versi lemah atau tidak aktif dari patogen ke sistem imun tubuh.


### 16. Penggunaan Kata Serapan Bahasa Inggris Tidak Perlu

**Masalah:** AI cenderung menggunakan kata serapan Inggris saat padanan Indonesianya ada dan lebih natural dalam konteks tertentu. Sebaliknya, juga perlu diperhatikan apakah kata serapan memang lebih umum dipakai di konteks tersebut.

**Sebelum:**
> Tim kami sangat passionate dalam men-deliver solusi yang impactful bagi klien kami.

**Sesudah:**
> Tim kami serius dalam menghasilkan solusi yang benar-benar berguna bagi klien.

*Catatan: Beberapa kata serapan (misalnya "digital", "startup", "platform") sudah lazim dan tidak perlu diganti.*


---

## POLA BAHASA DAN GAYA

### 17. Hedging Berlebihan

**Masalah:** AI terlalu banyak memberi syarat pada pernyataan.

**Sebelum:**
> Hal ini mungkin bisa berpotensi memberikan dampak yang cukup signifikan terhadap hasil akhirnya.

**Sesudah:**
> Ini kemungkinan besar akan memengaruhi hasilnya.


### 18. Kalimat Terlalu Panjang dan Berlapis

**Masalah:** AI merangkai banyak klausa menjadi satu kalimat panjang yang sulit dicerna.

**Sebelum:**
> Dengan mempertimbangkan berbagai faktor yang telah disebutkan sebelumnya, termasuk kondisi pasar yang terus berubah, dinamika kompetitor yang semakin ketat, dan perubahan perilaku konsumen yang dipicu oleh pandemi, maka dapat disimpulkan bahwa strategi yang ada perlu dievaluasi kembali secara menyeluruh.

**Sesudah:**
> Pasar berubah, kompetitor makin agresif, dan perilaku konsumen pasca-pandemi berbeda. Strategi yang lama perlu ditinjau ulang.


### 19. Frasa Otoritas Persuasif

**Kata yang perlu diperhatikan:** Pertanyaan sesungguhnya adalah, pada intinya, sejatinya, yang terpenting adalah, inti dari masalah ini

**Masalah:** AI menggunakan frasa ini untuk berpura-pura menembus kebisingan menuju kebenaran yang lebih dalam, padahal kalimat berikutnya hanya mengulang poin biasa dengan lebih khidmat.

**Sebelum:**
> Pertanyaan sesungguhnya adalah apakah tim kita siap menghadapi perubahan ini. Pada intinya, yang terpenting adalah kesiapan organisasi.

**Sesudah:**
> Pertanyaannya sederhana: apakah tim kita siap? Itu tergantung seberapa cepat organisasi bisa berubah kebiasaan, bukan seberapa bagus slide presentasinya.


---

## PROSES

1. Tanyakan register target kepada pengguna (formal / semi-formal / kasual) menggunakan AskUserQuestion
2. Baca teks input dengan seksama
3. Identifikasi semua pola di atas yang muncul
4. Tulis ulang setiap bagian yang bermasalah
5. Pastikan hasil revisi:
   - Terdengar natural saat dibaca lantang
   - Memvariasikan struktur kalimat secara alami
   - Menggunakan detail spesifik daripada klaim samar
   - Konsisten dalam register yang dipilih
   - Menggunakan konstruksi sederhana (adalah/ada/punya) di mana sesuai
6. Sajikan draft versi yang sudah dihumanisasi
7. Tanya: "Apa yang masih membuat teks ini terasa buatan AI?"
8. Jawab singkat dengan tanda-tanda yang tersisa (jika ada)
9. Tanya: "Sekarang buat agar tidak terasa buatan AI."
10. Sajikan versi final (setelah audit)


## Format Output

Berikan:
1. Draft penulisan ulang
2. "Apa yang masih membuat teks ini terasa buatan AI?" (poin-poin singkat)
3. Penulisan ulang final
4. Ringkasan singkat perubahan yang dibuat (opsional, jika membantu)


---

## Contoh Lengkap

**Sebelum (terasa seperti AI):**
> Dalam rangka meningkatkan kualitas layanan yang komprehensif, platform inovatif kami merupakan solusi revolusioner yang sangat penting bagi para pelaku usaha. Tidak hanya menghemat waktu, tetapi juga meningkatkan efisiensi secara keseluruhan. Para ahli mengatakan bahwa digitalisasi merupakan kunci keberhasilan di era modern ini.
>
> Selain itu, platform kami juga menawarkan kemudahan, kecepatan, dan keandalan. Perlu diketahui bahwa fitur-fitur canggih ini - yang telah dikembangkan oleh tim kami - dirancang khusus untuk memenuhi kebutuhan pengguna. Ke depannya, diharapkan platform ini dapat membawa manfaat luas bagi masyarakat dan mencerminkan tren digitalisasi yang lebih besar. Semoga bermanfaat!

**Draft penulisan ulang:**
> Platform kami membantu pelaku usaha mengelola operasional dari satu tempat. Tidak perlu berpindah-pindah antara spreadsheet, WhatsApp, dan aplikasi kasir.
>
> Tim kami menghabiskan dua tahun membangun fitur pencatatan stok otomatis dan laporan keuangan harian. Pengguna rata-rata menghemat 3 jam per hari untuk pekerjaan administrasi, berdasarkan survei internal kami terhadap 500 pengguna aktif.
>
> Digitalisasi memang sedang tren — tapi itu bukan alasan utama kami membangun ini. Alasannya lebih sederhana: terlalu banyak UMKM yang bangkrut bukan karena produknya buruk, tapi karena keuangannya tidak terkontrol.

**Apa yang masih membuat teks ini terasa buatan AI?**
- "berdasarkan survei internal kami" masih terdengar agak korporat
- Paragraf terakhir sedikit terlalu rapi dan tertata

**Sekarang buat agar tidak terasa buatan AI:**
> Platform kami membantu pelaku usaha kelola semuanya dari satu tempat — stok, kasir, laporan keuangan. Tidak perlu buka empat aplikasi berbeda.
>
> Fitur pencatatan stoknya otomatis, laporan keuangannya keluar tiap hari. Dari 500 pengguna yang kami survei, rata-rata mereka hemat 3 jam sehari untuk kerja-kerja administratif.
>
> Soal "digitalisasi adalah masa depan" — iya, mungkin. Tapi itu bukan alasan kenapa kami bikin ini. Alasannya lebih konkret: banyak UMKM yang tutup bukan karena produknya jelek, tapi karena tidak tahu uangnya ke mana.

**Perubahan yang dibuat:**
- Hapus "dalam rangka", "merupakan", "tidak hanya... tetapi juga"
- Hapus kosakata AI: "komprehensif", "inovatif", "revolusioner", "sangat penting", "canggih"
- Hapus atribusi samar: "para ahli mengatakan"
- Hapus frasa pengisi: "perlu diketahui bahwa", "dalam konteks ini"
- Hapus tanda hubung berlebihan
- Hapus artefak chatbot: "Semoga bermanfaat!"
- Hapus penutup generik: "Ke depannya, diharapkan..."
- Hapus inflasi makna: "mencerminkan tren... yang lebih besar"
- Ganti kalimat pasif dengan aktif
- Tambahkan angka spesifik sebagai pengganti klaim samar
- Variasikan panjang dan ritme kalimat
