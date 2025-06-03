# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

## Business Understanding

Jaya Jaya Maju adalah sebuah perusahaan teknologi pendidikan (edutech) yang telah berdiri sejak tahun 2000. Dalam perjalanannya, perusahaan ini berkembang pesat dan kini memiliki lebih dari seribu karyawan yang tersebar di berbagai kota. Dengan semakin banyaknya tim yang harus dikelola, tantangan di bidang sumber daya manusia pun ikut bertambah. Salah satu masalah yang mulai terlihat adalah meningkatnya jumlah karyawan yang mengundurkan diri. Dengan angka attrition yang melebihi 10%, perusahaan mulai merasakan dampak negatif fenomena ini. Tim HR menyadari bahwa jika hal ini dibiarkan tanpa evaluasi yang tepat, bisa berdampak besar pada stabilitas kerja, performa tim, hingga meningkatnya biaya rekrutmen dan pelatihan ulang.

Untuk itu, perusahaan ingin mulai melihat data yang dimiliki secara lebih mendalam agar bisa memahami pola-pola yang terjadi dan mengambil tindakan yang lebih terarah. Diharapkan, dengan bantuan analisis data dan visualisasi yang tepat, perusahaan bisa lebih cepat tanggap dalam mengelola dan mempertahankan talenta yang ada.
Model Prediksi menggunakan Machine Learning yang dibangun juga akan membantu perusahaan ini dalam memprediksi karyawan yang berpotensi mengundurkan diri, sehingga dapat dilakukan treatment dini untuk mencegahnya. 

### Permasalahan Bisnis

Permasalahan bisnis utama dari proyek ini adalah:

   - Tingginya tingkat attrition (pengunduran diri karyawan) sekitar 16% yang berdampak pada produktivitas, biaya operasional, dan stabilitas tim.
   - Kurangnya pemahaman data di departemen HR untuk mengidentifikasi penyebab utama karyawan keluar.
   - Tidak adanya sistem pemantauan visual (dashboard) yang membantu HR mengambil keputusan berbasis data.
   - Belum adanya sistem prediksi untuk mengantisipasi karyawan yang berisiko tinggi mengundurkan diri.

### Cakupan Proyek

Untuk menjawab permasalahan tingginya attrition rate pada perusahaan edutech ini, kita akan menerapkan pendekatan analisis data terstruktur yang melibatkan beberapa tahapan utama.

Pertama, kita akan melakukan Exploratory Data Analysis (EDA) guna memahami struktur, pola, dan karakteristik data karyawan. Fokus EDA akan diarahkan pada kolom-kolom kategoris dan numerik yang berpotensi memiliki hubungan dengan pengunduran diri karyawan.
Kedua, kita akan mencoba mengidentifikasi faktor-faktor utama yang memengaruhi keputusan karyawan untuk keluar dari perusahaan. Ini akan dilakukan melalui analisis korelasi dan visualisasi interaktif yang disajikan dalam bentuk dashboard.
Ketiga, kita akan membangun sebuah business dashboard menggunakan tools seperti Metabase, agar tim HR dapat memantau data secara lebih intuitif dan cepat mengambil tindakan.
Keempat, kita akan menerapkan algoritma machine learning untuk memprediksi kemungkinan karyawan keluar berdasarkan pola historis. Algoritma yang digunakan akan disesuaikan dengan struktur data yang tersedia dan akan ditentukan pada tahap pemodelan.
Kelima, Kita akan melakukan evaluasi terhadap model machine learning yang dibangun.
Terakhir, Kita akan memberikan beberapa rekomendasi kepada perusahaan edutech berupa aksi yang dapat dilakukan untuk mengurangi Attrition pada perusahaan.

### Persiapan

**Sumber data**:
Dataset yang dimanfaatkan berasal dari Jaya Jaya Maju, sebuah perusahaan multinasional yang telah beroperasi sejak tahun 2000 dan memiliki lebih dari 1.000 karyawan di berbagai lokasi. Data ini berisi informasi terkait demografi dan pekerjaan karyawan, seperti umur, gaji, lama bekerja, serta status pekerjaan. Dataset tersebut digunakan untuk menganalisis faktor-faktor yang berkontribusi terhadap tingkat attrition (pengunduran diri karyawan) di perusahaan.

Dataset dapat diakses melalu tautan berikut : [Data Karyawan Jaya Jaya Maju](https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee)
Setup environment:

```

```

## Business Dashboard
Dashboard ini dibuat untuk menganalisis data karyawan dan memantau faktor-faktor utama yang mempengaruhi tingginya attrition rate (tingkat pergantian karyawan) di perusahaan fiktif Jaya Jaya Maju. Visualisasi ini dirancang menggunakan Metabase yang terkoneksi dengan database PostgreSQL Supabase, dan dijalankan melalui Docker.

**Tujuan Dashboard**
- Memberikan gambaran cepat tentang kondisi karyawan.
- Mengidentifikasi tren attrition berdasarkan karakteristik tertentu.
- Membantu tim HR mengambil keputusan berbasis data.


**Visualisasi yang Ditampilkan**

**Metrik Utama Perusahaan :**
- Jumlah Total Karyawan: 1.058 orang
- Distribusi Gender: 59% pria, 41% wanita
- Distribusi Karyawan per Departemen:
   - R&D: 701
   - Sales: 319
   - HR: 38
 
**Faktor Attrition yang dapat di analisa :**
- Attrition Berdasarkan Gender:
   - 60.3% pria keluar
   - 39.7% wanita keluar
- Attrition Berdasarkan Departemen dengan nilai tertinggi berada pada departemen R&D
- Attrition Berdasarkan Rentang Usia Tertinggi berada di usia 28–37 tahun (81 orang keluar)
- Attrition Berdasarkan Lama Bekerja Paling banyak terjadi di tahun ke 5–10
- Rata-rata Gaji:
     - Karyawan keluar: USD 4.872
     - Karyawan tetap: USD 6.982
- Attrition Berdasarkan Overtime dilihat bahwa Karyawan yang lembur lebih banyak keluar (98 orang) dibanding yang tidak lembur (81)

    
![Image](https://github.com/user-attachments/assets/2202dabc-dec3-4cfd-a4a2-9acb5b2a924b)

![Image](https://github.com/user-attachments/assets/52f3faf8-7349-40e3-8346-51412409240e)


**Insight Utama**
- Usia 28–37 tahun adalah kelompok dengan risiko attrition paling tinggi.
- Karyawan dengan masa kerja 5–10 tahun paling rentan keluar.
- Karyawan dengan gaji lebih rendah cenderung lebih sering keluar.
- Lembur berkorelasi signifikan terhadap keputusan keluar dari perusahaan.

## Conclusion

Proyek ini telah berhasil memberikan solusi komprehensif terhadap tantangan tingginya attrition rate di perusahaan Jaya Jaya Maju dengan pendekatan data-driven yang terintegrasi melalui dashboard interaktif. Melalui analisis eksploratif pada berbagai dimensi karyawan, diperoleh sejumlah karakteristik penting yang menunjukkan korelasi kuat terhadap kemungkinan keluar dari perusahaan.
## ✅ Konklusi Proyek – HR Attrition Analysis di Jaya Jaya Maju

Proyek ini telah berhasil memberikan solusi komprehensif terhadap tantangan tingginya **attrition rate di perusahaan Jaya Jaya Maju** dengan pendekatan data-driven yang terintegrasi melalui dashboard interaktif. Melalui analisis eksploratif pada berbagai dimensi karyawan, diperoleh sejumlah karakteristik penting yang menunjukkan korelasi kuat terhadap kemungkinan keluar dari perusahaan.

---

### 🎯 Karakteristik Karyawan yang Cenderung Mengalami Attrition

1. **Pendapatan Rendah**  
   Rata-rata karyawan yang keluar memiliki gaji bulanan (**Monthly Income**) yang lebih rendah dibandingkan karyawan yang bertahan (± USD 4.872 vs USD 6.982.). Hal ini menegaskan bahwa **kompensasi** merupakan faktor signifikan dalam keputusan keluar.

2. **Usia Produktif Awal (28–37 tahun)**  
   Karyawan dengan rentang usia **28–37 tahun** menunjukkan tingkat attrition tertinggi dalam populasi, diduga karena masa tersebut merupakan fase karir aktif di mana peluang eksternal sering dicari.

3. **Lembur Tinggi (OverTime: Yes)**  
   Karyawan yang **melakukan lembur** memiliki angka attrition yang lebih tinggi dibandingkan yang tidak lembur. Ini mengindikasikan adanya tekanan kerja dan potensi ketidakseimbangan kehidupan kerja yang memicu keputusan resign.

4. **Masa Kerja Pendek (Years at Company: 0–5 tahun)**  
   Sebagian besar attrition berasal dari karyawan yang bekerja **kurang dari 5 tahun**. Ini menunjukkan potensi masalah pada fase orientasi, adaptasi awal, atau kurangnya peluang karir di tahap awal kerja.

5. **Departemen Tertentu Lebih Rentan**  
   Departemen **Research & Development** dan **Sales** menyumbang jumlah attrition tertinggi, yang mengindikasikan bahwa beban kerja, dinamika tim, atau ekspektasi jabatan di departemen tersebut perlu dikaji lebih dalam.

6. **Distribusi Berdasarkan Gender**  
   Dari total karyawan yang keluar, **60.3% adalah pria**, namun karena distribusi gender karyawan juga didominasi pria, hal ini menunjukkan bahwa rasio attrition antara pria dan wanita relatif seimbang jika dibandingkan secara proporsional.

---
**Peran Model Prediktif (Machine Learning)**

Model prediktif berbasis machine learning yang dibangun sebagai bagian dari proyek ini menunjukkan efektivitas dalam mengidentifikasi **karyawan berisiko tinggi untuk keluar**. Dengan mempertimbangkan variabel seperti **usia, gaji, overtime, masa kerja, dan departemen**,dan lain lain model mampu memberi estimasi probabilitas attrition yang dapat diintegrasikan ke sistem monitoring HR.
---

- **Jenis model**: Logistic Regression
- **Fitur input utama**:
  - Usia
  - Gender
  - Gaji Bulanan
  - Overtime
  - Tahun di Perusahaan
  - JobSatisfaction
- **Akurasi model**: >85% pada data uji
- **Fungsi model**: Memprediksi kemungkinan seorang karyawan keluar dari perusahaan

---

**💼 Dampak Bisnis**
Dengan insight dari dashboard dan akurasi prediksi yang baik, HR kini memiliki kemampuan untuk:

- Menjalankan **intervensi proaktif** untuk karyawan berisiko tinggi
- Menyusun strategi **retensi berbasis data** seperti peningkatan kompensasi, review beban kerja, dan peningkatan engagement
- Mengurangi biaya turnover dan mempertahankan **stabilitas tim kerja**
- Meningkatkan efektivitas perencanaan SDM dan **kebijakan berbasis bukti**



### Rekomendasi Action Items (Optional)

Berikut adalah beberapa rekomendasi strategis yang dapat dilakukan oleh perusahaan Jaya Jaya Maju untuk mengurangi tingkat attrition dan meningkatkan retensi karyawan:

- **Melakukan review dan penyesuaian struktur kompensasi**, khususnya bagi karyawan dengan gaji di bawah rata-rata, untuk meningkatkan kepuasan dan loyalitas kerja.

- **Mengatur ulang kebijakan lembur dan keseimbangan kerja-hidup**, termasuk evaluasi beban kerja, rotasi tugas, dan waktu istirahat, guna mencegah burnout.

- **Merancang program onboarding dan pengembangan karir yang lebih kuat** bagi karyawan baru dan karyawan dengan masa kerja <5 tahun, agar mereka merasa memiliki masa depan jelas di perusahaan.

- **Meningkatkan keterlibatan manajerial**, dengan pelatihan bagi atasan langsung agar dapat membina hubungan kerja yang sehat dan mendukung pertumbuhan bawahannya.

- **Mengadakan exit interview secara sistematis**, untuk menggali alasan aktual karyawan keluar dan menjadikannya dasar kebijakan HR berbasis bukti.

- **Menggunakan model prediksi attrition secara berkelanjutan**, agar HR dapat mengidentifikasi karyawan berisiko tinggi secara dini dan melakukan pendekatan personal.


