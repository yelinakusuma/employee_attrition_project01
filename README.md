# HR Analytics: Prediksi Resign Karyawan untuk Mengurangi Turnover

## Repository Outline
Berikut merupakan isi dari repository github:
```
1. README.md - Penjelasan gambaran umum project
2. notebook.ipynb - Notebook ini berisi proses pengolahan data dengan python (dari data loading hingga saving model)
3. model_inf.ipynb - Notebook ini berisi proses inference model untuk memprediksi data baru
```

## Problem Background
Perusahaan DEF merupakan multinational company yang memiliki banyak kantor cabang yang tersebar, salah satunya di Indonesia. Di salah satu wilayah, perusahaan ini mengalami masalah peningkatan jumlah karyawan yang resign dalam 3 bulan terakhir. Untuk mengatasi hal ini, perusahaan meminta bantuan tim Data Scientist dalam membangun model prediksi yang dapat mengidentifikasi karyawan yang berpeluang untuk resign berdasarkan data historis. Dengan model ini, perusahaan dapat mengambil langkah strategis untuk memertahankan karyawan yang berisiko resign. Oleh karena itu, proyek ini difokuskan pada pemilihan model klasifikasi terbaik dengan memertimbangkan metrik precision guna meminimalkan jumlah False Positive (FP), sehingga tim HR dapat menyusun strategi retensi yang lebih efektif.

## Project Output
Proyek ini menghasilkan model machine learning yang telah dideploy dan dapat digunakan untuk melakukan prediksi secara otomatis. Model ini dapat membantu user dalam memprediksi karyawan yang berisiko resign.

## Data
Dataset yang digunakan untuk pemodelan didapatkan dari Kaggle. Dataset ini berisi informasi detail tentang profil karyawan, seperti jarak rumah ke kantor, job role, dan kondisi pribadi yang dapat memengaruhi keputusan resign. Dataset ini memiliki 59598 baris dan 24 kolom, serta tidak terdapat missing value pada data sehingga dapat langsung diproses untuk Exploratory Data Analysis (EDA) dan Data Preprocessing untuk Modeling. Selain itu, informasi karyawan dalam dataset ini mencakup dari department Technology, Healthcare, Finance, Education, dan Media.

## Method
Proyek ini menggunakan model AdaBoost Classifier, yang dipilih sebagai best model yang berdasarkan hasil cross validation dengan membandingkan beberapa model machine learning lainnya.

## Stacks
- Bahasa pemrograman yang digunakan pada proyek ini yaitu dengan python, untuk pengolahan data dan pengembangan model
- Tools dan platform yang digunakan yaitu, hugging face untuk melakukan deployment aplikasi berbasis streamlit, dan VS Code untuk modeling
- Library python yang digunakan antara lain `pandas`, `numpy`, `matplotlib`, `seaborn`, dan `scipy` untuk manipulasi dan analisis data, serta `sklearn`, `phik`, `feature_engine`, dan `pickle` untuk pemodelan

## Reference
[URL Dataset](https://www.kaggle.com/datasets/stealthtechnologies/employee-attrition-dataset/data?select=train.csv)
[URL deployment](https://huggingface.co/spaces/yelinakusuma/Prediksi_Attrition_Karyawan)