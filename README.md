# Kalkulator Integral Metode Simpson

Aplikasi web interaktif untuk menghitung integral tentu dari data diskrit menggunakan **Metode Simpson 1/3 dan Simpson 3/8**. Cocok buat tugas kuliah, analisis data statistik, atau numerik teknik.

---

## Apa Itu Metode Simpson?

Metode Simpson adalah pendekatan numerik untuk menghitung nilai integral tentu dari suatu fungsi dengan menggunakan nilai-nilai diskrit dari fungsi tersebut. Alih-alih menggunakan rumus integral analitik, metode ini membagi area di bawah kurva menjadi bagian-bagian kecil dan memperkirakannya dengan polinomial.

### Tujuan:
Mendekati luas area di bawah kurva $f(x)$ di interval $[a, b]$ berdasarkan titik-titik data yang diketahui.

---

## Jenis-Jenis Metode Simpson

### Simpson 1/3 Rule
- Digunakan saat jumlah **subinterval (n)** genap.
- Menggunakan **parabola (polinomial orde 2)** untuk interpolasi.
- Rumus:
  \[
  \int_a^b f(x) dx \approx \frac{h}{3} \left[f(x_0) + 4f(x_1) + 2f(x_2) + \dots + 4f(x_{n-1}) + f(x_n)\right]
  \]

### Simpson 3/8 Rule
- Digunakan saat jumlah **subinterval (n)** kelipatan 3.
- Menggunakan **polinomial orde 3 (kubik)** untuk interpolasi.
- Rumus:
  \[
  \int_a^b f(x) dx \approx \frac{3h}{8} \left[f(x_0) + 3f(x_1) + 3f(x_2) + 2f(x_3) + \dots + f(x_n)\right]
  \]

---

## ⚙Syarat Penggunaan
- Titik-titik $x$ harus memiliki **jarak (h)** yang konstan.
- Data $f(x)$ harus tersedia secara diskrit.
- Jumlah titik tergantung pada metode:
  - Simpson 1/3 → $n$ genap → jumlah titik = n + 1 (ganjil)
  - Simpson 3/8 → $n$ kelipatan 3 → jumlah titik = 3k + 1

---

## Keunggulan
- Akurat untuk fungsi yang halus (kontinu dan terdiferensialkan).
- Lebih efisien daripada metode trapesium.
- Cocok untuk kasus real-world dengan data diskrit seperti:
  - Jumlah penduduk pertahun
  - Sensor suhu/humidity per detik
  - Curah hujan bulanan, dll.

---
