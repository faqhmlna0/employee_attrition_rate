# Proyek Akhir: Menyelesaikan Permasalahan Human Resources Jaya Jaya Maju

## Business Understanding
Jaya Jaya Maju adalah perusahaan multinasional dengan lebih dari 1000 karyawan. Namun, perusahaan menghadapi tantangan serius dalam hal pengelolaan karyawan, salah satunya adalah tingginya tingkat attrition (rasio karyawan keluar). Saat ini, attrition rate mencapai lebih dari 10% yang dikhawatirkan dapat memengaruhi performa perusahaan secara keseluruhan.

[Data Source:](https://github.com/faqhmlna0/employee_attrition_rate/blob/main/employee_data.csv)

### Permasalahan Bisnis
- Tingginya tingkat attrition yang sulit dikendalikan.
- Tim HR kesulitan mengidentifikasi faktor-faktor utama yang menyebabkan karyawan keluar.
- Tidak tersedia alat bantu visual atau sistematis untuk memonitor dan menganalisis data karyawan secara efektif.

### Cakupan Proyek
- Melakukan eksplorasi dan analisis terhadap data karyawan untuk mengidentifikasi pola attrition.
- Menyusun business dashboard interaktif berbasis data untuk membantu tim HR dalam pengambilan keputusan strategis.

### Persiapan
Cara Menjalankan di Google Colab

- Buka file notebook .ipynb menggunakan Google Colab.
- Pastikan runtime Colab diatur ke GPU (jika dibutuhkan).
- Jalankan sel-sel kode secara berurutan.

Untuk proyek ini saya hanya melakukan analisis data saja tanpa menggunakan model machine learning.

Setup Environment
Proyek ini dikembangkan dan dijalankan menggunakan Google Colaboratory (Colab) untuk kemudahan akses cloud, runtime GPU, serta kolaborasi. Namun, seluruh kode dan dependensi telah disusun sedemikian rupa agar tetap dapat dijalankan secara lokal menggunakan Visual Studio Code (VS Code).

Cara Menjalankan di VS Code
- Buat dan aktifkan virtual environment (opsional namun direkomendasikan):

Untuk Linux/Mac:
python -m venv venv
source venv/bin/activate

Untuk Windows:
python -m venv venv
.\venv\Scripts\activate

- Install semua dependensi dari file requirements.txt:

pip install -r requirements.txt

## Business Dashboard

Business dashboard dibangun menggunakan Google Looker Studio untuk membantu HR menganalisis attrition karyawan. Data diklasifikasikan berdasarkan usia, status pernikahan, serta apakah karyawan bekerja lembur, dengan metrik utama meliputi jumlah total karyawan, rata-rata usia, dan rata-rata kepuasan kerja.

[Link Dashboard:](https://lookerstudio.google.com/reporting/78e2d3f5-90bc-4c81-a32e-943e782d94f2)

Berdasarkan dashboard yang telah dibuat didapatkan beberapa hal penting yang perlu di pertimbangkan sebagai berikut:

## Dashboard
- Total Karyawan: 1,058 orang, terdiri dari 620 laki-laki dan 438 perempuan.
- Rata-rata Usia Karyawan: 37.06 tahun, menandakan mayoritas karyawan berada pada usia produktif dan matang secara karier.

Distribusi Attrition:
- Tingkat attrition sebesar 16.9%, yang berarti sebagian kecil karyawan telah meninggalkan perusahaan.
- Ditampilkan dalam bentuk pie chart, mayoritas karyawan (83.1%) masih aktif bekerja.

Attrition Berdasarkan Departemen:
- Departemen dengan jumlah attrition tertinggi adalah Research & Development, diikuti oleh Sales.
- Namun secara persentase, departemen dengan rasio attrition paling tinggi adalah Sales, karena proporsi keluarnya lebih besar dari total pegawai departemen tersebut.

Attrition Berdasarkan Overtime:
- Karyawan yang bekerja lembur memiliki tingkat attrition yang jauh lebih tinggi dibanding yang tidak lembur.
- Ini mengindikasikan bahwa beban kerja tambahan berpengaruh besar terhadap keputusan karyawan untuk resign.

Attrition Berdasarkan Bidang Pendidikan:
- Meskipun distribusi relatif merata, terlihat bahwa attrition sedikit lebih tinggi pada bidang dengan latar belakang pendidikan yang lebih rendah.

Attrition Berdasarkan Work-Life Balance:
- Tingkat attrition lebih tinggi pada karyawan dengan penilaian work-life balance rendah, memperkuat pentingnya keseimbangan antara kehidupan kerja dan pribadi.

## Conclusion

Melalui analisis data, diperoleh beberapa insight utama:
- Tingkat attrition tercatat sebesar 16.9%, dengan mayoritas karyawan (83.1%) masih aktif bekerja.
- Karyawan laki-laki mendominasi jumlah karyawan, namun attrition relatif tersebar di kedua gender.
- Departemen Sales memiliki proporsi attrition tertinggi dibandingkan departemen lain, mengindikasikan tekanan atau tantangan yang lebih besar pada divisi ini.
- Karyawan yang lembur (Overtime) memiliki risiko attrition yang jauh lebih tinggi, memperlihatkan bahwa workload berlebih berdampak signifikan pada keputusan resign.
- Work-Life Balance yang buruk berkorelasi dengan tingginya attrition—karyawan yang menilai keseimbangan kerjanya rendah lebih banyak keluar.
- Bidang pendidikan dan tingkat pendidikan juga menunjukkan variasi tingkat attrition, meskipun tidak terlalu signifikan dibanding faktor lembur dan departemen.

### Rekomendasi Action Items 

Untuk mengurangi tingkat attrition dan meningkatkan retensi karyawan, berikut beberapa rekomendasi yang dapat diterapkan oleh tim HR:
1. Evaluasi Beban Kerja pada Divisi Sales dan R&D, Tinjau ulang ekspektasi, target, serta dukungan kerja di divisi dengan tingkat attrition tinggi.
2. Manajemen Lembur yang Lebih Ketat dan Terukur, Buat kebijakan pembatasan lembur dan insentif kompensasi yang adil agar tidak menjadi penyebab burnout.
3. Perkuat Program Work-Life Balance, Fasilitasi program fleksibilitas kerja, cuti tambahan, dan sesi wellbeing untuk karyawan yang merasa beban hidup-kerjanya tidak seimbang.
4. Pemetaan Risiko Attrition Berdasarkan Profil Karyawan, Gunakan dashboard ini secara aktif untuk mengidentifikasi kelompok rentan (misal: usia tertentu, status lembur, departemen) dan lakukan intervensi dini.
5. Pendekatan Personal dan Retensi di Level Awal Karier, Sediakan jalur karier dan mentoring khusus untuk posisi entry-level, agar mereka merasa diperhatikan dan berkembang.
6. Monitoring Real-Time oleh Tim HR, Manfaatkan dashboard sebagai alat pemantauan attrition secara berkala, dan integrasikan feedback karyawan dalam pengambilan keputusan.
