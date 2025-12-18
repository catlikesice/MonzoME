# Monzo-Inspired Banking Tracker 🚀

**Full stack fintech clone** built from reverse-engineering Monzo.me via Firefox DevTools. Live demo: [yourapp.vercel.app](https://yourapp.vercel.app)

[![Pots Dashboard](screenshots/pots-dashboard.png)](https://yourapp.vercel.app/pots)
[![API Response](screenshots/api-pots-network.png)](https://yourapp.vercel.app/api/pots)

## 🎯 Features (Matching Monzo UX)

- ✅ **Pots CRUD**: Create/read/update/delete savings pots (`/api/pots`)
- ✅ **Transactions**: List/filter/export (`/api/transactions`)
- ✅ **Real-time transfers**: WebSocket balance updates
- ✅ **Auth**: JWT login/signup
- ✅ **Mobile-first**: Responsive PWA (tested iPhone/Android)

## 🛠 Tech Stack (Monzo-aligned)

| Frontend | Backend | Database | DevOps |
|----------|---------|----------|--------|
| React/Next.js + Tailwind | Go + Gin | PostgreSQL | Docker + GitHub Actions |
| Storybook components | REST APIs | Prisma ORM | Vercel + Railway |

## 🔍 Research → Implementation

### Monzo.me DevTools Capture
**Observed API** → **My exact replica**

| Monzo Endpoint | Response Shape | My Endpoint | Status |
|----------------|----------------|-------------|--------|
| `GET /api/pots` | `[{id, name, balance_cents, color}]` | `/api/pots` ✅ | [Live](https://yourapp.vercel.app/api/pots) |
| `POST /api/transfers` | `{success: true}` | `/api/transfers` ✅ | [Test](https://yourapp.railway.app/api/transfers) |

**Screenshots**: [Pots API](screenshots/api-pots.png) | [Transactions](screenshots/api-transactions.png)

### UI Components (Storybook)
[Interactive demo → username.github.io/storybook/?path=/story/pots--holiday-pot](your-storybook-link)

