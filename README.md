# Global Health Trends EDA

Analisis eksploratif data (**Exploratory Data Analysis/EDA**) terhadap dataset kesehatan global untuk mengidentifikasi tren dari waktu ke waktu serta hubungannya dengan faktor demografi dan sosial-ekonomi, seperti negara, jenis kelamin, kelompok usia, generasi, populasi, GDP per kapita, dan **Human Development Index (HDI)**.

## Deskripsi

Proyek ini bertujuan mengeksplorasi dan memvisualisasikan dataset statistik kesehatan global guna memperoleh insight mengenai pola, tren, dan hubungan antarvariabel. Analisis dilakukan menggunakan **Python**, **Pandas**, **Matplotlib**, dan **Seaborn** melalui serangkaian visualisasi serta analisis statistik deskriptif.

Fokus analisis meliputi:

* Tren jumlah kasus dari tahun ke tahun.
* Perbandingan jumlah kasus antarnegara.
* Distribusi berdasarkan jenis kelamin, kelompok usia, dan generasi.
* Hubungan antara jumlah kasus dengan indikator sosial-ekonomi, seperti populasi, GDP per kapita, dan Human Development Index (HDI).
* Analisis korelasi antarvariabel numerik menggunakan heatmap.

> **Catatan Dataset**
>
> Dataset yang digunakan merupakan **Suicide Rates Overview 1985–2016**, yang menggabungkan data dari **WHO**, **World Bank**, dan **UNDP**. Pada repository ini, dataset digunakan sebagai contoh analisis statistik kesehatan global untuk keperluan pembelajaran dan portofolio data analytics.

---

## Skill yang Digunakan

* Data cleaning menggunakan **Pandas**
* Data aggregation dan grouping
* Exploratory Data Analysis (EDA)
* Visualisasi data menggunakan **Matplotlib** dan **Seaborn**
* Analisis tren (*time series*)
* Analisis kategorikal
* Analisis korelasi antarvariabel
* Data storytelling melalui visualisasi

---

## Struktur Notebook

| No. | Tahapan                                 | Deskripsi                                                                               |
| :-: | --------------------------------------- | --------------------------------------------------------------------------------------- |
|  1  | **Import Libraries**                    | Mengimpor library `pandas`, `numpy`, `matplotlib`, dan `seaborn`.                       |
|  2  | **Load Dataset**                        | Membaca dataset serta menampilkan struktur dan informasi data.                          |
|  3  | **Analisis Tren Tahunan**               | Membuat line chart jumlah kasus setiap tahun.                                           |
|  4  | **Analisis Kasus per 100.000 Penduduk** | Membuat line chart tingkat kasus per 100.000 penduduk setiap tahun.                     |
|  5  | **Top 10 Negara**                       | Menampilkan 10 negara dengan jumlah kasus tertinggi menggunakan bar chart.              |
|  6  | **Distribusi Jenis Kelamin**            | Menampilkan proporsi kasus berdasarkan jenis kelamin menggunakan pie chart.             |
|  7  | **Distribusi Kelompok Usia**            | Menampilkan jumlah kasus berdasarkan kelompok usia dalam bentuk bar chart.              |
|  8  | **Distribusi Generasi**                 | Menampilkan jumlah kasus berdasarkan kategori generasi.                                 |
|  9  | **Analisis Populasi**                   | Menganalisis hubungan antara jumlah penduduk dan jumlah kasus menggunakan scatter plot. |
|  10 | **Analisis GDP per Kapita**             | Menganalisis hubungan antara GDP per kapita dan jumlah kasus.                           |
|  11 | **Analisis HDI**                        | Menganalisis hubungan antara Human Development Index (HDI) dan jumlah kasus.            |
|  12 | **Correlation Heatmap**                 | Menampilkan heatmap korelasi antarvariabel numerik dalam dataset.                       |

---

## Requirements

```text
pandas
numpy
matplotlib
seaborn
```

### Instalasi

```bash
pip install pandas numpy matplotlib seaborn
```

---

## Data Input

Notebook membutuhkan sebuah file **CSV** yang minimal memiliki kolom berikut.

| Kolom                | Deskripsi                                         |
| -------------------- | ------------------------------------------------- |
| `country`            | Nama negara                                       |
| `year`               | Tahun pencatatan data                             |
| `sex`                | Jenis kelamin                                     |
| `age`                | Kelompok usia                                     |
| `suicides_no`        | Jumlah kasus                                      |
| `population`         | Jumlah penduduk                                   |
| `suicides/100k pop`  | Jumlah kasus per 100.000 penduduk                 |
| `HDI for year`       | Nilai Human Development Index pada tahun tersebut |
| `gdp_per_capita ($)` | GDP per kapita (USD)                              |
| `generation`         | Kategori generasi                                 |

---

## Cara Menjalankan

1. Siapkan file dataset dalam format **CSV**.
2. Jika menggunakan **Google Colab**, unggah dataset ke direktori `/content/`. Jika menggunakan **Jupyter Notebook**, sesuaikan lokasi file dengan direktori kerja.
3. Instal seluruh dependency yang tercantum pada bagian **Requirements**.
4. Jalankan seluruh sel notebook secara berurutan.
5. Notebook akan menghasilkan berbagai visualisasi dan analisis statistik yang menggambarkan tren serta hubungan antarvariabel pada dataset.

---

## Output

Notebook menghasilkan beberapa visualisasi, antara lain:

* Grafik tren jumlah kasus setiap tahun.
* Grafik tren jumlah kasus per 100.000 penduduk.
* Bar chart 10 negara dengan jumlah kasus tertinggi.
* Pie chart distribusi kasus berdasarkan jenis kelamin.
* Bar chart distribusi kelompok usia.
* Bar chart distribusi berdasarkan generasi.
* Scatter plot hubungan antara jumlah kasus dengan:

  * Populasi
  * GDP per kapita
  * Human Development Index (HDI)
* Heatmap korelasi antarvariabel numerik.

---

## Insight Analisis

Melalui visualisasi yang dihasilkan, pengguna dapat:

* Mengidentifikasi perubahan tren jumlah kasus dari waktu ke waktu.
* Membandingkan distribusi kasus antarnegara.
* Mengetahui kelompok usia, jenis kelamin, dan generasi yang memiliki jumlah kasus lebih tinggi.
* Menganalisis hubungan antara indikator sosial-ekonomi dengan jumlah kasus.
* Memahami kekuatan hubungan antarvariabel numerik melalui correlation heatmap.

---
