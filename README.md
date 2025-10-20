🪨✋✌️ ImageClassification_RockPaperScissors
📖 Deskripsi Umum

Proyek ImageClassification_RockPaperScissors bertujuan untuk membangun model klasifikasi citra yang dapat mengenali tiga jenis gesture tangan — Batu (Rock), Kertas (Paper), dan Gunting (Scissors).
Model ini dikembangkan menggunakan pendekatan Deep Learning berbasis Convolutional Neural Network (CNN) untuk mempelajari pola visual dari gambar dan mengklasifikasikannya ke dalam tiga kategori tersebut.

🎯 Tujuan Proyek

Mengimplementasikan model CNN untuk klasifikasi gambar sederhana.

Mempelajari performa model terhadap data training dan validation.

Menghasilkan model yang dapat mengenali gesture tangan dengan akurasi tinggi.

🧩 Dataset

Dataset yang digunakan terdiri dari tiga kelas utama:

Rock (Batu)

Paper (Kertas)

Scissors (Gunting)

Dataset dibagi menjadi dua bagian:

Training Set → digunakan untuk melatih model

Validation Set → digunakan untuk menguji performa model setelah pelatihan

📊 Distribusi Data

Gambar berikut menunjukkan total data pada masing-masing set:

<img width="955" height="204" alt="image" src="https://github.com/user-attachments/assets/e95ed01a-774f-46b1-a1c5-9a6d0a790760" />
🖼️ Visualisasi Data

Sebelum pelatihan, dilakukan visualisasi beberapa sampel dari setiap kelas untuk memastikan data telah terdistribusi dengan benar.

<img width="739" height="448" alt="image" src="https://github.com/user-attachments/assets/40f9e29d-8574-43ba-a904-5a0dba900f59" /> <img width="718" height="445" alt="image" src="https://github.com/user-attachments/assets/dec1fa07-498d-4762-bc1a-7056b612076c" />
🧠 Arsitektur Model

Model dibangun menggunakan Convolutional Neural Network (CNN) dengan beberapa lapisan utama:

Conv2D untuk ekstraksi fitur dari gambar.

MaxPooling2D untuk mereduksi dimensi fitur.

Flatten untuk mengubah hasil ekstraksi menjadi vektor 1D.

Dense (Fully Connected Layer) sebagai lapisan klasifikasi akhir.

Model dioptimalkan menggunakan optimizer Adam dan loss function categorical crossentropy, dengan akurasi (accuracy) sebagai metrik evaluasi utama.

⚙️ Proses Pelatihan (Training Process)

Dataset dibaca dan diolah menjadi tensor menggunakan ImageDataGenerator.

Data dilakukan augmentation untuk menambah variasi (rotasi, flip, zoom, dsb).

Model dilatih menggunakan model.fit() selama beberapa epoch.

Hasil pelatihan divisualisasikan dalam bentuk grafik akurasi dan loss.

🧾 Hasil dan Evaluasi

Setelah model selesai dilatih, dilakukan pengujian menggunakan data baru (testing data).
Berikut hasil prediksi model terhadap beberapa sampel gambar:

<img width="686" height="510" alt="image" src="https://github.com/user-attachments/assets/725dbe74-f484-43d5-96b3-42565cdf5aa6" /> <img width="711" height="523" alt="image" src="https://github.com/user-attachments/assets/bb9739b9-0dcc-4a1a-875e-5df025f7f4a8" />

Model mampu mengenali gesture tangan dengan tingkat akurasi yang baik, terutama pada data yang memiliki kualitas pencahayaan dan posisi tangan yang jelas.

🧪 Pengujian Model (Testing)

Model diuji dengan beberapa gambar acak untuk melihat apakah klasifikasi berjalan dengan benar.
Setiap hasil prediksi disertai label aktual dan label hasil prediksi model untuk perbandingan.

📈 Kesimpulan

Model CNN berhasil mengenali tiga kelas gesture tangan dengan akurasi tinggi.

Kinerja model dapat ditingkatkan dengan menambah jumlah data atau menggunakan transfer learning (misalnya dengan MobileNetV2 atau ResNet).

Model ini dapat dijadikan dasar untuk aplikasi interaktif seperti game atau sistem deteksi gesture real-time menggunakan kamera.

🔧 Teknologi yang Digunakan

Python

TensorFlow / Keras

NumPy & Matplotlib

Google Colab / Jupyter Notebook

🚀 Cara Menjalankan Proyek

Clone repository:

git clone https://github.com/<username>/ImageClassification_RockPaperScissors.git
cd ImageClassification_RockPaperScissors


Install dependensi:

pip install -r requirements.txt


Jalankan notebook pelatihan model:

ImageClassification_RockPaperScissors.ipynb


Lihat hasil prediksi dan evaluasi model.

🏁 Saran Pengembangan

Menambahkan real-time classification menggunakan webcam.

Meningkatkan dataset agar model lebih robust terhadap kondisi pencahayaan.

Menggunakan transfer learning untuk hasil yang lebih cepat dan akurat.
