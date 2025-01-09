# UAS_ML_221011403287

# Sistem Fuzzy Logic untuk Kontrol Kecepatan Kipas AC
## Universitas Pamulang - 2025

## Banyu Santoso
## 221011403287
## 05TPLE016

### 1. Pendahuluan
- **Tujuan Sistem**: Mengontrol kecepatan kipas AC secara otomatis
- **Input Variables**:
  - Suhu Ruangan (16°C - 30°C)
  - Tingkat Kenyamanan (0-10)
- **Output**: Kecepatan Kipas (0-100%)

### 2. Variabel Fuzzy

#### A. Suhu Ruangan (Temperature)
- **Range**: 16°C - 30°C
- **Himpunan Fuzzy**:
  - Dingin (Cold): [16, 16, 22]
  - Nyaman (Comfortable): [20, 24, 28]
  - Panas (Hot): [26, 30, 30]

#### B. Tingkat Kenyamanan (Comfort)
- **Range**: 0 - 10
- **Himpunan Fuzzy**:
  - Rendah (Low): [0, 0, 5]
  - Sedang (Medium): [3, 5, 7]
  - Tinggi (High): [6, 10, 10]

#### C. Kecepatan Kipas (Fan Speed)
- **Range**: 0% - 100%
- **Himpunan Fuzzy**:
  - Rendah (Low): [0, 0, 50]
  - Sedang (Medium): [30, 50, 70]
  - Tinggi (High): [60, 100, 100]

### 3. Aturan Fuzzy (Fuzzy Rules)

1. IF Temperature is Cold AND Comfort is High THEN Fan Speed is Low
2. IF Temperature is Cold AND Comfort is Medium THEN Fan Speed is Low
3. IF Temperature is Cold AND Comfort is Low THEN Fan Speed is Medium
4. IF Temperature is Comfortable AND Comfort is High THEN Fan Speed is Low
5. IF Temperature is Comfortable AND Comfort is Medium THEN Fan Speed is Medium
6. IF Temperature is Comfortable AND Comfort is Low THEN Fan Speed is High
7. IF Temperature is Hot AND Comfort is High THEN Fan Speed is Medium
8. IF Temperature is Hot AND Comfort is Medium THEN Fan Speed is High
9. IF Temperature is Hot AND Comfort is Low THEN Fan Speed is High

### 4. Implementasi Sistem

#### A. Tools dan Library yang Digunakan
- Python 3.x
- NumPy: Untuk operasi numerik
- scikit-fuzzy: Untuk implementasi fuzzy logic
- Tkinter: Untuk GUI
- Matplotlib: Untuk visualisasi

#### B. Fitur Sistem
1. **Input Interface**
   - Field untuk memasukkan suhu ruangan
   - Field untuk memasukkan tingkat kenyamanan

2. **Output Display**
   - Menampilkan hasil perhitungan kecepatan kipas
   - Visualisasi kurva keanggotaan

### 5. Cara Penggunaan Sistem

1. Masukkan nilai suhu ruangan (16-30°C)
2. Masukkan nilai tingkat kenyamanan (0-10)
3. Klik tombol "Calculate" untuk mendapatkan hasil
4. Klik tombol "Show Curves" untuk melihat visualisasi

### 6. Keuntungan Sistem

1. **Otomatisasi**: Mengurangi kebutuhan pengaturan manual
2. **Adaptif**: Menyesuaikan dengan kondisi ruangan
3. **User-Friendly**: Interface yang mudah digunakan
4. **Efisiensi**: Optimalisasi penggunaan energi

### 7. Kesimpulan

- Sistem menggunakan 2 input dan 1 output
- Total 9 aturan fuzzy untuk pengambilan keputusan
- Implementasi menggunakan Python dengan GUI
- Visualisasi memudahkan pemahaman sistem

<img width="277" alt="Screenshot 2025-01-09 at 22 13 38" src="https://github.com/user-attachments/assets/fe124541-828c-4030-b107-8e6f27cb6df3" />

<img width="278" alt="Screenshot 2025-01-09 at 22 14 09" src="https://github.com/user-attachments/assets/1339d183-e4b7-4ac5-a78a-524128312c22" />

<img width="278" alt="Screenshot 2025-01-09 at 22 13 58" src="https://github.com/user-attachments/assets/ca20d127-f881-4f40-84ae-5a56bd3b1f43" />

<img width="277" alt="Screenshot 2025-01-09 at 22 13 38" src="https://github.com/user-attachments/assets/f169efcc-0c72-4997-8ac1-fa734c0fbdd8" />


![image](https://github.com/user-attachments/assets/87460797-a4c8-43c3-9864-6beadab701a6)
