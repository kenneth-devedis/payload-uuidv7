# Setup

Make sure you have nothing running on port `5432` and `3000`.

```bash
docker compose up -d
pnpm i
cp .env.example .env
pnpm run payload migrate
pnpm run dev
```

Visit `http://localhost:3000/admin/login`

Login repeatedly.