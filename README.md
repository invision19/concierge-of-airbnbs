# Concierge of Airbnbs — Launch Pack

Rebrand & product line for **Mark J Russell LLC** operating as **Concierge of Airbnbs**.
Mark J Russell LLC is, and remains, the legal entity and the alias/operator name;
**Concierge of Airbnbs** is the operating (DBA) brand under which the business is sold.
This is the working project root.

## Brand map

| Name                                    | Role                                                           |
| --------------------------------------- | -------------------------------------------------------------- |
| **Concierge of Airbnbs**                | Public brand, DBA, site name — what customers see              |
| **Mark J Russell / Mark J Russell LLC** | Legal entity + operator alias — what filings and contracts say |

## What's here

```
concierge-of-airbnbs/
├── README.md                      this file (launch roadmap)
├── naics-codes.md                 NAICS codes — DECIDED 2026-09-26 (primary 531110)
├── forms/
│   ├── 01-dba-name-form.md        DBA application (Mark J Russell LLC → Concierge of Airbnbs)
│   ├── 02-change-of-ownership-form.md   ownership-change form set for rental/hosting ops
│   └── 03-addendum-updated.md     updated Addendum (ownership change + current terms)
├── ops/                           operations pack (drafted)
│   ├── 04-owner-onboarding.md     owner intake record + onboarding checklist
│   ├── 05-booking-flow.md         middleman booking/transaction runbook + fee placeholder
│   └── 06-booking-ledger.csv      per-booking ledger (bookkeeping + tax)
├── promo/
│   └── PROMO-PLAYBOOK.md          launch engine: style kit, 3 ready posts, partner
│                                  handshakes, referral mechanics, order of ops
└── docs/                          served to GitHub Pages (branch main, path /docs)
    ├── index.html                 sales/concierge page (brand: Concierge of Airbnbs)
    ├── doorman.html               interactive "the doorman is in" promo page (buzzboard)
    └── forms-pack.html            printable/notarizable form set (DBA · ownership · addendum)
```

## Launch roadmap

### ⬜ Phase 1 — Entity & filings

1. [ ] File/renew the **DBA**: Mark J Russell LLC, conducting business as **Concierge of Airbnbs** (`forms/01-dba-name-form.md` — fill, sign, file with your county).
2. [ ] Lock the LLC's **NAICS** on EIN / business license / tax returns — **DECIDED: primary `531110` (Airbnb rental per user directive)**, secondary `561599` booking/concierge, `561410` document prep (`naics-codes.md`).
3. [ ] Open a **separate business bank account** in the DBA name (needed for the middleman transaction flows).

### ⬜ Phase 2 — Offer & forms

4. [ ] Adopt the form set: `02-change-of-ownership-form.md` + `03-addendum-updated.md` (owner/renter signature set, printable — see `docs/forms-pack.html`).
5. [ ] Have an attorney/lawyer review the documents once before first use (templates, not legal advice).
6. [x] Add the form set to the site as a service line — DONE (`docs/forms-pack.html` linked from the forms section).

### ⬜ Phase 3 — Site

7. [x] Hosted — **LIVE** at <https://invision19.github.io/concierge-of-airbnbs/> (GitHub Pages, served from `/docs`; `index.html` + `doorman.html` + `forms-pack.html` all 200, mailto CTAs verified resolving in production).
8. [ ] Set the real business inbox — CTAs currently wired to `jkcontractorsllc1@gmail.com` (marketing/dev inbox); update the single `CONTACT_EMAIL` constant in `docs/index.html` + `docs/doorman.html` when a dedicated business inbox exists, then push to re-deploy automatically.

### ⬜ Phase 4 — Operations

9. [x] Owner-side intake documented — `ops/04-owner-onboarding.md` (onboarding + Change-of-Ownership checklist). Pending first real owner.
10. [x] Renter-side booking flow documented — `ops/05-booking-flow.md` (inquiry → offer → book → hold → stay → settle → close). Pending launch.
11. [ ] Set the concierge fee — placeholder in `ops/05-booking-flow.md` ($35/flat or 20% recommended); set before first booking.
12. [x] Transaction ledger template ready — `ops/06-booking-ledger.csv`. Pending first booking.

## Compliance notes (read before use)

- The LLC is the **middleman/concierge** — bookings and transactions flow THROUGH it per the agreements. It is not an Airbnb brand and not a listing platform owner.
- Forms are **templates for document preparation services** — not legal advice; professional review recommended before first use (per `naics-codes.md` note).
- No clinical/PHI exposure (not applicable here); still: no guest SSN/PII beyond what the transaction legally requires, and never store more than the booking needs.
- State/county DBA rules vary — the DBA form is a generic template; confirm your county's official form/format.

## Current status

- [x] Brand structure decided (DBA "Concierge of Airbnbs", alias "Mark J Russell").
- [x] Form set drafted (ownership change + addendum) and site scaffolded AND hosted at <https://invision19.github.io/concierge-of-airbnbs/>.
- [ ] User steps: file DBA, confirm NAICS, open business bank account, set fee.
