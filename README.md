# Laravel Integration Service (3-Service Architecture)

Nama Kelompok 9
Anggota : 
Alief sukma dewanta (1204220030)
Ramadhani Vanva Fauzia (1204220068)

Repositori ini berisi 3 layanan Laravel yang saling terintegrasi:

- **Service A (Pelanggan_service)** – Service data pelanggan CRUD
- **Service B (Produk_service)** – Service data Produk CRUD
- **Service C (Order_service)** – Service data Order CRUD

## 🧱 Struktur Folder


## 🚀 Port & Perintah Jalankan

| Service   | Fungsi               | Port Laravel | Jalankan dengan                                 
|-----------|----------------------|--------------|---------------------------------|
| Service A | data pelanggan CRUD  | 8001         | `php artisan serve --port=8001` |
| Service B | data Produk CRUD     | 8002         | `php artisan serve --port=8002` |
| Service C | data Order CRUD      | 8003         | `php artisan serve --port=8003` |


## 🔗 Contoh Endpoint API

- `GET http://localhost:8001/api/customers` → (pelanggan dari service A)  
- `GET http://localhost:8002/api/menus` → (Product dari Service B)
- `GET http://localhost:8003/api/orders` → (Orders dari Service C)

---

## ⚙️ Instalasi & Setup

Lakukan untuk setiap folder service:

```bash
composer install
npm install
npm install boostrap-icons boostrap
cp .env.example .env
php artisan key:generate
php artisan migrate
