# Rencana Pembelajaran Semester (RPS) Berbasis OBE
**Mata Kuliah:** Komputasi Tepi (*Edge Computing*)  
**Bobot SKS:** 3 SKS (2 Teori, 1 Praktikum)  
**Semester:** VI (Enam) / Pilihan Konsentrasi  
**Prasyarat:** Sistem Embedded / IoT Dasar, Pengantar Kecerdasan Buatan  

---

## 1. Deskripsi Mata Kuliah
Mata kuliah ini membahas paradigma Komputasi Tepi (*Edge Computing*) dengan fokus pada implementasi *Internet of Things* (IoT) dan *Machine Learning* (ML) pada perangkat dengan sumber daya terbatas (khususnya ESP32). Mahasiswa akan belajar memindahkan beban komputasi analitik dari *cloud* ke *edge* (TinyML), mencakup akuisisi data sensor, pelatihan model ML, kuantisasi model, hingga *deployment* dan *inferencing* lokal di dalam *mikrokontroler* ESP32 untuk menghasilkan sistem cerdas berlatensi rendah dan efisien.

## 2. Capaian Pembelajaran Lulusan (CPL) yang Dibebankan
- **CPL-1 (Sikap):** Menunjukkan sikap bertanggung jawab atas pekerjaan di bidang keahlian informatika/sistem komputer secara mandiri.
- **CPL-2 (Pengetahuan):** Menguasai konsep teoretis dan prinsip arsitektur sistem IoT, *Edge Computing*, dan algoritma *Machine Learning*.
- **CPL-3 (Keterampilan Umum):** Mampu menerapkan pemikiran logis, kritis, sistematis, dan inovatif dalam pengembangan dan implementasi teknologi *Edge AI*.
- **CPL-4 (Keterampilan Khusus):** Mampu merancang, membangun, dan menguji sistem IoT cerdas dengan menanamkan model *Machine Learning* pada *microcontroller* (ESP32) untuk klasifikasi dan prediksi data sensor secara *real-time*.

## 3. Capaian Pembelajaran Mata Kuliah (CPMK)
- **CPMK-1:** Mahasiswa mampu menjelaskan arsitektur *Edge Computing* dan perbandingannya dengan *Cloud Computing* dalam ekosistem IoT.
- **CPMK-2:** Mahasiswa mampu mengakuisisi dan memproses data time-series/sensor menggunakan ESP32 dan mengirimkannya ke *Cloud* untuk pengumpulan dataset.
- **CPMK-3:** Mahasiswa mampu melatih model *Machine Learning* skala kecil (TinyML) menggunakan platform *Edge AI* (misal: Edge Impulse / TensorFlow Lite for Microcontrollers).
- **CPMK-4:** Mahasiswa mampu mengimplementasikan dan mengoptimasi (*deployment*) model ML ke dalam ESP32 untuk melakukan inferensi data sensor secara lokal tanpa koneksi internet.
- **CPMK-5:** Mahasiswa mampu merancang purwarupa akhir *Edge Computing* terintegrasi yang memecahkan masalah nyata (Studi Kasus).

---

## 4. Rencana Kegiatan Pembelajaran Mingguan (16 Pertemuan)

| Minggu | Kemampuan Akhir yang Diharapkan (Sub-CPMK) | Materi Pembelajaran | Bentuk & Metode Pembelajaran | Penilaian (Indikator & Kriteria) | Bobot |
| :---: | :--- | :--- | :--- | :--- | :---: |
| **1** | Mampu menjelaskan konsep dasar *Edge Computing*, IoT, dan TinyML. | 1. Pengenalan *Edge vs Cloud Computing*<br>2. Arsitektur sistem Edge IoT<br>3. Konsep dasar TinyML pada MCU | Kuliah Interaktif, Diskusi<br>*(TM: 2x50", BM: 2x60")* | Ketepatan menjelaskan perbedaan Edge dan Cloud. | 2% |
| **2** | Mampu mengatur lingkungan pengembangan untuk ESP32. | 1. Arsitektur ESP32 (Dual-core, memori, I/O)<br>2. Setup Arduino IDE / PlatformIO<br>3. Pemrograman GPIO dasar | Praktikum, *Project-based*<br>*(TM: 2x50", P: 1x170")* | Keberhasilan konfigurasi environment dan *blink* LED/Sensor. | 3% |
| **3** | Mampu melakukan akuisisi data sensor melalui ESP32. | 1. Integrasi sensor analog & digital (misal: MPU6050, DHT22)<br>2. *Signal processing* dasar di MCU | Praktikum, Demonstrasi<br>*(TM: 2x50", P: 1x170")* | Ketepatan pembacaan dan parsing data sensor. | 5% |
| **4** | Mampu mengirimkan data akuisisi ke *Cloud* atau *Data Logger*. | 1. Protokol MQTT & HTTP POST/GET<br>2. Mengirim data *telemetry* ke Cloud<br>3. Pengumpulan dataset untuk ML | Praktikum, *Problem-based*<br>*(TM: 2x50", P: 1x170")* | Keberhasilan koneksi ESP32 ke broker MQTT dan visualisasi data. | 5% |
| **5** | Mampu memahami *pipeline* Machine Learning untuk *Edge Devices*. | 1. *Pipeline* TinyML (Data -> Latih -> Kuantisasi -> *Deploy*)<br>2. Pengenalan Edge Impulse / TFLite | Kuliah Interaktif, Studi Kasus<br>*(TM: 2x50", P: 1x170")* | Ketepatan merancang alur kerja dari data hingga model. | 5% |
| **6** | Mampu melakukan pra-pemrosesan data dan ekstraksi fitur. | 1. *Windowing* data *time-series*<br>2. Ekstraksi fitur (*Spectral Analysis, FFT, MFCC*)<br>3. Reduksi dimensi | Praktikum, *Hands-on*<br>*(TM: 2x50", P: 1x170")* | Kejelasan dataset dan hasil ekstraksi fitur di platform ML. | 10% |
| **7** | Mampu melatih dan mengevaluasi model Neural Network (NN) skala kecil. | 1. Desain arsitektur NN untuk MCU<br>2. *Training* model klasifikasi<br>3. Analisis *Confusion Matrix* | Praktikum, *Hands-on*<br>*(TM: 2x50", P: 1x170")* | Akurasi model pada *validation set* minimal >85%. | 10% |
| **8** | **Evaluasi Tengah Semester (UTS)** | **Review Materi Minggu 1-7 & Proposal Proyek Akhir** | **Presentasi & Ujian Tulis** | **Kelayakan teknis dari proposal proyek akhir IoT & ML.** | **15%** |
| **9** | Mampu melakukan optimasi dan kuantisasi model untuk ESP32. | 1. *Post-training Quantization* (Float32 ke INT8)<br>2. Trade-off antara ukuran model, RAM, dan akurasi | Kuliah Interaktif, Praktikum<br>*(TM: 2x50", P: 1x170")* | Pemahaman komparasi kinerja model kuantisasi vs *unquantized*. | 5% |
| **10** | Mampu melakukan *deployment* model (C++ Library) ke dalam ESP32. | 1. Ekspor model ML menjadi *library* C++<br>2. Integrasi *library* ke Arduino IDE/PlatformIO<br>3. Manajemen *Memory* ESP32 | Praktikum, *Project-based*<br>*(TM: 2x50", P: 1x170")* | Keberhasilan kompilasi model ML di dalam lingkungan ESP32. | 10% |
| **11** | Mampu mengeksekusi *Local Inferencing* data sensor secara *real-time*. | 1. Menghubungkan *buffer* sensor ke *input tensor* model<br>2. Menjalankan *inference* di ESP32<br>3. Mengukur latensi (*Inference time*) | Praktikum, Eksperimen<br>*(TM: 2x50", P: 1x170")* | Model dapat menebak data *live* dari sensor fisik pada ESP32. | 10% |
| **12** | Mampu merancang aktuasi *Edge-to-Cloud* berdasarkan hasil inferensi. | 1. Memicu aktuator berdasarkan hasil prediksi lokal<br>2. Mengirim log/hasil ke Cloud (saat *event* terjadi) | Praktikum, *Problem-based*<br>*(TM: 2x50", P: 1x170")* | Sistem mampu mengurangi *bandwidth* (hanya mengirim data penting). | 5% |
| **13** | Mampu merancang sistem hemat daya (*Low Power Edge IoT*). | 1. *Deep Sleep* ESP32<br>2. *Wake-up* berbasis interupsi sensor<br>3. Siklus *Wake -> Sense -> Infer -> Sleep* | Praktikum<br>*(TM: 2x50", P: 1x170")* | Keberhasilan implementasi *Deep Sleep* untuk efisiensi daya. | 5% |
| **14** | Pengembangan Proyek Akhir Terintegrasi. | *Mentoring* proyek kelompok (Implementasi E2E: Sensor -> Inferensi ESP32 -> Aktuasi/Cloud) | Pembelajaran Berbasis Proyek (PjBL)<br>*(P: 1x170")* | Progres sistem fisik dan *source code* mencapai 80%. | - |
| **15** | Pengembangan & *Troubleshooting* Proyek Akhir. | Pengujian sistem di lingkungan nyata (*Field Testing*), Kalibrasi model, dan finalisasi laporan. | Pembelajaran Berbasis Proyek (PjBL)<br>*(P: 1x170")* | Kesesuaian sistem dengan perancangan awal. | - |
| **16** | **Evaluasi Akhir Semester (UAS)** | **Demonstrasi Proyek Akhir & Pameran Karya** | **Presentasi Proyek & Tanya Jawab** | **Fungsi alat, kompleksitas ML, akurasi, dan kemampuan komunikasi.** | **10%** |

---

## 5. Sistem Penilaian (OBE Assessment)
Pendekatan penilaian difokuskan pada hasil keluaran teknis dan kemampuan memecahkan masalah.

| Komponen Penilaian | Terkait dengan CPMK | Persentase Bobot | Keterangan |
| :--- | :--- | :---: | :--- |
| **Tugas / Kuis Praktikum** | CPMK-1, CPMK-2 | **20%** | Penilaian kemampuan *coding* dasar ESP32 & IoT. |
| **Praktikum TinyML** | CPMK-3, CPMK-4 | **30%** | Penilaian dari keberhasilan *training* dan *deploy* model di modul Edge Impulse/TFLite. |
| **Ujian Tengah Semester (UTS)** | CPMK-1, CPMK-2 | **15%** | Ujian teori dan pengajuan rancangan proposal purwarupa. |
| **Proyek Akhir Terintegrasi (UAS)** | CPMK-4, CPMK-5 | **35%** | Evaluasi purwarupa fisik, laporan teknis, dan demonstrasi (*Local Inference* berfungsi penuh). |
| **TOTAL** | | **100%** | |

---

## 6. Referensi & Daftar Pustaka

**Buku Utama:**
1. Warden, P., & Situnayake, D. (2019). *TinyML: Machine Learning with TensorFlow Lite on Arduino and Ultra-Low-Power Microcontrollers*. O'Reilly Media.
2. Situnayake, D., & Plunkett, J. (2022). *AI at the Edge: Solving Real-World Problems with Embedded Machine Learning*. O'Reilly Media.

**Referensi Pendukung / Platform:**
- [Dokumentasi Resmi Espressif ESP32](https://docs.espressif.com/)
- [Dokumentasi Edge Impulse](https://docs.edgeimpulse.com/)
- [TensorFlow Lite for Microcontrollers](https://www.tensorflow.org/lite/microcontrollers)

**Perangkat yang Dibutuhkan:**
- **Software:** Arduino IDE / PlatformIO, Akun Edge Impulse, Broker MQTT (Mosquitto/HiveMQ/ThingsBoard).
- **Hardware:** ESP32 Development Board, Kabel Data (Micro-USB/Type-C), Modul Sensor (contoh: IMU MPU6050, DHT22, atau Modul Mic I2S INMP441), Aktuator (Relay/LED).