# 🚀 JMeter Load Testing – DummyJSON API

## 📌 Endpoint
GET https://dummyjson.com/products

## 🎯 Tujuan
Simulasikan 50 pengguna mengakses daftar produk secara bersamaan

## ⚙️ Konfigurasi
- Threads: 50
- Ramp-Up: 10 detik
- Loop: 1
- Assertion: response harus mengandung `"products"`

## 📊 Contoh Hasil
- Avg Response Time: ~190ms
- Error Rate: 0%
- Throughput: ~45 request/sec

## 📂 Cara Menjalankan
```bash
jmeter -n -t Request Load Test.jmx -l results.jtl -e -o report/
