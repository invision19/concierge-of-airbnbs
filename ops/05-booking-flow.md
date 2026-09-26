# Ops 05 — Booking & Transaction Flow (runbook)

The middleman loop for every stay. Source of truth for who pays what when — keep the ledger
(ops/06-booking-ledger.csv) current per step 6.

## Flow

1. **Inquiry** — Renter sends dates/location/guests. Reconciling: which roster owner covers
   it live (availability + pricing honored as listed).
2. **Offer** — Present 1–3 confirmed options with all-in price: stay + cleaning + concierge
   fee, disclosed up front (Form 03 §4).
3. **Book** — Renter signs the booking acknowledgment (Form 03 renter block) and pays the
   full amount to the concierge account.
4. **Hold** — Funds held; owner notified; listing blocked for those dates; renter gets
   confirmation with the updated owner/emergency contact (Form 03 §5).
5. **Stay** — Renter checks in per listing rules. Damage window: owner claim + photos within
   48h of check-out (Form 03 §7).
6. **Settle** — Disburse owner payout within 3 business days of check-in completion
   (or per the set hold policy). Deduct cleaning + concierge fee. Write the row to the ledger.
7. **Close** — Emails: renter receipt (paid/handled), owner payout statement (booked,
   collected, fee, paid). File under the booking reference.

## Money rules

- **One pot:** renters pay the concierge account; owners get paid from it. Nothing is
  "chased" between parties.
- **Ownership changes:** anything tied to a stay completed before the Change of Ownership
  Effective Date settles with the prior owner (Form 02 §3) — confirm before disbursing.
- **Cancellations:** per Form 03 §6; rebooks happen at the concierge level before any refunds
  leave the pot.
- **Never disburse to an unverified account** — payout routing in Form 03 §4 or paid-with,
  verified as part of onboarding.

## Recommended fee (placeholder — user to set)

Flat option: **$35/booking** · Percent option: **20% of the stay** (incl. cleaning). The fee
is disclosed to both sides and deducted at settlement (Form 03 §4).

## Bookkeeping per stay (also in the CSV)

Booking ref · Renter (initials only for PII-lean ledger) · Property/listing · Dates ·
Gross stay · Cleaning · Concierge fee · Owner payout · Platform fee (if any) · Status .
