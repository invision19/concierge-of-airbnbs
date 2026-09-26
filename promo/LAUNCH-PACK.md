# Launch Pack — ready to fire (paste-ready)

Post copy as-cut. Post 1 ships with `promo/assets/post1-card.png`. Buffer wiring on this machine
is currently unusable (token is a Public API token; legacy REST retired — see note below), so post
to the channels directly — 2 minutes, no adspend.

## Post 1 — X / IG (the never-seen angle)

> Airbnb sold. Next guest already booked. Nobody noticed — because the doorman was on duty.
> Concierge of Airbnbs: bookings, the money, and the ownership-change paperwork, handled. 🎩
> by Mark J Russell
> 🔔 https://invision19.github.io/concierge-of-airbnbs/

Art: `promo/assets/post1-card.png` (VACANT ✕ flipping to OCCUPIED — "came back handled").

## Post 2 — Local / FB owner groups

> Selling your Airbnb? Your _calendar_ isn't for sale. We close the loop a transfer usually
> breaks — Change of Ownership + updated addendum, notarized, and your booked guests never feel
> it. Free printable set in the link.
> 🔔 https://invision19.github.io/concierge-of-airbnbs/forms-pack.html

## Post 3 — Email / mailer (first 20 warm contacts)

> **Dear host —**
> when your keys change hands, most agencies drop at least one booking. Ours is the one that
> doesn't. Reply and we'll put your listing on the board — first five stays, concierge fee on us.
> 🔔 https://invision19.github.io/concierge-of-airbnbs/

## Buffer note (why this is paste-and-post)

The machine's `~/.buffer_token` is a **Public API token**; the Buffer legacy REST API now rejects
it (HTTP 401 "Public API tokens are not accepted for REST API access", API sunset 2027-02-01).
Until the account rotates in an OAuth access token (or migrates to Buffer's GraphQL API with auth),
posts can't be scheduled from here. When that's wired, these three go out as a scheduled queue.

## Tracking

Every CTA already carries a tracked mailto subject (index / doorman / forms-pack). Tally the
subjects after week 1 — that's the ad budget.
