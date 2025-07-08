# 🚀 Landing Page Deployment di VPS (AWS EC2)

Repositori ini berisi:
- File landing page sederhana (HTML, CSS, JavaScript)
- Contoh konfigurasi NGINX
- Screenshot proses deploy website ke VPS (AWS EC2)


## 📌 Deskripsi Project

- Tujuan: Membuat dan mendistribusikan website statis menggunakan server VPS dengan NGINX.
- Domain: `anisalukman.my.id` atau melalui IP publik.
- Tools & Teknologi:
  - AWS EC2 (Amazon Linux 2023)
  - PuTTY (SSH client)
  - SCP / WinSCP (untuk upload file)
  - NGINX (web server)
  - Custom Domain (opsional)


## 📝 Langkah Singkat Deploy

1. Buat Instance EC2
   - Jalankan Amazon Linux 2023.
   - Buka port 80 (HTTP) dan 443 (HTTPS) di security group.

2. Akses VPS
   - SSH ke instance menggunakan PuTTY.

3. Install & Jalankan NGINX
   ```bash
   sudo yum install nginx -y
   sudo systemctl start nginx
   sudo systemctl enable nginx

4. Upload File Website
   Gunakan SCP atau WinSCP untuk upload file ke /usr/share/nginx/html.

5. Konfigurasi NGINX
   Edit file nginx.conf atau file konfigurasi di /etc/nginx/conf.d/.
   Edit file nginx.conf atau file konfigurasi di /etc/nginx/conf.d/.

6. Edit file nginx.conf atau file konfigurasi di /etc/nginx/conf.d/.
   sudo nginx -t
   sudo systemctl restart nginx

7. sudo systemctl restart nginx
   sudo systemctl restart nginx
