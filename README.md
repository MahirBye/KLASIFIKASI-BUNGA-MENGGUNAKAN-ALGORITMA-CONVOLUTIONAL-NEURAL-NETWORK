# Klasifikasi Bunga Menggunakan Convolutional Neural Network (CNN)

Proyek ini bertujuan untuk mengklasifikasikan tiga jenis bunga (Matahari, Aglonema, dan Bougenville) menggunakan algoritma **Convolutional Neural Network (CNN)**. Model yang digunakan melibatkan CNN dasar dan transfer learning dengan **VGG16** untuk meningkatkan akurasi klasifikasi.

## **Fitur Utama**
- **Pra-pemrosesan Data**: 
  - Mengubah ukuran gambar menjadi 150x150 piksel.
  - Normalisasi nilai piksel ke rentang [0, 1].
  - Augmentasi data (rotasi, flipping, zooming, perubahan brightness, dll.) untuk meningkatkan keragaman data.
- **Model Klasifikasi**: 
  - CNN dasar dengan lapisan konvolusi, pooling, dan fully connected.
  - Transfer learning menggunakan pretrained model VGG16 dengan fine-tuning untuk tugas klasifikasi.
- **Evaluasi Model**: 
  - Metrik utama: Akurasi, precision, recall, F1-score, dan confusion matrix.
  - Grafik akurasi dan loss menunjukkan model tidak mengalami overfitting atau underfitting.

## **Struktur Proyek**
- `data/`: Dataset berisi 300 gambar, terdiri dari tiga kelas dengan distribusi 100 gambar per kelas.
- `notebooks/`: Notebook Jupyter untuk eksplorasi data, pemrosesan, dan pelatihan model.
- `results/`: Hasil evaluasi model, seperti confusion matrix dan grafik akurasi/loss.
- `scripts/`: Skrip Python untuk pelatihan model dan augmentasi data.

## **Teknologi yang Digunakan**
- **Python Libraries**:
  - `TensorFlow` & `Keras`: Untuk membangun dan melatih model CNN.
  - `pandas` & `numpy`: Untuk manipulasi dan analisis data.
  - `matplotlib` & `seaborn`: Untuk visualisasi hasil.
- **Google Colab**: Digunakan untuk mempercepat pelatihan dengan GPU.

## **Cara Menjalankan Proyek**
1. Clone repository ini:
   ```bash
   git clone https://github.com/username/klasifikasi-bunga-cnn.git
   ```
2. Install dependensi:
   ```bash
   pip install -r requirements.txt
   ```
3. Jalankan notebook atau skrip untuk melatih dan mengevaluasi model:
   ```bash
   python train_model.py
   ```

## **Hasil**
- **Akurasi Training**: 93.33%
- **Akurasi Validasi**: 91.67%
- Grafik akurasi dan loss menunjukkan bahwa model bekerja optimal dengan kemampuan generalisasi yang baik.

## **Dataset**
Data set yang digunakan: https://www.kaggle.com/datasets/muhammateditrisusilo/klasifikasi-bunga
