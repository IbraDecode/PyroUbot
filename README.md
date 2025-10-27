# 🔥 PyroUbot

<div align="center">
  <img src="https://img.shields.io/github/stars/IbraDecode/PyroUbot?style=for-the-badge&logo=github" alt="Stars">
  <img src="https://img.shields.io/github/forks/IbraDecode/PyroUbot?style=for-the-badge&logo=github" alt="Forks">
  <img src="https://img.shields.io/github/issues/IbraDecode/PyroUbot?style=for-the-badge&logo=github" alt="Issues">
  <img src="https://img.shields.io/github/license/IbraDecode/PyroUbot?style=for-the-badge&logo=github" alt="License">
  <br>
  <img src="https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python" alt="Python">
  <img src="https://img.shields.io/badge/Pyrogram-2.0+-red?style=for-the-badge&logo=telegram" alt="Pyrogram">
  <img src="https://img.shields.io/badge/MongoDB-Cloud-green?style=for-the-badge&logo=mongodb" alt="MongoDB">
</div>

---

## 📖 Tentang PyroUbot

**PyroUbot** adalah bot Telegram yang powerful dan multifungsi yang dibangun menggunakan **Pyrogram** dan **PyTgCalls**. Bot ini dirancang untuk mengelola userbot Telegram secara otomatis dengan fitur-fitur canggih dan sistem plugin yang modular.

### ✨ Keunggulan

- 🚀 **Performa Tinggi**: Menggunakan Pyrogram untuk API Telegram yang stabil
- 🎵 **Voice & Video Calls**: Dukungan panggilan suara dan video melalui PyTgCalls
- 🤖 **Multi-Userbot**: Kelola hingga 100 userbot secara bersamaan
- 🔌 **Plugin System**: Sistem plugin modular untuk kemudahan pengembangan
- 🧹 **Auto Cleanup**: Pembersihan otomatis userbot yang expired
- 📊 **Monitoring**: Sistem monitoring dan logging yang comprehensive
- 🎮 **Entertainment**: Berbagai fitur hiburan dan utility

---

## 🛠️ Quick Start

### Persyaratan Sistem

| Komponen | Versi Minimum | Keterangan |
|----------|---------------|------------|
| Python | 3.10+ | Runtime utama |
| Node.js | Latest | Untuk UglifyJS |
| MongoDB | 4.0+ | Database penyimpanan |
| RAM | 512MB+ | Minimum untuk operasi |
| Storage | 1GB+ | Untuk cache dan logs |

### Instalasi Cepat

```bash
# Clone repository
git clone https://github.com/IbraDecode/PyroUbot.git
cd PyroUbot

# Install dependencies
pip install -r requirements.txt
npm install -g uglify-js

# Setup environment
cp sample.env .env
# Edit .env dengan kredensial Anda

# Jalankan bot
python3 -m PyroUbot
```

---

## 📋 Daftar Fitur Lengkap

### 🤖 Userbot Management
- ✅ Multi-account management (hingga 100 bot)
- ✅ Auto-login dan session management
- ✅ Userbot expiration monitoring
- ✅ Bulk userbot operations

### 🎵 Media & Entertainment
- 🎵 **Music Player**: Spotify, YouTube, SoundCloud
- 📹 **Video Calls**: Group voice/video calls
- 🎬 **Downloader**: Instagram, TikTok, YouTube, Twitter
- 🎨 **Image Tools**: Remove BG, enhancer, converter
- 🎮 **Games**: Tic-tac-toe, quiz, mini-games

### 🛠️ Utilities
- 📊 **System Monitor**: CPU, RAM, disk usage
- 🌤️ **Weather**: Cuaca real-time
- 📅 **Reminder**: Scheduled notifications
- 🔍 **Search**: Google, Wikipedia, lyrics
- 💱 **Converter**: Currency, units, formats
- 📝 **Notes**: Personal notes dan reminders

### 👮‍♂️ Administration
- 🚫 **Anti-Spam**: Auto-mute/ban spammers
- 👥 **Group Management**: Welcome, rules, moderation
- 📢 **Broadcast**: Mass messaging
- 🔒 **Security**: Anti-flood, anti-porn
- 📈 **Analytics**: User statistics

### 🎨 Creative Tools
- 🎨 **Logo Maker**: Custom logo generator
- ✏️ **Text Tools**: Stylish text, fonts
- 🖼️ **Image Editor**: Filters, effects, stickers
- 🎭 **Fun**: Memes, quotes, jokes

---

## 🚀 Instalasi Detail

### 1. Persiapan Sistem

```bash
# Update sistem
sudo apt update && sudo apt upgrade -y

# Install Python 3.10+
sudo apt install python3.10 python3.10-venv -y

# Install Node.js
curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
sudo apt-get install -y nodejs

# Install MongoDB (opsional, bisa pakai cloud)
sudo apt install mongodb -y
```

### 2. Setup Project

```bash
# Clone repository
git clone https://github.com/IbraDecode/PyroUbot.git
cd PyroUbot

# Buat virtual environment
python3 -m venv venv
source venv/bin/activate  # Linux/Mac
# atau venv\Scripts\activate  # Windows

# Install Python packages
pip install -r requirements.txt

# Install Node.js packages
npm install -g uglify-js
```

### 3. Konfigurasi Environment

```bash
# Copy template
cp sample.env .env

# Edit file .env
nano .env  # atau editor favorit Anda
```

**Isi file .env dengan:**

```env
# Bot Configuration
MAX_BOT=100
DEVS=6924389613
API_ID=your_api_id
API_HASH=your_api_hash
BOT_TOKEN=your_bot_token
OWNER_ID=6924389613

# Database
MONGO_URL=mongodb+srv://username:password@cluster.mongodb.net/dbname

# APIs (opsional)
RMBG_API=your_removebg_api_key
OPENAI_API=your_openai_key

# Logging
BLACKLIST_CHAT=-1002125842026 -1002056443221
LOGS_MAKER_UBOT=-1002807087960
```

### 4. Mendapatkan Kredensial

#### Bot Token
1. Buka [@BotFather](https://t.me/botfather) di Telegram
2. Kirim `/newbot`
3. Ikuti instruksi untuk membuat bot
4. Copy token yang diberikan

#### API ID & Hash
1. Kunjungi https://my.telegram.org
2. Login dengan akun Telegram
3. Buat aplikasi baru
4. Copy API ID dan API Hash

#### MongoDB URL
- **Cloud**: Gunakan [MongoDB Atlas](https://cloud.mongodb.com)
- **Local**: `mongodb://localhost:27017/pyroubot`

### 5. Menjalankan Bot

```bash
# Development mode
python3 -m PyroUbot

# Production mode (recommended)
python3 -m PyroUbot > logs.txt 2>&1 &

# Using startup script
chmod +x start.sh
./start.sh
```

---

## 📁 Struktur Proyek

```
PyroUbot/
├── PyroUbot/
│   ├── __init__.py              # Bot initialization
│   ├── __main__.py              # Main entry point
│   ├── config.py                # Environment configuration
│   └── core/
│       ├── database/            # Database operations
│       │   ├── __init__.py
│       │   ├── ubot.py         # Userbot database
│       │   └── vars.py         # Global variables
│       ├── function/
│       │   ├── __init__.py
│       │   ├── plugins.py      # Plugin loader
│       │   └── inline.py       # Inline functions
│       └── helpers/
│           ├── __init__.py
│           ├── _cmd.py         # Command decorators
│           ├── formatter.py    # Text formatting
│           └── misc.py         # Miscellaneous helpers
├── modules/                     # Plugin modules (200+ files)
│   ├── admin.py                 # Admin commands
│   ├── music.py                 # Music player
│   ├── downloader.py            # Media downloader
│   ├── games.py                 # Games & entertainment
│   └── ...                      # Other modules
├── requirements.txt             # Python dependencies
├── sample.env                  # Environment template
├── start.sh                    # Startup script
├── installnode.sh              # Node.js installer
├── README.md                   # This documentation
└── LICENSE                     # MIT License
```

---

## 🎯 Cara Penggunaan

### Menambah Userbot

1. **Via Bot Commands**:
   ```
   /add_ubot - Mulai proses penambahan userbot
   ```

2. **Manual Setup**:
   - Bot akan meminta nomor telepon
   - Masukkan kode verifikasi
   - Bot akan membuat session otomatis

### Perintah Dasar

| Perintah | Deskripsi |
|----------|-----------|
| `/start` | Memulai bot |
| `/help` | Menampilkan bantuan |
| `/ping` | Cek status bot |
| `/stats` | Statistik penggunaan |
| `/ubot` | Kelola userbot |

### Advanced Commands

```
# Admin Commands
/add_ubot     - Tambah userbot baru
/del_ubot     - Hapus userbot
/list_ubot    - List semua userbot
/restart      - Restart bot

# Music Commands
/play         - Putar musik
/pause        - Pause musik
/skip         - Skip lagu
/queue        - Lihat antrian

# Utility Commands
/weather      - Cek cuaca
/remind       - Set reminder
/translate    - Terjemahkan teks
/download     - Download media
```

---

## 🔧 Troubleshooting

### Masalah Umum

#### 1. Import Error
```bash
# Install missing packages
pip install geopy speedtest-cli pytimeparse
```

#### 2. MongoDB Connection Failed
```bash
# Check MongoDB status
sudo systemctl status mongodb

# Or use cloud MongoDB Atlas
# Update MONGO_URL in .env
```

#### 3. Bot Token Invalid
```
- Pastikan token dari @BotFather valid
- Jangan bagikan token ke orang lain
- Regenerate token jika compromised
```

#### 4. API ID/Hash Invalid
```
- Kunjungi https://my.telegram.org
- Buat aplikasi baru jika perlu
- Pastikan API credentials benar
```

#### 5. FloodWait Error
```
- Bot terkena limit rate Telegram
- Tunggu beberapa menit
- Kurangi frekuensi request
```

### Logs & Debugging

```bash
# View logs
tail -f logs.txt

# Debug mode
python3 -m PyroUbot --debug

# Check system resources
htop
df -h
free -h
```

---

## 🤝 Kontribusi

Kami sangat menghargai kontribusi dari komunitas! 🚀

### Cara Berkontribusi

1. **Fork** repository ini
2. **Clone** fork Anda: `git clone https://github.com/username/PyroUbot.git`
3. **Buat branch** fitur: `git checkout -b feature/AmazingFeature`
4. **Commit** perubahan: `git commit -m 'Add some AmazingFeature'`
5. **Push** ke branch: `git push origin feature/AmazingFeature`
6. **Buat Pull Request**

### Guidelines

- ✅ Ikuti PEP 8 style guide
- ✅ Tambahkan docstrings pada functions
- ✅ Test kode sebelum submit
- ✅ Update dokumentasi jika diperlukan
- ❌ Jangan commit file sensitif (.env, credentials)

### Contributors

Terima kasih kepada semua yang telah berkontribusi! 🙏

<a href="https://github.com/IbraDecode/PyroUbot/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=IbraDecode/PyroUbot" />
</a>

---

## 📄 Lisensi

**PyroUbot** didistribusikan di bawah lisensi **MIT License**.

```
MIT License - see the LICENSE file for details.
```

---

## ⚠️ Disclaimer & Terms

### Penggunaan

- Bot ini untuk **tujuan edukasi dan personal use** saja
- **Dilarang** menggunakan untuk spam, phishing, atau aktivitas ilegal
- Pengguna bertanggung jawab penuh atas penggunaan bot ini

### Terms of Service

- Patuhi [Terms of Service Telegram](https://telegram.org/tos)
- Jangan abuse API rate limits
- Respect privacy pengguna lain

### Support

Jika ada pertanyaan atau masalah:

- 🐛 **Issues**: [GitHub Issues](https://github.com/IbraDecode/PyroUbot/issues)
- 💬 **Discussions**: [GitHub Discussions](https://github.com/IbraDecode/PyroUbot/discussions)
- 📧 **Email**: ibradecode@gmail.com

---

## 🙏 Credits & Attribution

**Dibuat dengan ❤️ oleh [Ibra Decode](https://github.com/IbraDecode) dan teman-teman yang telah berkontribusi.**

### Special Thanks

- **Pyrogram Team** - Library utama
- **PyTgCalls Team** - Voice/video calls
- **MongoDB** - Database solution
- **Community Contributors** - Bug fixes & features

### Tech Stack

- **Backend**: Python 3.10+, Pyrogram, PyTgCalls
- **Database**: MongoDB
- **Frontend**: Telegram Bot API
- **Deployment**: VPS/Cloud servers

---

<div align="center">

**⭐ Jika Anda menyukai proyek ini, berikan star di GitHub!**

[![GitHub stars](https://img.shields.io/github/stars/IbraDecode/PyroUbot.svg?style=social&label=Star)](https://github.com/IbraDecode/PyroUbot)
[![GitHub forks](https://img.shields.io/github/forks/IbraDecode/PyroUbot.svg?style=social&label=Fork)](https://github.com/IbraDecode/PyroUbot)

---

**PyroUbot © 2024. Made with ❤️ in Indonesia**

</div>