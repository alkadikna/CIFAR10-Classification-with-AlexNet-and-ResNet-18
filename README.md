# Klasifikasi Gambar menggunakan AlexNet dan ResNet pada CIFAR-10

<p align="center">
  <img src="https://github.com/user-attachments/assets/977b75d7-cbab-4fe8-8dd2-508b19dd4ba5" alt="CIFAR-10 Dataset" width="500"/>
</p>

## Daftar Isi
- [Deskripsi](#deskripsi-eksperimen)
- [Arsitektur Model](#arsitektur-model)
  - [AlexNet](#alexnet)
  - [ResNet](#resnet)
- [Dataset](#dataset)
  - [Regulasi](#teknik-regulasi)
- [Instalasi](#instalasi)
- [Hasil](#hasil)
  - [AlexNet](#hasil-alexnet)
  - [ResNet](#hasil-resnet)

## Deskripsi Eksperimen
Eksperimen ini mengimplementasikan dua model deep learning, yaitu **AlexNet** dan **ResNet-18**, untuk klasifikasi gambar pada dataset CIFAR-10. Dataset CIFAR-10 terdiri dari 60.000 gambar warna berukuran 32x32 piksel dalam 10 kelas, dengan masing-masing kelas memiliki 6.000 gambar. Tujuan eksperimen ini adalah untuk melihat dan membandingkan performa dari kedua model pada dataset CIFAR-10.

### Requirement
- Python 3.10
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

### Teknik Regulasi
- Augementasi Data
- Normalisasi
- Dropout

### Download Dataset
Dataset dapat dengan mudah diunduh menggunakan torchvision. Dataset pelatihan dan pengujian diunduh secara otomatis saat pelatihan model.

## Instalasi
Clone repositori dan instal paket yang diperlukan:

```bash
git clone https://github.com/alkadikna/CIFAR10-Classification-with-AlexNet-and-ResNet-18
cd CIFAR10-Classification-with-AlexNet-and-ResNet-18
```

## Hasil
Setelah notebook dijalankan, hasil akan berupa akurasi dan loss dari training dan testing. Untuk hyperparameter, di kedua model adalah **sama**.

<p align="center">
  <img src="https://github.com/user-attachments/assets/25674d2c-de40-48dd-a507-476ea77a0303" alt="" width="500"/>
</p>

### Hasil AlexNet
<p align="center">
  <img src="https://github.com/user-attachments/assets/c8b03ef5-a883-4aa6-9703-8ecd50065551" alt=""/>
  <img src="https://github.com/user-attachments/assets/4fa603d8-9419-47fd-a80c-02b0d56bb155" alt="" width="500"/>
</p>

### Hasil ResNet
<p align="center">
  <img src="https://github.com/user-attachments/assets/98e3af9e-ab47-4646-ba49-7bd4d613e779" alt=""/>
  <img src="https://github.com/user-attachments/assets/c9209b0c-badc-429a-a218-b4efb0480a84" alt="" width="500"/>
</p>
