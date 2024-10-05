# Klasifikasi Gambar menggunakan AlexNet dan ResNet pada CIFAR-10

![CIFAR-10 Dataset](https://github.com/user-attachments/assets/977b75d7-cbab-4fe8-8dd2-508b19dd4ba5)

## Daftar Isi
- [Deskripsi Proyek](#deskripsi-proyek)
- [Persiapan](#persiapan)
- [Arsitektur Model](#arsitektur-model)
  - [AlexNet](#alexnet)
  - [ResNet](#resnet)
- [Dataset](#dataset)
- [Instalasi](#instalasi)
- [Penggunaan](#penggunaan)
- [Hasil](#hasil)
- [Lisensi](#lisensi)
- [Penghargaan](#penghargaan)

## Deskripsi Proyek
Proyek ini mengimplementasikan dua model deep learning, **AlexNet** dan **ResNet**, untuk klasifikasi gambar pada dataset CIFAR-10. Dataset CIFAR-10 terdiri dari 60.000 gambar warna berukuran 32x32 piksel dalam 10 kelas, dengan masing-masing kelas memiliki 6.000 gambar. Tujuan proyek ini adalah untuk mengeksplorasi performa dari kedua model ini pada dataset gambar yang lebih kecil.

## Persiapan
Sebelum memulai proyek ini, pastikan Anda telah menginstal Python beserta pustaka yang diperlukan.

### Kebutuhan
- Python 3.x
- Jupyter Notebook
- PyTorch
- torchvision
- torchsummary
- numpy
- matplotlib

## Arsitektur Model

### AlexNet
AlexNet adalah jaringan saraf konvolusi dalam yang telah mencapai keberhasilan signifikan dalam berbagai tugas visi komputer. Model ini terdiri dari beberapa lapisan konvolusi, lapisan pooling, dan lapisan fully connected.

**Fitur Utama:**
- **Ukuran Input**: Disesuaikan untuk menangani gambar berukuran 32x32.
- **Lapisan**: Beberapa lapisan konvolusi dan fully connected.
- **Fungsi Aktivasi**: ReLU digunakan sebagai fungsi aktivasi.

### ResNet
ResNet (Residual Network) memperkenalkan pembelajaran residual untuk memungkinkan pelatihan jaringan yang sangat dalam. ResNet-18, varian dari ResNet, digunakan dalam proyek ini.

**Fitur Utama:**
- **Ukuran Input**: Dirancang untuk gambar berukuran 32x32.
- **Blok Residual**: Menggunakan koneksi shortcut untuk mencegah gradien menghilang.
- **Performa**: Dikenal karena performa superior pada berbagai dataset.

## Dataset
Dataset **CIFAR-10** terdiri dari 10 kelas:
- Pesawat
- Mobil
- Burung
- Kucing
- Rusa
- Anjing
- Katak
- Kuda
- Kapal
- Truk

### Mengunduh Dataset
Dataset dapat dengan mudah diunduh menggunakan torchvision. Dataset pelatihan dan pengujian diunduh secara otomatis saat pelatihan model.

## Instalasi
Clone repositori dan instal paket yang diperlukan:

```bash
git clone https://github.com/yourusername/nama-repo-anda.git
cd nama-repo-anda
pip install -r requirements.txt
