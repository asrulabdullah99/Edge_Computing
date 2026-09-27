# Praktikum 1: Pengenalan GPIO Output (Blink LED)

**Mata Kuliah:** Internet of Things (IoT)  
**Topik:** Pengenalan GPIO Output Blink LED (Aktuator)  
**Perangkat:** ESP32 Development Board (atau mikrokontroler sejenis)

---

## 1. Tujuan Praktikum
* Memahami struktur dasar program mikrokontroler (fungsi `setup()` dan `loop()`).
* Mampu mengonfigurasi pin General Purpose Input/Output (GPIO) sebagai keluaran (Output).
* Mampu memberikan sinyal digital tegangan tinggi (`HIGH`) dan rendah (`LOW`) untuk mengendalikan komponen fisik (LED).

## 2. Kebutuhan Perangkat keras
1. 1x ESP32 Development Board
2. 1x Kabel Micro-USB / USB-C (sesuai tipe board) untuk koneksi dan daya
3. 1x LED
4. Kabel Jumper / Wire
5. Resistor 220 Ohm (jika diperlukan)
6. Breadboard (jika diperlukan)

---

## 3. Kode Program (Source Code)

Salin kode berikut ke dalam editor kode (Arduino IDE atau berkas `main.cpp` di PlatformIO):

```cpp
/**
 * Proyek      : Praktikum 1 - Blink LED (IoT Hello World)
 * Deskripsi   : Mengendalikan LED internal agar berkedip dengan interval 1 detik.
 */

const int ledPin = 2; 

void setup() { 
  pinMode(ledPin, OUTPUT); 
}

void loop() { 
  digitalWrite(ledPin, HIGH);  
  delay(1000);                 
  
  digitalWrite(ledPin, LOW);  
  delay(1000);                 
}
```

---

## Tugas Eksperimen Mandiri (Challenge)
Untuk mendalami konsep di atas, cobalah modifikasi kode program Anda untuk menyelesaikan tantangan berikut:

1. **Ubah Kecepatan:** Ubah nilai di dalam fungsi `delay()` agar LED berkedip sangat cepat (misal: 200 milidetik). Perhatikan apa yang terjadi.
2. **Pola Asimetris:** Buat agar durasi menyala lebih lama (misal 2 detik) dibandingkan durasi mati (0.5 detik).
3. **Pesan Darurat (SOS):** Modifikasi blok `loop()` untuk membuat pola kedipan sinyal morse SOS:
   * 3 kedipan cepat (titik)
   * 3 kedipan lambat (garis)
   * 3 kedipan cepat (titik)
   * Jeda 3 detik sebelum mengulang kembali pola.