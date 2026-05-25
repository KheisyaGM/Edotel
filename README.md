# 🚀 TeFa MyEdotel

A new Flutter project for **TeFa MyEdotel**.

---

# 📑 Project Documentation

Untuk detail rencana pengembangan proyek ini, silakan cek:

* 📄 **Implementation Plan**

---

# 🛠️ Getting Started

Project ini merupakan starter project untuk aplikasi Flutter.

## 📚 Referensi Belajar Flutter

* [https://docs.flutter.dev/get-started/learn-flutter](https://docs.flutter.dev/get-started/learn-flutter)
* [https://docs.flutter.dev/get-started/codelab](https://docs.flutter.dev/get-started/codelab)
* [https://docs.flutter.dev/reference/learning-resources](https://docs.flutter.dev/reference/learning-resources)

---

# 🔄 Git Flow (WAJIB DIPAHAMI)

## 1️⃣ Clone Project (Pertama Kali)

```bash
git clone https://github.com/NauvalFaiz/TeFa_MyEdotel.git
cd TeFa_MyEdotel
```

---

## 2️⃣ Setup Branch

Cek branch saat ini:

```bash
git branch
```

Jika masih menggunakan `master`, ubah menjadi `main`:

```bash
git branch -M main
```

---

## 3️⃣ Push Pertama Kali

```bash
git add .
git commit -m "Initial commit"
git push -u origin main
```

---

## 4️⃣ Push Update Kode

```bash
git add .
git commit -m "Deskripsi perubahan"
git push origin main
```

---

## 5️⃣ Pull Update dari GitHub

```bash
git pull origin main
```

---

# ⚠️ Error yang Sering Terjadi + Solusi

## ❌ 1. `error: failed to push some refs`

### Penyebab

Repository GitHub sudah memiliki perubahan terbaru.

### Solusi

```bash
git pull origin main
git push origin main
```

Jika muncul editor **Vim**:

1. Tekan `ESC`
2. Ketik:

```bash
:wq
```

3. Tekan `Enter`

---

## ❌ 2. `Permission denied (HTTPS / SSH)`

### Penyebab

Autentikasi gagal.

---

### 🔐 Solusi HTTPS

Gunakan **Personal Access Token (PAT)**, bukan password GitHub.

Buat PAT di:

[https://github.com/settings/tokens](https://github.com/settings/tokens)

---

### 🔐 Solusi SSH (Rekomendasi)

Cek koneksi SSH:

```bash
ssh -T git@github.com
```

Jika belum memiliki SSH key:

```bash
ssh-keygen -t ed25519 -C "email@example.com"
```

Tambahkan SSH key ke GitHub melalui:

`Settings → SSH and GPG Keys`

---

## ❌ 3. `src refspec main does not match any`

### Penyebab

Belum melakukan commit.

### Solusi

```bash
git add .
git commit -m "Initial commit"
git push origin main
```

---

## ❌ 4. `remote origin already exists`

### Penyebab

Remote repository sudah ada sebelumnya.

### Solusi

```bash
git remote set-url origin https://github.com/NauvalFaiz/TeFa_MyEdotel.git
```

---

## ❌ 5. File > 100MB (Limit GitHub)

### Pesan Error

```bash
File is 120MB; exceeds GitHub limit
```

---

### ✔️ Solusi 1 (Disarankan)

Gunakan `.gitignore`.

Contoh:

```gitignore
*.zip
*.mp4
*.apk
/build/
```

---

### ✔️ Solusi 2 (Jika Wajib Upload File Besar)

Gunakan **Git LFS**.

Install Git LFS:

[https://git-lfs.com/](https://git-lfs.com/)

```bash
git lfs install
git lfs track "*.zip"
git add .gitattributes
git add .
git commit -m "Add large files with LFS"
git push
```

---

# 💻 Catatan Penting

## ✔️ Terminal yang Bisa Digunakan

* Git Bash
* CMD
* PowerShell
* Terminal Linux / macOS

---

## ✔️ Pastikan Sudah Install

* Git → [https://git-scm.com/](https://git-scm.com/)
* Flutter → [https://docs.flutter.dev/get-started/install](https://docs.flutter.dev/get-started/install)

---

# 🔥 Best Practice

* Selalu lakukan `git pull` sebelum `git push`
* Gunakan pesan commit yang jelas
* Jangan upload file besar sembarangan
* Gunakan `.gitignore` sejak awal project

---

# 📌 Repository

```bash
https://github.com/NauvalFaiz/TeFa_MyEdotel.git
```
