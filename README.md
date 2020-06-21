# Prediksi Harga Jual Rumah dengan Scikit-Learn

Pada notebook ini, library Python yang dibutuhkan adalah numpy, pandas, matplotlib, seaborn, scipy, dan scikit-learn. 

## Sumber Data
Dataset didapat dari [Kaggle](https://www.kaggle.com/c/home-data-for-ml-course).

## Deskripsi File Jupyter Notebook
Singkatnya, langkah pengerjaan dibagi menjadi empat bagian:
1. Exploratory Data Analysis—mendapatkan insight dari data tersebut. Pada tahap ini, visualisasi dilakukan dengan seaborn dan matplotlib. Nilai yang hilang/tidak ada pada setiap kolom dicek dengan pandas.
2. Data wrangling—yaitu mengubah data agar bisa dimengerti oleh algoritma machine learning (menggunakan sklearn), serta melakukan data cleaning. Pandas dan seaborn digunakan pada tahap ini.
3. Prediksi—menggunakan sklearn untuk mempelajari pola pada training data. Pertama, beberapa algoritma machine learning tanpa tuning akan digunakan. Kemudian, didapatkan satu algoritma dengan error paling rendah. Pada kasus ini, Gradient Boosting Regressor mendapat nilai terbaik. Algoritma GB ini akan di-tuning dengan GridSearchCV dan di-fix-kan.
4. Mengaplikasikan pada data test. Sebelumnya, data test akan diubah terlebih dahulu, kurang lebih sama dengan step ke-2. Setelah itu, model Gradient Boosting akan memprediksi data test ini.
