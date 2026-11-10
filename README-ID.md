# TWIST Automation Studio

Repository untuk website katalog automation dan kumpulan template workflow n8n, termasuk kebutuhan UMKM, customer support, crypto, konten, edukasi, dan event.

## Website

https://twist5202-ux.github.io/automation/

**Catatan:** alamat website publik tersebut dihosting melalui repo GitHub Pages. Perubahan di repo `twist-automation` belum tentu langsung terlihat di website publik sebelum kontennya disinkronkan ke repo yang melakukan deploy.

## Struktur project

```text
twist-automation/
├── index.html             # Landing page utama
├── automation/
│   ├── index.html         # Halaman katalog automation
│   ├── umkm/              # Template UMKM
│   ├── crypto/            # Template crypto
│   ├── cs/                # Template customer service
│   └── ...                # Kategori lainnya
├── cs/                    # Halaman demo customer support
├── demo/                  # Halaman demo
├── fashion/               # Halaman terkait fashion
├── harga/                 # Halaman harga
├── n8n/                   # Materi dan dokumentasi n8n
├── n8n-crypto/            # Koleksi workflow crypto lainnya
├── build.py               # Script generator yang sudah ada
├── README.md              # Dokumentasi English
└── README-ID.md           # Dokumentasi Indonesia
```

## Cara melihat website secara lokal

Jalankan perintah ini dari folder repository:

```bash
python -m http.server 8000
```

Buka http://localhost:8000/ atau http://localhost:8000/automation/.

## Cara menggunakan template n8n

1. Pilih file workflow `.json` sesuai kebutuhan.
2. Import ke aplikasi n8n.
3. Periksa setiap node, credential, webhook, integrasi, dan nilai placeholder.
4. Uji workflow sebelum mengaktifkannya.

Template mungkin memerlukan konfigurasi tambahan sebelum siap digunakan.

## Penting sebelum merapikan struktur

- Jangan langsung menghapus direktori yang mirip atau memindahkan file tanpa mengecek semua link.
- Perubahan CSS dan JavaScript perlu dites karena sebagian masih berada di file HTML.
- Sinkronisasi ke repo GitHub Pages perlu dikelola secara terpisah.
- Jangan simpan API key, token bot, atau credential aktif di repository.
- Pastikan tampilan dan animasi tetap normal di desktop maupun HP.

Dokumentasi security research berada di repository [security-writeups](https://github.com/twist5202-ux/security-writeups).
