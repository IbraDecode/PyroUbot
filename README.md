# PyroUbot

PyroUbot adalah bot Telegram yang powerful dan multifungsi yang dibangun menggunakan Pyrogram dan PyTgCalls. Bot ini menyediakan berbagai fitur untuk mengelola userbot Telegram secara otomatis.

## 🚀 Fitur Utama

- **Multi-Userbot Management**: Kelola hingga 100 userbot secara bersamaan
- **Voice & Video Calls**: Dukungan panggilan suara dan video melalui PyTgCalls
- **Plugin System**: Sistem plugin modular untuk menambah fitur baru
- **Auto Cleanup**: Pembersihan otomatis userbot yang expired
- **Rich Commands**: Berbagai perintah untuk administrasi dan entertainment

## 📋 Persyaratan Sistem

- Python 3.10+
- Node.js & npm (untuk UglifyJS)
- MongoDB (untuk penyimpanan data)

## 🛠️ Instalasi

### 1. Clone Repository
```bash
git clone https://github.com/yourusername/PyroUbot.git
cd PyroUbot
```

### 2. Install Python Dependencies
```bash
pip install -r requirements.txt
```

### 3. Install Node.js Dependencies
```bash
npm install -g uglify-js
```

### 4. Konfigurasi Environment
Salin file `sample.env` ke `.env` dan isi dengan kredensial Anda:
```bash
cp sample.env .env
```

Edit file `.env` dengan:
- `BOT_TOKEN`: Token bot dari @BotFather
- `API_ID` & `API_HASH`: Dari https://my.telegram.org
- `MONGO_URL`: URL koneksi MongoDB
- Dan konfigurasi lainnya sesuai kebutuhan

### 5. Jalankan Bot
```bash
python3 -m PyroUbot
```

## 📁 Struktur Proyek

```
PyroUbot/
├── PyroUbot/
│   ├── __init__.py          # Inisialisasi bot
│   ├── __main__.py          # Entry point utama
│   ├── config.py            # Konfigurasi environment
│   ├── core/
│   │   ├── database/        # Operasi database
│   │   ├── function/        # Fungsi utilitas
│   │   └── helpers/         # Helper functions
│   └── modules/             # Plugin modules
├── requirements.txt         # Python dependencies
├── sample.env              # Template environment
├── start.sh                # Startup script
└── README.md               # Dokumentasi ini
```

## 🔧 Konfigurasi

### Environment Variables
- `MAX_BOT`: Maksimal jumlah userbot (default: 100)
- `DEVS`: ID developer (pisahkan dengan spasi)
- `API_ID`: API ID dari Telegram
- `API_HASH`: API Hash dari Telegram
- `BOT_TOKEN`: Token bot dari BotFather
- `OWNER_ID`: ID owner bot
- `BLACKLIST_CHAT`: ID chat yang di-blacklist
- `RMBG_API`: API key untuk remove background
- `MONGO_URL`: URL MongoDB
- `LOGS_MAKER_UBOT`: ID chat untuk logging

## 📚 Modules

Bot ini memiliki berbagai module yang dapat digunakan:

- **Admin**: Perintah administrasi
- **Music**: Pemutar musik dan panggilan
- **Downloader**: Download dari berbagai platform
- **Games**: Game dan entertainment
- **Utilities**: Tools bermanfaat
- Dan banyak lagi...

## 🤝 Kontribusi

Kontribusi selalu diterima! Silakan:

1. Fork repository
2. Buat branch fitur baru (`git checkout -b feature/AmazingFeature`)
3. Commit perubahan (`git commit -m 'Add some AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Buat Pull Request

## 📄 Lisensi

Distributed under the MIT License. See `LICENSE` for more information.

## ⚠️ Disclaimer

Bot ini untuk tujuan edukasi dan personal use. Pengguna bertanggung jawab atas penggunaan bot ini sesuai dengan Terms of Service Telegram.

## 📞 Support

Jika ada pertanyaan atau masalah:
- Buat issue di GitHub
- Join komunitas Telegram (jika tersedia)

---

**Dibuat dengan ❤️ menggunakan Pyrogram**