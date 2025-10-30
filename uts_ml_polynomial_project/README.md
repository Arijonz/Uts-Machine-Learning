# UTS Machine Learning — Polynomial Regression (Google Colab)

Project ini menyiapkan notebook lengkap untuk memenuhi *semua* butir penilaian pada soal UTS:
- EDA, preprocessing, scaling & penyimpanan scaler
- Polynomial Features derajat 1–5
- Linear, Ridge (α=0.1,1,10), Lasso (α=0.1,1,10)
- Evaluasi: R², MSE, RMSE, MAE, MAPE (train & test)
- Analisis over/underfitting + learning curves
- Visualisasi utama (histogram, scatter, heatmap korelasi, residual, predicted vs actual, dsb.)
- Analisis regularisasi (Ridge vs Lasso; α=[0.001..100]) dan feature importance
- Seleksi model terbaik via K-Fold CV (k=5), simpan model terbaik (joblib)
- Fungsi prediksi & uji pada 5 data baru (+ interval prediksi sederhana via bootstrap/resampling)
- Bonus: implementasi polynomial regression dari nol (gradient descent)

## Struktur
```
uts_ml_polynomial_project/
├─ data/
│  └─ properties.csv
├─ uts_polynomial_regression.ipynb
├─ requirements.txt
└─ report.md
```

## Cara Menjalankan (di Google Colab)
1. Unggah folder zip ini ke Google Drive Anda, lalu ekstrak.
2. Buka `uts_polynomial_regression.ipynb` di Google Colab.
3. Jalankan semua sel dari atas ke bawah.
4. Model terbaik dan scaler akan tersimpan di folder kerja (`artifacts/`).

> Dataset default adalah *synthetic* yang telah dibuat sesuai spesifikasi soal. Anda bebas mengganti dengan dataset real (mis. Kaggle) selama kolomnya serupa atau Anda sesuaikan pipeline-nya.

## Catatan
- Notebook sudah modular (menggunakan fungsi-fungsi) dan diberi komentar per bagian.
- `report.md` adalah template laporan yang bisa Anda lengkapi dan ekspor ke PDF.
- `requirements.txt` berisi library yang diperlukan bila Anda ingin menjalankan secara lokal.

Semoga membantu, selamat mengerjakan UTS!
