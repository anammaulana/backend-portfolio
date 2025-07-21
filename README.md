# backend-portfolio

Keren banget, Anam! Kombinasi **NestJS** untuk backend dan **Vue.js** untuk frontend sangat bagus untuk membangun aplikasi portofolio dan blog yang modern. Aku bantu kamu bikin struktur awal dan fitur-fitur dasar ya.

---

## 🎯 Tujuan Aplikasi:

1. **Portofolio pribadi**: menampilkan proyek, skill, pengalaman.
2. **Blog teknologi**: untuk dokumentasi belajar, tips, atau sharing pengetahuan.

---

## 🏗️ Arsitektur dan Stack

### Backend (NestJS)

* **NestJS** dengan TypeScript
* **PostgreSQL** (atau MongoDB kalau lebih suka NoSQL)
* ORM: **TypeORM** atau **Prisma**
* Auth: **JWT** + **bcrypt**
* REST API (bisa GraphQL kalau mau fleksibel)
* File upload untuk gambar portofolio & thumbnail blog

### Frontend (Vue.js)

* Vue 3 + Composition API
* Pinia (untuk state management)
* Vue Router
* TailwindCSS (opsional tapi cakep)
* Axios untuk komunikasi API

---

## 🧩 Struktur Fitur (Sederhana dulu)

### Auth

* Login Admin
* Middleware untuk melindungi route admin (JWT)

### Blog

* Create, Read, Update, Delete (CRUD) artikel
* Kategori artikel (opsional)
* Slug URL yang SEO friendly
* Markdown support (pakai library seperti `marked.js`)

### Portofolio

* CRUD Proyek
* Gambar proyek + deskripsi
* Link ke GitHub atau live project

### Dashboard Admin

* Kelola artikel
* Kelola proyek portofolio
* Analytics sederhana (jumlah view artikel misalnya)

---

## 🗂️ Struktur Folder (Contoh)

### Backend (NestJS)

```
src/
├── auth/
├── users/
├── blog/
├── portfolio/
├── common/
├── database/
└── main.ts
```

### Frontend (Vue)

```
src/
├── assets/
├── components/
├── pages/
├── router/
├── store/
├── views/
└── App.vue
```

---

## 🔐 Auth Flow Sederhana (JWT)

1. Admin login (POST `/auth/login`) → token JWT
2. Simpan token di localStorage (atau cookie)
3. Tambahkan token di header setiap request ke endpoint yang perlu autentikasi

---

## 🚀 Langkah Selanjutnya

1. **Setup project NestJS**:

   ```bash
   nest new backend-portfolio-blog
   ```

2. **Setup project Vue**:

   ```bash
   npm init vue@latest frontend-portfolio-blog
   ```

3. **Pilih database**: mau pakai PostgreSQL, MongoDB, atau SQLite?

4. **Mulai dari fitur blog atau auth dulu**, baru lanjut ke portofolio.

---

Kalau kamu mau, aku bisa bantuin:

* generate skema database awal
* bikin endpoint backend dasar (login, artikel, proyek)
* atau generate UI template Vue-nya

Kamu mau mulai dari mana dulu? Auth, Blog, atau Portofolio?
