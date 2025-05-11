# 🛢⛽ Analisis Penggunaan Solar Dengan Model Time Series ⛽🛢

Sebuah proyek berbasis *FastAPI* yang dapat memprediksi  *penggunaan solar*, berdasarkan input hari.

## 📁 Struktur File


├── main.py                 # File python yang berisi endpoint API utama

├── expsmooth_model.pkl     # File model Machine Learning yang telah dilatih

├── requirements.txt        # Daftar dependency/library yang dibutuhkan


## ☁ Fitur API ☁

* Prediksi penggunaan solar
* Menerima input melalui metode POST
* Hasil prediksi: Penggunaan solar selama x hari dan total solarnya yang digunakan

## ⚙ Cara Menjalankan

### 1. Clone Repositori

cmd
git clone https://github.com/Qollie/FastAPI_capstone_datmin.git
cd FastAPI_capstone_datmin


### 2. Buat Virtual Environment

cmd
python -m venv .env
.env\Scripts\activate


### 3. Install Dependensi

cmd
pip install -r requirements.txt


### 4. Jalankan API

cmd
uvicorn app:app --reload


### 5. Akses Swagger UI

Buka browser ke:  
👉 [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

## ✏ Contoh JSON Input

json
{
  "steps": 1
}


## ✅ Contoh Output

json
{
    "prediction": [
    "Prediksi pada 2025-05-10 : 28.29 KL",
    "Total prediksi selama 1 hari adalah: 28.29 KL"
  ]
}


Dibuat sebagai bagian dari praktik tahap *Deployment* dengan menggunakan metode *CRISP-DM*.
