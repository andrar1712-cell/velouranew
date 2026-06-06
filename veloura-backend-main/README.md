# Veloura Backend

Backend Express untuk chat Veloura memakai Groq API.

## Jalankan lokal

```bash
npm install
copy .env.example .env
npm run dev
```

Isi `GROQ_API_KEY` di file `.env`.

## Deploy ke Vercel

1. Push folder ini ke GitHub.
2. Import repository ke Vercel.
3. Set Environment Variable `GROQ_API_KEY`.
4. Deploy.

Endpoint utama:

- `GET /`
- `POST /api/chat`
- `GET /test`
