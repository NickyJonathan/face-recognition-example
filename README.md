cat <<EOL > README.md
# Dokumentasi Implementasi Model Face Recognition

## Persyaratan:
- Python sudah terinstall di komputer Anda.
- Perangkat kamera (bisa menggunakan kamera laptop atau webcam).

## Langkah-Langkah:

### 1. Ekstrak File
Ekstrak file RAR yang berisi kode program. Pastikan file telah diekstrak di lokasi yang mudah diakses.

### 2. Buka Terminal atau Command Prompt
- Buka **Terminal** untuk pengguna Linux atau macOS.
- Buka **Command Prompt (CMD)** untuk pengguna Windows.
- Arahkan terminal atau CMD ke folder hasil ekstraksi menggunakan perintah:
  \`\`\`bash
  cd /path/ke/folder/hasil/ekstrak
  \`\`\`
  Gantilah \`/path/ke/folder/hasil/ekstrak\` dengan path folder yang sesuai.

### 3. Instalasi Library
Instal library yang dibutuhkan dengan perintah berikut:
\`\`\`bash
pip install opencv-python opencv-contrib-python pillow
\`\`\`
Library yang diinstal adalah:
- **opencv-python**: Untuk pengolahan gambar dan video.
- **opencv-contrib-python**: Untuk algoritma tambahan di OpenCV, termasuk face recognition.
- **pillow**: Untuk mengelola gambar.

### 4. Capture Wajah Mahasiswa
Setelah instalasi selesai, jalankan program untuk mengambil gambar wajah:
\`\`\`bash
python face_taker.py
\`\`\`
Saat diminta, masukkan **username** mahasiswa yang akan di-capture wajahnya. Program akan membuka kamera dan mengambil beberapa gambar wajah.

Ulangi langkah ini untuk setiap mahasiswa yang ingin Anda masukkan ke dalam sistem pengenalan wajah.

### 5. Melatih Model Pengenalan Wajah
Setelah gambar wajah dari beberapa mahasiswa sudah berhasil diambil, lakukan pelatihan model dengan menjalankan:
\`\`\`bash
python face_train.py
\`\`\`
Proses ini akan melatih model menggunakan gambar wajah yang sudah diambil.

### 6. Menjalankan Pengenalan Wajah
Setelah pelatihan model selesai, jalankan program pengenalan wajah:
\`\`\`bash
python face_recognizer.py
\`\`\`
Program ini akan membuka kamera dan mendeteksi wajah-wajah yang sudah pernah dicapture sebelumnya.

## Catatan:
- Pastikan pencahayaan saat mengambil gambar wajah cukup terang agar model pengenalan wajah bekerja lebih baik.
- Jika ada masalah saat instalasi library atau menjalankan program, pastikan Python dan pip sudah terpasang dengan benar.

## Penutup
Dengan mengikuti langkah-langkah di atas, Anda dapat melakukan capture wajah, melatih model pengenalan wajah, dan mendeteksi wajah menggunakan kamera secara real-time.
EOL
