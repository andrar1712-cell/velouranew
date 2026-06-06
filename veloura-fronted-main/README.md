# Veloura Frontend

Frontend statis Veloura. Bisa di-host di Vercel, Netlify, atau GitHub Pages.

## Jalankan lokal

Buka `index.html` langsung di browser, atau jalankan static server:

```bash
npx serve .
```

## Hubungkan ke backend

Default chat memakai endpoint `/api/chat`, cocok jika frontend dan API berada di domain Vercel yang sama.

Jika backend ada di domain berbeda, ubah konfigurasi di `index.html`:

```js
window.VELOURA_API_URL = 'https://nama-backend-kamu.vercel.app';
```

Alternatif tanpa edit file, jalankan di console browser:

```js
localStorage.setItem('veloura_backend_url', 'https://nama-backend-kamu.vercel.app');
```

## Deploy ke GitHub Pages

1. Push folder ini ke GitHub.
2. Aktifkan GitHub Pages dari branch utama.
3. Pastikan backend Vercel sudah aktif.
4. Set URL backend lewat konfigurasi di atas.
