# Linux Command & Nmap Basic Pentesting

Repository ini berisi dokumentasi pembelajaran mengenai penggunaan Linux Command dan Nmap untuk kebutuhan administrasi sistem serta pengenalan dasar penetration testing secara legal.

---

## Tujuan Project

Project ini dibuat sebagai media belajar untuk memahami:

- Dasar penggunaan Terminal Linux
- Navigasi file dan direktori
- Manajemen file
- Permission pada Linux
- Network Scanning menggunakan Nmap
- Service Enumeration
- Host Discovery
- Port Scanning
- Banner Grabbing

---

## Tools

- Kali Linux
- Ubuntu
- Nmap
- Bash Terminal
- VirtualBox

---

## Materi Linux Command

### Navigasi

- pwd
- ls
- cd
- tree

### Manajemen File

- mkdir
- touch
- cp
- mv
- rm

### Melihat Isi File

- cat
- less
- head
- tail

### Permission

- chmod
- chown
- sudo

### Networking

- ip
- ping
- traceroute
- netstat
- ss

---

# Materi Nmap

## Host Discovery

```bash
nmap 192.168.1.1
```

Melakukan pengecekan apakah host aktif.

---

## Scan Seluruh Port

```bash
nmap -p- 192.168.1.1
```

Melakukan scanning seluruh port TCP.

---

## Service Detection

```bash
nmap -sV 192.168.1.1
```

Menampilkan versi service yang berjalan.

---

## Operating System Detection

```bash
sudo nmap -O 192.168.1.1
```

Mendeteksi sistem operasi target.

---

## Aggressive Scan

```bash
sudo nmap -A 192.168.1.1
```

Melakukan:

- OS Detection
- Version Detection
- Script Scanning
- Traceroute

---

## Scan Jaringan

```bash
nmap 192.168.1.0/24
```

Mendeteksi host aktif dalam satu jaringan.

---

## Contoh Output

```text
PORT     STATE SERVICE VERSION

22/tcp   open  ssh
80/tcp   open  http
443/tcp  open  https
```

---

## Struktur Repository

```
linux-basic-commands/
│
├── README.md
├── linux-command/
│   ├── navigation.md
│   ├── file-management.md
│   ├── permission.md
│   └── networking.md
│
├── nmap/
│   ├── host-discovery.md
│   ├── port-scanning.md
│   ├── service-detection.md
│   ├── os-detection.md
│   └── examples.md
│
└── images/
```

---

## Yang Dipelajari

- Linux Fundamental
- Command Line Interface
- Network Scanning
- Enumeration
- Basic Penetration Testing
- Cyber Security Fundamental

---

## Disclaimer

Repository ini dibuat hanya untuk tujuan edukasi.

Seluruh contoh scanning dilakukan pada:

- Virtual Machine
- Localhost
- Lab pribadi
- Target yang memiliki izin

Dilarang menggunakan materi ini untuk aktivitas yang melanggar hukum.

---

## Author

Nama: Dije Jato

Mahasiswa Informatika

Learning Cyber Security • Linux • Networking • Penetration Testing
