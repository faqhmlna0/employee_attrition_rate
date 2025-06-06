# Proyek Akhir: Menyelesaikan Permasalahan Human Resources Jaya Jaya Maju

## Business Understanding
Jaya Jaya Maju adalah perusahaan multinasional dengan lebih dari 1000 karyawan. Namun, perusahaan menghadapi tantangan serius dalam hal pengelolaan karyawan, salah satunya adalah tingginya tingkat attrition (rasio karyawan keluar). Saat ini, attrition rate mencapai lebih dari 10% yang dikhawatirkan dapat memengaruhi performa perusahaan secara keseluruhan.

### Permasalahan Bisnis
- Tingginya tingkat attrition yang sulit dikendalikan.
- Tim HR kesulitan mengidentifikasi faktor-faktor utama yang menyebabkan karyawan keluar.
- Tidak tersedia alat bantu visual atau sistematis untuk memonitor dan menganalisis data karyawan secara efektif.

### Cakupan Proyek
- Melakukan eksplorasi dan analisis terhadap data karyawan untuk mengidentifikasi pola attrition.
- Membangun model prediksi risiko attrition dengan menggunakan algoritma machine learning.
- Menyusun business dashboard interaktif berbasis data untuk membantu tim HR dalam pengambilan keputusan strategis.

### Persiapan
Cara Menjalankan di Google Colab

- Buka file notebook .ipynb menggunakan Google Colab.
- Pastikan runtime Colab diatur ke GPU (jika dibutuhkan).
- Jalankan sel-sel kode secara berurutan.

## Business Dashboard

Business dashboard dibangun menggunakan Google Looker Studio untuk membantu HR menganalisis attrition karyawan. Data diklasifikasikan berdasarkan usia, status pernikahan, serta apakah karyawan bekerja lembur, dengan metrik utama meliputi jumlah total karyawan, rata-rata usia, dan rata-rata kepuasan kerja.

[Link Dashboard:](https://lookerstudio.google.com/reporting/78e2d3f5-90bc-4c81-a32e-943e782d94f2)

Berdasarkan dashboard yang telah dibuat didapatkan beberapa hal penting yang perlu di pertimbangkan sebagai berikut:

## Slide 1
![alt text](https://github.com/Sopyaan/human_resources_analysis/blob/main/dashboard/Slide1%20-%20dashboard.png?raw=true)
- Total Karyawan: 1,058 orang
- Rata-rata Usia Karyawan: 37.06 tahun
- Rata-rata Kepuasan Kerja: 2.75 / 4
- Tingkat Attrition: 16.9% dari total karyawan telah keluar dari perusahaan. Visualisasi pie chart menunjukkan bahwa mayoritas karyawan (83.1%) masih aktif.
- Grafik garis menunjukkan bahwa attrition paling sering terjadi pada kelompok usia 30–40 tahun, yang juga merupakan kelompok usia dominan dalam organisasi.
- Attrition Berdasarkan Lembur (Overtime) menunjukkan bahwa karyawan yang bekerja lembur memiliki tingkat attrition yang lebih tinggi dibandingkan yang tidak lembur.
- Tingkat attrition tertinggi terjadi pada karyawan yang belum menikah (single), sementara karyawan yang menikah cenderung lebih stabil dan loyal.

## Slide 2
![alt text](https://github.com/Sopyaan/human_resources_analysis/blob/main/dashboard/Slide2%20-%20dashboard.png?raw=true)

Analisis berdasarkan Job Level dan Years Since Last Promotion menunjukkan bahwa:
- Mayoritas attrition terjadi pada karyawan dengan Job Level 1 dan 2, yaitu posisi awal karier.
- Sebagian besar karyawan yang keluar belum pernah mendapatkan promosi atau baru bekerja kurang dari 1 tahun sejak terakhir dipromosikan.
- Pola ini mengindikasikan bahwa early attrition (keluar dalam masa awal bekerja) merupakan tantangan utama bagi organisasi.

Berdasarkan departemen, tingkat attrition tertinggi terjadi pada:
- Sales Executive, Research Scientist, dan Laboratory Technician.
- Fungsi-fungsi ini umumnya memiliki tekanan kerja tinggi, target ketat, atau ketergantungan pada performa individu.

Sebaliknya, departemen seperti Human Resources dan Research Director mencatat attrition yang jauh lebih rendah, mengindikasikan stabilitas yang lebih besar pada level strategis atau administratif.

## Conclusion

Melalui analisis data dan pemodelan, diperoleh beberapa insight utama:
- Karyawan usia 30–40 tahun, belum menikah, dan yang bekerja lembur memiliki risiko keluar lebih tinggi.
- Attrition Berdasarkan Lembur (Overtime) menunjukkan bahwa karyawan yang bekerja lembur memiliki tingkat attrition yang lebih tinggi dibandingkan yang tidak lembur.
- Jabatan di level awal karier (Job Level 1 dan 2) dan mereka yang belum pernah dipromosikan juga memiliki tingkat attrition tinggi.
- Logistic Regression digunakan sebagai model prediktif, dengan akurasi sekitar 89% dan recall yang baik untuk mendeteksi karyawan yang berpotensi keluar.
- Dashboard interaktif memudahkan tim HR dalam mengawasi faktor-faktor ini secara real time.

### Rekomendasi Action Items 

Berikan beberapa rekomendasi action items yang harus dilakukan perusahaan guna menyelesaikan permasalahan yaitu: 
- Fokus pada Karyawan Usia 30–40 Tahun: Segmentasi ini perlu mendapatkan perhatian lebih dalam hal pengembangan karier dan keseimbangan kerja-hidup.
- Evaluasi Beban Kerja: Tingginya attrition di kelompok yang bekerja lembur menandakan perlunya review terhadap kebijakan overtime.
- Perkuat Engagement Karyawan Muda & Single: Program retensi yang dipersonalisasi berdasarkan usia dan status sosial dapat membantu menurunkan tingkat attrition.
- Implementasi onboarding yang komprehensif dan mentorship program di Job Level rendah.
- Lakukan review terhadap tekanan kerja di departemen dengan attrition tinggi.
- Gunakan data analitik SDM untuk memprediksi risiko keluar dini (early attrition risk).
