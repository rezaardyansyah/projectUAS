# 📘 Judul Proyek

_(Perbandingan Metode Machine Learning dan Deep Learning untuk Klasifikasi Citra Menggunakan CNN MobileNetV2)_

## 👤 Informasi

- **Nama:** [MUHAMMAD HIKMAL AKBAR REZA ARDYANSYAH]
- **Repo:** [https://github.com/rezaardyansyah/projectUAS.git]
- **Video:** [https://drive.google.com/drive/folders/1CeMFVl_Jdiut9_5It82qJ2G17BpQqOAW?usp=drive_link]

---

# 1. 🎯 Ringkasan Proyek

Proyek ini bertujuan untuk membangun dan membandingkan performa tiga pendekatan pemodelan, yaitu model baseline, model machine learning lanjutan, dan model deep learning, pada tugas klasifikasi citra multikelas. Tahapan proyek meliputi data preparation, pemodelan, evaluasi, serta analisis hasil untuk menentukan model terbaik berdasarkan metrik evaluasi yang relevan.

---

# 2. 📄 Problem & Goals

**Problem Statements:**

- [Model klasifikasi citra perlu mampu mengenali pola visual secara otomatis dengan tingkat akurasi yang tinggi]
- [Dataset citra memiliki variasi bentuk dan tekstur sehingga membutuhkan preprocessing yang tepat]
- [Diperlukan model deep learning yang mampu mempelajari representasi fitur kompleks]
- [Perlu dilakukan perbandingan performa antara pendekatan klasik dan deep learning]

**Goals:**

- [Membangun tiga model klasifikasi: baseline, advanced ML, dan deep learning]
- [Mengukur dan membandingkan performa model menggunakan metrik evaluasi klasifikasi]
- [Menentukan model terbaik berdasarkan hasil evaluasi]
- [Menghasilkan pipeline pemodelan yang reproducible dan terdokumentasi dengan baik]

---

## 📁 Struktur Folder

```
project/
│
├── data/
│
├── notebooks/
│   └── ML_Project.ipynb
│
├── src/
│
├── models/
│   ├── model_baseline.pkl
│   ├── model_rf.pkl
│   └── model_cnn.h5
│
├── images/
│   └── r
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

# 3. 📊 Dataset

- **Sumber:** [Google Drive (dataset citra Folio)]
- **Jumlah Data:** [±1.500 gambar]
- **Tipe:** [Image (RGB)]

### Fitur Utama

| Fitur | Deskripsi                   |
| ----- | --------------------------- |
| image | Citra RGB berukuran 224×224 |
| label | Kelas target (multiclass)   |

---

# 4. 🔧 Data Preparation

- Cleaning: pengecekan data rusak dan duplikat
- Transformasi: resize gambar dan normalisasi piksel (0–1)
- Splitting: training (80%) dan test (20%)
- Augmentasi: rotation, flip, dan zoom untuk model deep learning

---

# 5. 🤖 Modeling

- **Model 1 – Baseline:** [Logistic Regression (fitur citra diekstraksi)]
- **Model 2 – Advanced ML:** [Random Forest Classifier]
- **Model 3 – Deep Learning:** [CNN dengan Transfer Learning MobileNetV2]

---

# 6. 🧪 Evaluation

**Metrik:** Accuracy / F1 / MAE / MSE (pilih sesuai tugas)

### Hasil Singkat

| Model         | Score  | Catatan                                 |
| ------------- | ------ | --------------------------------------- |
| Baseline      | [0.75] | [Performa dasar sebagai pembanding]     |
| Advanced      | [0.85] | [Lebih stabil dalam mengenali pola]     |
| Deep Learning | [0.89] | [Performa terbaik dan paling konsisten] |

---

# 7. 🏁 Kesimpulan

- Model terbaik: [Deep Learning (CNN MobileNetV2)]
- Alasan: [Memiliki akurasi dan F1-score tertinggi serta mampu menangkap fitur visual kompleks]
- Insight penting: [
  - Transfer learning sangat efektif untuk dataset citra berukuran menengah
  - Model klasik masih berguna sebagai baseline pembanding
  - Augmentasi data membantu meningkatkan generalisasi model]

---

# 8. 🔮 Future Work

- [ ] Menambah jumlah dan variasi data
- [ ] Hyperparameter tuning lebih lanjut
- [ ] Mencoba arsitektur CNN lain (EfficientNet, ResNet)
- [ ] Deployment model ke web atau mobile

---

# 9. 🔁 Reproducibility

Gunakan environment berikut:

Python: 3.10

Libraries utama: - numpy - pandas - scikit-learn - matplotlib - tensorflow
