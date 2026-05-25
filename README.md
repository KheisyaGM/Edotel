🚀 tefa_myedotel
A new Flutter project for TeFa MyEdotel.

📑 Project Documentation
Untuk detail rencana pengembangan proyek ini, silakan cek:

📄 Implementation Plan
🛠️ Getting Started
Project ini adalah starter untuk aplikasi Flutter.

Referensi belajar Flutter:

https://docs.flutter.dev/get-started/learn-flutter
https://docs.flutter.dev/get-started/codelab
https://docs.flutter.dev/reference/learning-resources
🔄 FLOW GIT (WAJIB DIPAHAMI)
1️⃣ Clone Project (Pertama Kali)
git clone https://github.com/NauvalFaiz/TeFa_MyEdotel.git
cd TeFa_MyEdotel
2️⃣ Setup Branch
Cek branch:

git branch
Jika masih master, ubah ke main:

git branch -M main
3️⃣ Push Pertama Kali
git add .
git commit -m "Initial commit"
git push -u origin main
4️⃣ Push Rutin (Update Kode)
git add .
git commit -m "Deskripsi perubahan"
git push origin main
5️⃣ Pull Update dari GitHub
git pull origin main
⚠️ ERROR YANG SERING TERJADI + SOLUSI
❌ 1. error: failed to push some refs
Penyebab: Repository GitHub sudah memiliki perubahan terbaru.

Solusi:

git pull origin main
git push origin main
Jika muncul editor (Vim):

tekan ESC
ketik :wq
Enter
❌ 2. Permission denied (HTTPS / SSH)
Penyebab: Autentikasi gagal

🔐 Solusi HTTPS
Gunakan Personal Access Token (PAT) Bukan password GitHub

Buat di: https://github.com/settings/tokens

🔐 Solusi SSH (Rekomendasi)
Cek koneksi:

ssh -T git@github.com
Jika belum ada SSH key:

ssh-keygen -t ed25519 -C "email@example.com"
Tambahkan ke GitHub: Settings → SSH and GPG Keys

❌ 3. src refspec main does not match any
Penyebab: Belum commit

Solusi:

git add .
git commit -m "initial commit"
git push origin main
❌ 4. remote origin already exists
Penyebab: Remote sudah ada

Solusi:

git remote set-url origin https://github.com/NauvalFaiz/TeFa_MyEdotel.git
❌ 5. File > 100MB (Limit GitHub)
Pesan:

File is 120MB; exceeds GitHub limit
✔️ Solusi 1 (Disarankan)
Gunakan .gitignore

Contoh:

*.zip
*.mp4
*.apk
/build/
✔️ Solusi 2 (Jika wajib upload file besar)
Gunakan Git LFS:

Install: https://git-lfs.com/

git lfs install
git lfs track "*.zip"
git add .gitattributes
git add .
git commit -m "Add large files with LFS"
git push
💻 CATATAN PENTING
✔ Bisa dijalankan di:

Git Bash
CMD
PowerShell
Terminal Linux / macOS
✔ Pastikan sudah install:

Git → https://git-scm.com/
Flutter → https://docs.flutter.dev/get-started/install
🔥 BEST PRACTICE
Selalu git pull sebelum git push
Gunakan pesan commit yang jelas
Jangan upload file besar sembarangan
Gunakan .gitignore dari awal
📌 Repository
https://github.com/NauvalFaiz/TeFa_MyEdotel.git
