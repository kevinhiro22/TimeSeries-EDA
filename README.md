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

tugas ini dikerjakan dalam format *notebook* dengan beberapa *kriteria wajib* di bawah ini:

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
