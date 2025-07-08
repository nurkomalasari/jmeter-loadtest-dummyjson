# 🚀 JMeter Load Testing – DummyJSON API

![JMeter CI](https://github.com/nurkomalasari/jmeter-loadtest-dummyjson/actions/workflows/jmeter-ci.yml/badge.svg)

## 📌 Endpoint
**GET** [`https://dummyjson.com/products`](https://dummyjson.com/products)  
Mengambil data daftar produk dari API publik DummyJSON.

---

## 🎯 Tujuan
Simulasikan **50 pengguna secara bersamaan** untuk mengakses endpoint `GET /products`, guna mengukur performa dan stabilitas respon server.

---

## ⚙️ Konfigurasi JMeter
- **Threads (Users)**: 50  
- **Ramp-Up Time**: 10 detik  
- **Loop Count**: 1  
- **Assertion**: Response body harus mengandung keyword `"products"`

---

## 📊 Contoh Hasil Pengujian
| Metode | Avg Time | Error | Throughput | APDEX |
|--------|----------|-------|------------|--------|
| GET /products | ~190 ms | 0% | ~45 req/sec | 0.6

