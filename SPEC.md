# InvoicePilot — AI Invoicing for Freelancers

## One-Liner
Describe your project → get a professional invoice in 30 seconds. Track payments, auto-chase late invoices, get paid faster.

## Problem
Freelancers waste 3-5 hours/month on invoicing:
- Formatting invoices manually (Word/Google Docs)
- Tracking who's paid vs. who hasn't
- Awkward follow-up emails for late payments
- Calculating taxes, discounts, project hours

## Solution
AI-powered invoicing that does it all:
1. **Generate** — Describe the project → professional invoice with line items, taxes, payment terms
2. **Send** — Email directly or download PDF
3. **Track** — Dashboard shows paid/pending/overdue at a glance
4. **Chase** — Auto-generate polite → firm follow-up emails based on days overdue
5. **Learn** — AI learns your pricing, common clients, preferred terms

## Competitive Landscape
| Competitor | Price | Gap |
|-----------|-------|-----|
| FreshBooks | $19-60/mo | Overkill for solo freelancers |
| Wave | Free | No AI, clunky, acquired by H&R Block |
| Bonsai | $24-39/mo | Expensive for basic invoicing |
| Invoicely | $9.99-29.99/mo | Dated UI, no AI |
| Paymo | $5.9-11.9/mo | Project management focus |
| Invoice Ninja | Free/OSS | No AI, developer-oriented |
| Deel | $49+/mo | Enterprise, contractor management |
| Copilot | Free tier | Portal-focused, not invoice-first |

**Our gap:** Nobody does AI-generated invoices from natural language for $0-9/mo. Every competitor requires manual line-item entry.

## Ecosystem Fit
IntakeBot (qualify client) → ContractPilot (sign contract) → **InvoicePilot (get paid)** → ReviewAgent (get review)

Completes the freelancer revenue pipeline.

## MVP Features
- Natural language invoice generation ("I did 40 hours of web dev for Acme at $100/hr, net-30")
- Professional PDF output (3 templates: minimal, modern, bold)
- Client database (auto-remember names, addresses, rates)
- Payment status tracking (draft/sent/viewed/paid/overdue)
- Late payment follow-up email generator (3 escalation levels)
- Tax calculation (sales tax / VAT % configurable)
- Multi-currency support
- Recurring invoice templates

## Pricing
- **Free:** 3 invoices/month, 1 template, basic tracking
- **Pro ($9/mo):** Unlimited invoices, all templates, auto-chase, recurring, client database
- **Business ($19/mo):** Team, white-label, Stripe/PayPal integration, expense tracking, reports

## Tech Stack
- Landing page: HTML + Tailwind + client-side demo
- Backend: Shared Vercel serverless (same as other products)
- AI: Claude API for invoice generation + follow-up emails
- PDF: jsPDF client-side (same as ContractPilot)
- Storage: Supabase (shared)

## Revenue Potential
- TAM: 70M+ freelancers globally
- Conversion: Even 0.1% = 70K users → at $9/mo avg = $630K MRR
- LTV: Invoicing is sticky — once set up, hard to switch
- Cross-sell: Every InvoicePilot user is a ContractPilot/IntakeBot prospect
