# KIRANA Omnichannel Performance Intelligence
### Dashboard Keputusan Realokasi Promo dan Perbaikan Kinerja H2 2026

## 1. Project Overview

**KIRANA Omnichannel Performance Intelligence** merupakan proyek Business Intelligence (BI) yang dirancang untuk mendukung pengambilan keputusan bisnis terkait realokasi anggaran promosi dan perbaikan kinerja penjualan pada semester kedua (H2) tahun 2026.

KIRANA Home & Living, atau PT Kirana Mitra Retailindo, merupakan perusahaan ritel fiktif yang berdiri sejak 2019. Perusahaan menjual berbagai produk home & living, termasuk perlengkapan dapur, dekorasi, bedding, elektronik rumah tangga, fashion, dan perawatan diri.

Operasional penjualan dilakukan melalui **18 toko fisik di Jawa, Bali, dan Sumatera**, serta tiga kanal digital: Website, Mobile App, dan Marketplace.

Sepanjang periode 2024 hingga Juni 2026, penjualan perusahaan menunjukkan pertumbuhan. Namun, pertumbuhan tersebut belum sepenuhnya menghasilkan kinerja bisnis yang sehat. Margin kotor cenderung menurun, pencapaian target berbeda antar-channel dan region, serta terdapat ketidaksesuaian angka penjualan antara tim komersial dan finance.

Kondisi ini diperburuk oleh data yang tersebar pada berbagai sumber, seperti export POS toko, platform e-commerce, master produk, data member, retur, promosi, biaya channel, dan file Excel target yang belum terintegrasi.

Pada awal Juli 2026, Direktur Komersial membutuhkan satu sumber angka yang dapat dipercaya untuk menentukan strategi promosi dan prioritas perbaikan kinerja pada H2 2026.

## 2. Business Problem

Proyek ini berfokus pada tiga permasalahan utama:

1. **Kesenjangan pencapaian target:** Kinerja penjualan belum merata antar-channel, region, dan toko sehingga diperlukan identifikasi area yang membutuhkan intervensi.
2. **Efektivitas promosi dan profitabilitas:** Pertumbuhan revenue belum tentu menghasilkan keuntungan yang lebih baik. Promosi tertentu berpotensi meningkatkan penjualan dengan mengorbankan margin.
3. **Ketidakkonsistenan data bisnis:** Perbedaan sumber dan metode perhitungan menyebabkan angka yang digunakan tim komersial dan finance tidak selalu sama.

Permasalahan tersebut dirumuskan ke dalam tiga pertanyaan bisnis:

- Di mana kinerja berada di bawah target, dan faktor apa yang berkontribusi terhadap kesenjangan tersebut?
- Channel, kategori produk, dan mekanisme promosi mana yang menghasilkan pertumbuhan menguntungkan, dan mana yang hanya meningkatkan revenue dengan mengorbankan margin?
- Bagaimana anggaran promosi perlu dialokasikan kembali, dan toko atau region mana yang harus diprioritaskan dalam program perbaikan kinerja H2 2026?

## 3. Project Objectives

Proyek ini bertujuan membangun solusi BI end-to-end yang mengubah data operasional menjadi informasi yang konsisten, dapat ditelusuri, dan dapat digunakan dalam pengambilan keputusan bisnis.

Tujuan utamanya meliputi:

- Mengintegrasikan data dari berbagai sumber ke dalam satu model analitik yang konsisten.
- Membersihkan dan memvalidasi data untuk meningkatkan kualitas serta konsistensi angka pelaporan.
- Merancang model dimensional berbasis star schema untuk mendukung analisis penjualan, target, promosi, retur, biaya, dan profitabilitas.
- Mendefinisikan KPI dan aturan perhitungan yang tidak ambigu serta disepakati sebagai acuan bersama.
- Mengembangkan dashboard interaktif di Metabase untuk mengidentifikasi kesenjangan target, mengevaluasi efektivitas promosi, dan menentukan prioritas perbaikan.
- Menyusun insight brief berisi temuan analitis dan rekomendasi tindakan untuk keputusan H2 2026.
- Mengevaluasi tata kelola data, kualitas model, konsistensi metrik, serta keterbatasan analisis.

## 4. Scope of Analysis

Analisis diarahkan pada dimensi bisnis berikut:

| Dimensi | Fokus Analisis |
|---|---|
| Waktu | Tren penjualan dan kinerja selama 2024 hingga Juni 2026 sebagai dasar evaluasi H2 2026 |
| Channel | Perbandingan kinerja Website, Mobile App, Marketplace, dan toko fisik |
| Region dan toko | Pencapaian target, kontribusi penjualan, serta identifikasi area yang membutuhkan perbaikan |
| Kategori produk | Kontribusi revenue, margin, dan kinerja kategori |
| Promosi | Evaluasi kinerja berdasarkan jenis atau mekanisme promosi |
| Profitabilitas | Analisis margin dan dampak retur serta biaya channel sesuai ketersediaan dan definisi data |
| Target | Perbandingan aktual terhadap target dengan periode dan cakupan yang sebanding |

Analisis historis digunakan sebagai dasar penyusunan rekomendasi untuk H2 2026. Rekomendasi harus mempertimbangkan kualitas data, ketersediaan metrik, dan batasan interpretasi yang relevan.

## 5. Role and Stakeholders

Dalam proyek ini, mahasiswa berperan sebagai **BI Analyst / Analytics Engineer** di tim Data & Analytics.

| Stakeholder | Kebutuhan Utama |
|---|---|
| Direktur Komersial | Menentukan realokasi anggaran promosi dan prioritas perbaikan kinerja |
| Head of Store Operations | Mengidentifikasi toko atau region dengan kinerja di bawah target |
| Head of E-Commerce | Mengevaluasi performa kanal digital dan efektivitas promosi |
| Finance Controller | Memastikan konsistensi angka, definisi KPI, serta transparansi perhitungan |

Solusi yang dibangun harus dapat digunakan sebagai dasar diskusi bersama lintas fungsi, bukan hanya sebagai laporan deskriptif.

## 6. Proposed BI Solution

Solusi dikembangkan melalui rangkaian proses BI end-to-end:

1. **Data ingestion:** Memuat data mentah dari sumber operasional dan file target ke lingkungan analitik.
2. **Data preparation:** Melakukan pembersihan, standardisasi, penanganan data duplikat atau tidak valid, serta pemeriksaan integritas data.
3. **Dimensional modeling:** Menyusun fact table dan dimension table berdasarkan grain yang jelas, hubungan antartabel, dan kebutuhan analisis bisnis.
4. **KPI definition:** Menetapkan definisi metrik, formula, aturan agregasi, dan perlakuan terhadap retur, diskon, biaya, serta target.
5. **Data validation:** Menguji kualitas data, konsistensi perhitungan, dan rekonsiliasi angka terhadap sumber yang tersedia.
6. **Dashboard development:** Membangun dashboard interaktif di Metabase untuk analisis performa dan dukungan keputusan.
7. **Insight and recommendation:** Menyusun insight brief yang menghubungkan hasil analisis dengan tindakan bisnis yang dapat dipertimbangkan.
8. **Governance evaluation:** Mendokumentasikan lineage data, definisi KPI, keterbatasan data, serta kontrol kualitas yang diperlukan.

### Proposed Dashboard Focus

Dashboard dirancang untuk mendukung tiga area keputusan:

- **Performance Monitoring:** Memantau pencapaian target dan mengidentifikasi kesenjangan kinerja antar-channel, region, toko, serta kategori produk.
- **Promotion and Profitability Analysis:** Mengevaluasi hubungan antara aktivitas promosi, pertumbuhan penjualan, dan margin untuk membantu menentukan prioritas alokasi anggaran.
- **Business Improvement Prioritization:** Menentukan toko atau region yang perlu dievaluasi lebih lanjut berdasarkan pencapaian target, tren kinerja, dan indikator profitabilitas.

Dashboard diharapkan tidak hanya menyajikan angka, tetapi juga memudahkan stakeholder menelusuri faktor yang berkontribusi terhadap hasil bisnis dan membandingkan alternatif tindakan.

## 7. Technology Stack

| Teknologi | Fungsi |
|---|---|
| DuckDB | Memuat, membersihkan, memodelkan, dan menguji data menggunakan SQL |
| Metabase Self-hosted | Membangun dashboard interaktif dan menghasilkan ekspor PDF |
| PostgreSQL (alternatif) | Menyediakan backend database untuk Metabase apabila driver DuckDB tidak dapat digunakan |
| dbdiagram.io | Mendokumentasikan star schema dan merancang wireframe dashboard |
| SQL | Mengimplementasikan transformasi data, model dimensional, KPI, dan validasi |

Pemilihan koneksi database untuk Metabase disesuaikan dengan kompatibilitas driver dan kebutuhan implementasi. PostgreSQL merupakan alternatif teknis, bukan pengganti otomatis bagi DuckDB dalam proses transformasi data.

## 8. Project Deliverables

Output akhir proyek terdiri atas:

| Deliverable | Isi |
|---|---|
| SQL Scripts | Skrip DuckDB untuk ingestion, transformasi, pemodelan, definisi metrik, dan pengujian data |
| Dimensional Model | Dokumentasi star schema, grain tabel, relasi, dan definisi fact serta dimension |
| Metabase Dashboard | Dashboard interaktif untuk analisis kinerja penjualan, target, promosi, dan profitabilitas |
| Dashboard PDF Export | Ekspor dashboard untuk kebutuhan dokumentasi dan presentasi |
| Technical Documentation | Penjelasan sumber data, pipeline, transformasi, model, definisi KPI, dan hasil validasi |
| Insight Brief | Ringkasan temuan, implikasi bisnis, dan rekomendasi keputusan untuk H2 2026 |
| Governance Evaluation | Evaluasi kualitas data, rekonsiliasi, lineage, konsistensi metrik, keterbatasan, dan kontrol yang disarankan |

## 9. Success Criteria

Keberhasilan proyek dievaluasi berdasarkan kemampuan solusi untuk:

- Menghasilkan angka yang konsisten dan dapat ditelusuri ke sumber data.
- Memiliki model dimensional dengan grain, relasi, dan aturan agregasi yang jelas.
- Menyediakan KPI dengan definisi dan formula yang terdokumentasi.
- Menampilkan kesenjangan pencapaian target dan perbedaan kinerja antarsegmen bisnis.
- Membantu mengevaluasi efektivitas promosi dengan mempertimbangkan profitabilitas, bukan revenue semata.
- Menghasilkan rekomendasi realokasi promosi dan prioritas perbaikan yang didukung bukti analitis.
- Mendokumentasikan keterbatasan data serta aspek tata kelola yang memengaruhi interpretasi hasil.

## 10. Project Limitations and Governance

Hasil analisis bergantung pada kelengkapan, konsistensi, dan kualitas data sumber. Perbedaan grain, definisi transaksi, perlakuan retur, diskon, biaya channel, serta cakupan target perlu diperiksa sebelum metrik dibandingkan.

Setiap KPI harus memiliki definisi yang eksplisit, termasuk numerator, denominator jika relevan, periode pengukuran, satuan, dan aturan agregasinya. Proses rekonsiliasi juga perlu menjelaskan perbedaan antara angka sumber dan angka hasil transformasi.

Selain itu, hubungan antara promosi dan perubahan kinerja tidak otomatis membuktikan hubungan sebab-akibat. Rekomendasi realokasi anggaran perlu mempertimbangkan konteks operasional, periode promosi, ketersediaan stok, dan faktor lain yang dapat memengaruhi hasil.

Karena KIRANA Home & Living merupakan skenario perusahaan fiktif, hasil proyek digunakan sebagai simulasi analisis dan pengambilan keputusan bisnis.

## 11. Expected Business Outcome

Melalui KIRANA Omnichannel Performance Intelligence, manajemen diharapkan memperoleh satu acuan analitik yang konsisten untuk:

- Memahami sumber kesenjangan pencapaian target.
- Membedakan pertumbuhan penjualan dari pertumbuhan yang menguntungkan.
- Mengevaluasi prioritas promosi berdasarkan performa dan margin.
- Mengidentifikasi toko atau region yang membutuhkan program perbaikan.
- Mendukung diskusi keputusan H2 2026 menggunakan metrik, visualisasi, dan rekomendasi yang dapat ditelusuri.

Pada akhirnya, proyek ini menunjukkan bagaimana integrasi data, dimensional modeling, definisi KPI, dashboard interaktif, dan tata kelola data dapat diterapkan untuk mendukung keputusan bisnis yang lebih terukur.

---

*Project type:* Business Intelligence & Analytics Engineering  
*Business domain:* Omnichannel Retail  
*Primary tools:* DuckDB, SQL, Metabase, dbdiagram.io  
*Decision focus:* Promotion Budget Reallocation & Store Performance Improvement, H2 2026
