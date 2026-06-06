# Deploy Veloura

Proyek ini terdiri dari dua bagian:

- `veloura-backend-main`: API Express untuk chat.
- `veloura-fronted-main`: frontend statis.

## Backend ke Vercel

1. Masuk ke folder `veloura-backend-main`.
2. Push ke GitHub.
3. Import repository/folder ini di Vercel.
4. Tambahkan Environment Variable:

```text
GROQ_API_KEY=isi_api_key_groq_kamu
```

5. Deploy.
6. Cek endpoint:

```text
https://domain-backend.vercel.app/
https://domain-backend.vercel.app/test
```

## Frontend ke GitHub Pages atau Vercel

1. Masuk ke folder `veloura-fronted-main`.
2. Push ke GitHub.
3. Deploy sebagai static site.
4. Setelah backend punya domain, set URL backend di `index.html`:

```js
window.VELOURA_API_URL = 'https://domain-backend.vercel.app';
```

Jika frontend dan backend digabung di satu domain Vercel, frontend otomatis memakai `/api/chat`.

## Catatan

File `.env` tidak boleh di-push ke GitHub. Gunakan `.env.example` sebagai contoh saja.
