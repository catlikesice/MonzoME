# Monzo API/UI Capture Sheet

## Pots Dashboard

| API Endpoint | Method | Request | Response | UI Selector | CSS Classes |
|--------------|--------|---------|----------|-------------|-------------|
| `/api/pots` | GET | - | `[{id, name, balance_cents, color}]` | `.pot-card` | `bg-gradient p-4 rounded-xl` |
| `/api/pots/:id` | PATCH | `{amount_cents: 1000}` | `{success: true}` | `.transfer-form` | `shadow-lg` |

## Transactions

| API Endpoint | Method | Request | Response | UI Selector | CSS Classes |
|--------------|--------|---------|----------|-------------|-------------|
| `/api/transactions` | GET | `?limit=20` | `[{id, amount, merchant, category}]` | `.transaction-row` | `flex py-3 border-b` |
```

**Paste into**: VS Code (`Ctrl+P` → `monzo-research.md`), GitHub.com new file, or Notion.

## Quick generators

- **TableFlip.app**: Type headers → auto-generates Markdown table → copy.
- **GitHub**: New repo file → paste headers → Tab between cells → auto-formats.
- **VS Code extension**: "Markdown Table Creator" (Ctrl+Shift+P → "Table").

## Fill from DevTools (30 seconds)

```
1. F12 → Network → Pots page loads
2. Right-click GET /api/pots → Copy Response → Paste into "Response" cell
3. Elements → Click pot → Copy selector → Paste into "UI Selector"
4. Done—table auto-aligns
```

Commit: `git add docs/; git commit -m "Added Monzo research capture sheet"`. Recruiters clone and see your process immediately.
