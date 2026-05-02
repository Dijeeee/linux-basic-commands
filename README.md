#🔍 Nmap Basic Scanning & Pentesting

Repository ini berisi dokumentasi pembelajaran dasar penggunaan Nmap untuk melakukan scanning jaringan dan pengenalan dasar penetration testing secara legal di lingkungan sendiri.

🧑‍💻 Tentang Project

Project ini dibuat sebagai bagian dari pembelajaran Cyber Security dasar, khususnya dalam memahami:

Network scanning
Port discovery
Service detection
Basic penetration testing
🛠️ Tools & Teknologi
Nmap
Kali Linux / Ubuntu
Terminal Linux
⚠️ Disclaimer

Semua aktivitas scanning dilakukan hanya pada:

Jaringan pribadi / lokal
Target yang memiliki izin

IP address pada repository ini telah disamarkan:

192.168.xxx.xxx
🚀 Cara Menggunakan Nmap (Step by Step)
1. Install Nmap
sudo apt update
sudo apt install nmap
2. Cek Instalasi
nmap --version
📌 Jenis Scanning Menggunakan Nmap
🔎 1. Scan Host (Ping Scan)

Mengetahui apakah host aktif atau tidak.

nmap 192.168.xxx.xxx
🔐 2. Scan Port (Range Port)

Mengetahui port yang terbuka.

nmap -p 1-1000 192.168.xxx.xxx
🧠 3. Service Version Detection

Mengetahui versi service yang berjalan.

nmap -sV 192.168.xxx.xxx
⚡ 4. Stealth Scan (SYN Scan)

Scan cepat dan lebih “silent”.

sudo nmap -sS 192.168.xxx.xxx
🧪 5. OS Detection

Mengetahui sistem operasi target.

sudo nmap -O 192.168.xxx.xxx
🔥 6. Aggressive Scan

Scan lengkap (port + service + OS).

sudo nmap -A 192.168.xxx.xxx
🌐 7. Scan Domain / Website

Digunakan untuk scanning domain.

nmap example.com
⚙️ 8. Scan Semua Port

Scan seluruh port (1–65535).

nmap -p- 192.168.xxx.xxx
💾 9. Simpan Hasil Scan

Menyimpan hasil scan ke file.

nmap -oN scan-result.txt 192.168.xxx.xxx
📊 Contoh Hasil Scan
PORT     STATE SERVICE
22/tcp   open  ssh
80/tcp   open  http
443/tcp  open  https
