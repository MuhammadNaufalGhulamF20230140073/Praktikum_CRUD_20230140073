# 🚀 User Management API Documentation

**Base URL:** `http://localhost:8080`

---

## 🛠️ Daftar Endpoint (Methods)

### 1. ➕ Tambah User Baru (POST)
**Endpoint:** `/api/users`  
**Fungsi:** Menambahkan data user baru ke database.

**Request Body (JSON):**
```json
{
  "name": "Naufal",
  "age": 22
}
```
Respon Sukses (201 Created):
```json
{
  "status": "success",
  "data": {
    "id": "a2f2f0ac-b23a-4846-813b-fee327de43c3",
    "name": "Naufal",
    "age": 22
  }
}
```

### 2. ➕ Melihat  User (GET)
**Endpoint:** `/api/users`  
**Fungsi:** Melihat data user baru.

**Respon Sukses (200):*

```json

{
"data": [
{
"age": 22,
"id": "a348c6f2-ce5e-486c-8c3a-b78d28b61058",
"name": "Naufal"
}
],
"status": "success"
}
```



### 3. ➕ Edit User  (PUT)
**Endpoint:** `http://localhost:8080/api/users/a348c6f2-ce5e-486c-8c3a-b78d28b61058`  
**Fungsi:** Mengedit data user baru.

**Request Body (JSON):*

```json

{
  "name": "Naufal Update",
  "age": 29
}
```
Respon Sukses (200):
```json
{
    "data": {
        "age": 29,
        "id": "a348c6f2-ce5e-486c-8c3a-b78d28b61058",
        "name": "Naufal Updated"
    },
    "status": "success"
}
```
