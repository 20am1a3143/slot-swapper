# SlotSwapper Backend

## Setup
1. Install deps
```bash
npm install
```

2. Environment (`.env` in backend)
```
DATABASE_URL="postgresql://user:password@localhost:5432/slot_swapper?schema=public"
JWT_SECRET="change-me"
PORT=4000
```

3. Prisma
```bash
npx prisma migrate dev --name init
npx prisma generate
```

4. Run
```bash
npm run dev
```

5. Test
```bash
npm test
```

## API
- POST /api/auth/signup
- POST /api/auth/login
- GET /api/events
- POST /api/events
- PUT /api/events/:id
- DELETE /api/events/:id
- GET /api/swappable-slots
- POST /api/swap-request
- POST /api/swap-response/:requestId
- GET /api/swap-requests
