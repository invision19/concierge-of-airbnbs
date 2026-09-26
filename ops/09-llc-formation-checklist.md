# Ops 09 — LLC Formation Checklist (Mark J Russell LLC)

The 15-minute path that unblocks everything downstream: Mercury (ops/08) needs a FORMED entity +
EIN. This gets you both. You'll be in three places: your **state Secretary of State** site,
**irs.gov**, then the **Mercury kit**. Total hands-on time ≈ 15–20 min; EIN is instant.

## Have ready before you start (5 min)

- [ ] Your legal name, SSN, and home address (owner/beneficial owner).
- [ ] Payment card for the state formation fee (usually **$50–$300** by state; most are
      $100–$150; the exact number is the state's "LLC filing fee" on its SOS site).
- [ ] The business address for the LLC (street address; a home address works).
- [ ] Registered agent decision — see step 4. Default: **yourself** (free).

## Form the LLC (10 min)

1. [ ] Open `<your state> Secretary of State · business entity search` and confirm
       **"Mark J Russell LLC"** is available in your state (search also "Mark J Russell" without
       LLC). If it's taken, choose a close variant (e.g. "MJ Russell LLC") and keep the DBA
       "Concierge of Airbnbs" doing the branding — the DBA form (forms/01) already covers that.
2. [ ] Start the **online LLC formation / "Articles of Organization"** filing. Fields you'll
       answer: legal name (Mark J Russell LLC), business address, registered agent (yourself),
       organizer/manager names, and your signature/consent. There is no "incubator"/"pending"
       checkmark — you want the state to ARRIVE at **Approved / Active**.
3. [ ] Pay the filing fee. The state returns a stamped/confirmation — the **formation
       certificate / Articles of Organization** with the entity's **formation date**.
4. [ ] Registered agent: self-registering is free and fine. If your state strongly recommends
       an agent service (rarely required for a single-owner LLC), skip it — self is enough here.
5. [ ] **Save the formation certificate** into `entity-docs/_identity/`:
       `mkdir -p entity-docs/_identity && chmod 600 entity-docs/_identity/*` — this whole
       directory is git-ignored (PII policy: identity records live here, emailed only).
       Note the **formation date** — Mercury's kit asks for it.

## Get the EIN (5 min, free, instant)

6. [ ] IRS: https://www.irs.gov/ein · "Apply for an EIN online". Answer SS-4 questions:
       LLC, formed under your state, principal officer = you (your SSN), reason = "Started new
       business", establishment date = the formation date from step 5.
7. [ ] Save the **EIN confirmation letter (CP 575/PDF)** into `entity-docs/_identity/`
       (chmod 600). This EIN is what Mercury underwrites on — NOT your personal credit.

## Then Mercury (10 min)

8. [ ] Open `ops/08-mercury-application-kit.md` and complete the application with the values
       there — entity = Mark J Russell LLC, EIN + formation date from steps 5/7. You complete
       the **owner identity/KYC screen** in your own browser (government ID + sometimes a
       proof-of-life check) — that step is never done by an assistant.

## Gotchas

- **No extra cost for "expedited" or "rush"** at this stage — normal processing is fine.
- If the state shows a "**Dissolved/Inactive**" match of the name you wanted, just pick the
  clean available variant — don't fight it.
- EIN and formation are FREE at the real sites (SOS filing fee aside). Anyone charging you to
  "register your business" or "get your EIN" is a duplicate-paperwork middleman — skip them.
- After Mercury opens: EIN-only tradelines + Nav (ops/07) build the business credit file.
  The DBA filing (Phase 1, roadmaps) still gets done at your county — it pairs the DBA name to
  the LLC publicly, and Mercury accepts the legal name with DBA branding regardless.
