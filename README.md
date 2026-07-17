[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/-Per8O2k)
# Live Code 5

---

## Assignment Objectives

*Live Code 5* ini dibuat guna mengevaluasi konsep Time Series Analysis pada pembelajaran Phase 1 sebagai berikut:

- Mampu memahami konsep Time Series Analysis untuk kebutuhan forecasting.

- Mampu melakukan time series decomposition untuk mengetahui pola seasonal data.

- Mampu menerapkan pengujian stasioneritas dan penerapan teknik differencing pada data.
.
- Mampu melakukan forecasting data dengan model ARIMA.

- Mampu menentukan model yang terbaik berdasarkan metrik evaluasi.

---

## Dataset Description

Dataset : `multiTimeline.csv`

| Column | Description |
| --- | --- |
| `Week` | Tanggal pertama pada setiap minggu (berformat `YYYY-MM-DD`) |
| `Pulau Pari: (Indonesia)` |  Informasi persentase popularitas terhadap nilai maksimum dari kata kunci yang dicari. <br><br> - `0 : tidak ada data`, <br> - `50 : popularitas hanya setengah`, <br> - `100 : sangat populer` |

> [!TIP]
> Bukalah terlebih dahulu datasetnya dan perhatikan dengan seksama isi dataset sebelum Anda melakukan Data Loading dengan library Pandas.

---

## Problems

Anda bekerja di sebuah perusahaan travel agent dan diminta untuk menganalisa permintaan paket wisata ke Pulau Pari. Anda memiliki data yang berasal dari Google Trends yang mengandung informasi seberapa populer kata kunci `Pulau Pari` di pencarian Google. Anda diminta untuk memprediksi seberapa populer wisata ke Pulau Pari selama setahun ke depan dari tanggal terakhir dari dataset yang diberikan.

---

## Assignment Instructions

*Live Code 4* dikerjakan dalam format *notebook* dengan beberapa *kriteria wajib* di bawah ini:

1. Time series analysis dan forecasting dilakukan dengan menggunakan library *Statsmodels*.

2. Pengolahan data dilakukan dengan library *Pandas*.

3. Data visualisasi dapat menggunakan library *Matplotlib* atau *Pandas*.

4. Isi *notebook* harus mengikuti *outline* di bawah ini:
   1. Perkenalan
      > Bab pengenalan harus diisi dengan identitas, gambaran besar dataset yang digunakan, dan *objective* yang ingin dicapai.
   
   2. Import Libraries
      > *Cell* pertama pada *notebook* **harus berisi dan hanya berisi** semua *library* yang digunakan dalam *project*.
   
   3. Data Loading
      > Bagian ini berisi proses penyiapan data sebelum dilakukan eksplorasi data lebih lanjut. Proses Data Loading dapat berupa memberi nama baru untuk setiap kolom, mengecek tipe data setiap kolom, dll.
 
   4. Exploratory Data Analysis (EDA)
      > Bagian ini berisi visualisasi data time series, time series decomposition, ekstraksi periode seasonal, uji stasioner.
 
   5. Model Definition and Training
      > Bagian ini berisi proses definisi model hingga pelatihan model menggunakan algoritma ARIMA.

   6. Model Evaluation
      > Bagian ini berisi evaluasi model menggunakan metrics MAE yang menunjukkan performansi model untuk forecasting data.

   7. Model Improvement
      > Bagian ini berisikan proses improvasi model seperti fine tuning.

   7. Model Inference
      > Model yang sudah dilatih dan terpilih sebagai model terbaik akan dicoba untuk memprediksi data dimasa depan.

5. Ketentuan Exploratory Data Analysis:
   1. Wajib menampilkan visualisasi data untuk mendapatkan gambaran bentuk time seriesnya. Bagaimana karakteristik dari data time series tersebut ?

   2. Diperlukan untuk melakukan Time Series Decomposition dengan model `additive` atau `multiplicative` sesuai dengan pilihan dan justifikasi yang tepat. Perlu diperhatikan bahwa interval waktu 1 minggu bukan 1 hari.

   3. Lakukan pengujian apakah data stasioner atau tidak, dan tentukan pula nilai parameter `d`.


## Assignment Submission

- Simpan assignment pada sesi ini dengan nama `P1LC5_<nama-student>.ipynb`, misal `P1LC5_raka_ardhi.ipynb`.

- Push Assigment yang telah Anda buat ke akun Github Classroom Anda masing-masing.

- Contoh bentuk isi repository.
    ```
    ├── P1LC5_raka_ardhi.ipynb
    ├── multiTimeline.csv
    └── README.md
    ```

---

## Assignment Rubrics

### Code Review

| Criteria | Meet Expectations | Points|
| --- | --- | --- |
| Time Series Decomposition | Mampu melakukan time series decomposition dan menentukan periode seasonal data | 5 pts |
| Stationarity | Mampu menerapkan uji stasioneritas pada data dan melakukan tindaklanjut dari hasil pengujian, menentukan parameter `d` | 5 pts |
| ARIMA | Mampu melakukan forecasting dengan model ARIMA dengan parameter yang tepat | 5 pts |
| Fine Tuning | Mampu menentukan kombinasi `p` dan `q` untuk mengimprovisasi model | 5 pts |
| Model Inference | Mampu memprediksi data hingga setahun ke depan | 5 pts |
| Runs Perfectly | Kode berjalan tanpa ada error. Seluruh kode berfungsi dan dibuat dengan benar | 5 pts |


### Readability

| Criteria | Meet Expectations | Points|
| --- | --- | --- |
| Tertata Dengan Baik | Semua baris kode terdokumentasi dengan baik dengan menggunakan Markdown untuk penjelasan kode. | 5 pts |

```
Kriteria tertata dengan baik diantaranya adalah : 

1. Terdapat section Perkenalan yang jelas
2. Tidak menyalin markdown dari tugas lain.
3. Import library rapih (terdapat dalam 1 cell dan tidak ada unused libs).
4. Pemakaian fungsi markdown yang optimal (Heading, text formating, dll). 
5. Terdapat komentar pada setiap baris kode.
6. Adanya pemisah yang jelas antar section, dll.
7. Tidak adanya typo.
```

### Analysis

| Criteria | Meet Expectations | Points|
| --- | --- | --- |
| Overall Analysis | Menarik informasi/kesimpulan dari keseluruhan kegiatan yang dilakukan | 5 pts |

```
Contoh kriteria analisa yang baik diantaranya adalah: 

1. Terdapat penjelasan hasil evaluasi model dengan menggunakan metrics MAE interpretasi/kaitannya terhadap kasus yang diselesaikan.
2. Dapat menjelaskan kelemahan/kekurangan dan kelebihan dari model yang dibuat.
3. Dapat menyebutkan insight yang dilakukan pada proses EDA, dll.
```

---

```
Total Points : 40
```

---
