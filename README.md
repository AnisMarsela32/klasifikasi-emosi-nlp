# Klasifikasi Emosi dari Kalimat dengan LSTM

Proyek ini bertujuan membangun model deep learning untuk mengenali emosi dalam kalimat bahasa Inggris menggunakan arsitektur LSTM. Model dapat mengklasifikasikan enam emosi utama: **joy**, **sadness**, **anger**, **fear**, **love**, dan **surprise**.

## Fitur Utama

- Pembersihan teks: lowercase, hapus simbol/angka, stopword removal, lemmatization
- Padding dan tokenisasi kalimat
- Model LSTM dengan layer embedding, Bidirectional LSTM, dan dropout
- Penanganan ketidakseimbangan data dengan class weight
- Evaluasi dengan classification report dan confusion matrix
- Aplikasi interaktif dengan Streamlit

## Hasil Model

Model mencapai akurasi validasi ~90%. Emosi dengan data terbatas seperti *surprise* menunjukkan performa yang lebih rendah dibanding emosi dominan seperti *joy* atau *sadness*.

## Demo Online

Model bisa dicoba langsung melalui Hugging Face Spaces:  
👉 [Demo Aplikasi di Hugging Face](https://huggingface.co/spaces/anismarsela32/klasifikasi-emosi-NLP)

## 📁 Struktur Folder

```

├── src/
│   ├── data/           # Dataset train.txt
│   ├── image/          # Ilustrasi emosi
│   └── model/          # Model terlatih (.h5 / .pkl)
├── eda.py              # Visualisasi data (EDA)
├── main.py             # Aplikasi Streamlit
└── README.md

````

## 🛠️ Cara Menjalankan Lokal

1. Clone repository ini
2. Install dependensi:
   ```bash
   pip install -r requirements.txt
````

3. Jalankan aplikasi:

   ```bash
   streamlit run streamlit_app.py
   ```

> Pastikan resource NLTK sudah terunduh: `punkt`, `stopwords`, `wordnet`, `omw-1.4`.

## Teknologi

* Python
* TensorFlow / Keras
* NLTK
* scikit-learn
* Streamlit

```


