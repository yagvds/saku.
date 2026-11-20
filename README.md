# Saku – Finansial lebih terarah

Situs statis satu file (`index.html`), tanpa build step. Data pengguna disimpan di localStorage browser masing-masing; tidak ada server atau database.

## Deploy ke Vercel (gratis)

**Lewat GitHub**
1. Buat repo baru di GitHub, unggah `index.html` dan `vercel.json` di root repo.
2. Di vercel.com pilih Add New → Project → import repo tersebut.
3. Framework Preset: Other. Kosongkan Build Command dan Output Directory. Klik Deploy.

**Lewat CLI**
```
npm i -g vercel
cd saku-vercel
vercel --prod
```

## Catatan
- Aplikasi mulai dalam kondisi kosong: tidak ada akun, transaksi, anggaran, target, atau utang contoh.
- Tiap pengunjung hanya melihat datanya sendiri di browser-nya. Data hilang jika data browser dibersihkan, jadi gunakan Pengaturan → Privasi & data → Unduh cadangan.
- Untuk sinkron antar perangkat dan login sungguhan, tahap berikutnya adalah menambah backend (mis. Supabase).
