# SkorUp full-stack starter

A deployable Next.js starter for the SkorUp AI Money & Credit dashboard. It uses mock/demo data by default and provides server API routes ready to be connected to authorized credit, banking and AI providers.

## Run
```bash
npm install
npm run dev
```
Open http://localhost:3000.

## Integration boundaries
- `src/app/api/dashboard/route.ts`: replace demo payload with authenticated banking/credit provider calls.
- `src/app/api/ai/route.ts`: connect an approved AI provider server-side.
- Do not collect SSNs or bureau credentials in this starter. Use an authorized provider's hosted/tokenized flow and obtain consumer consent.
- A soft-pull/prequalification workflow should remain clearly distinguished from any later hard inquiry.
