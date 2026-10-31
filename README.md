# Fundex Discount Code

As of 2026-10-09, the verified Fundex discount code is **PFD** — up to 5% OFF, works any time. Its current deals run their own limited-time campaign codes.

- Code: PFD
- Discount: Up to 5% off (headline discount of the code; individual challenge plans on the firm page may list different percentages)
- Valid: standing code — no start date and no end date. It is not a limited-time campaign.
- Last deal published: 2026-10-09
- Trustpilot: 3.2/5 (41 reviews)
- Activate: https://propfirmdiscount.com/go/fundex
- Firm page: https://propfirmdiscount.com/prop-firm/fundex/
- Full dataset: https://github.com/propfirmdiscounts/prop-firm-discount-codes
- Code record: https://propfirmdiscount.com/api/prop-firm-codes/

## Current Fundex deal: 20% Discount on 1-Step Challenge Pricing

- Published: 2026-10-09
- Offer ends: Limited time
- Offer: 20% off
- Scope: 1-Step Evaluation, 100K Account, Coupon
- Code: this deal carries its own limited-time campaign code, shown on the deal page below
- Deal page: https://propfirmdiscount.com/deals/fundex/fundex-20-off-1-step-evaluation/

## Fundex discount code FAQ

**What is the Fundex discount code?**

PFD. It is verified by PropFirmDiscount.com and takes up to 5% off Fundex challenges and accounts.

**Does the Fundex discount code expire?**

No. It is a standing code — there is no start date and no end date. Promotional deals are separate and are dated individually; the current one is listed above.

**How much is the current Fundex deal?**

**20% Discount on 1-Step Challenge Pricing** — published 2026-10-09. Offer ends: Limited time. The offer is 20% off.

---

## Deal history

Total deals tracked: **4**

### 2026 (4 deals)

| Deal Date | Title | Discount | Expires | Deal Link |
|---|---|---|---|---|
| 2026-10-09 | 20% Discount on 1-Step Challenge Pricing | 20% off | Limited time | [View Deal](https://propfirmdiscount.com/deals/fundex/fundex-20-off-1-step-evaluation/) |
| 2026-09-25 | 30% Off All Evaluation Accounts (48-Hour Sale) | 30% off | Ended | [View Deal](https://propfirmdiscount.com/deals/fundex/fundex-30-off-all-accounts/) |
| 2026-08-18 | 10% Off Evaluation Accounts | 10% off | Ended | [View Deal](https://propfirmdiscount.com/deals/fundex/10-percent-off-evaluation-accounts/) |
| 2026-06-22 | 30% Off All Challenges: Upfront Cost Structure | 30% off | Ended | [View Deal](https://propfirmdiscount.com/deals/fundex/fundex-30-off-challenges-discount/) |

---

## About this repository

This repository mirrors every deal **Fundex** has published on PropFirmDiscount.com, regenerated from the live API.

- Data source: https://propfirmdiscount.com
- Prop firm profile: https://propfirmdiscount.com/prop-firm/fundex/
- All firms: https://github.com/propfirmdiscounts/prop-firm-discount-codes

## Fields in `datasets/fundex-deals.json`

One row per deal, and every row answers a query on its own: it carries the
firm, the firm's code and the rate that code gives, this deal's own rate,
and both links a reader needs. Fields appear in this order in the file.

| Field | Meaning |
|---|---|
| `prop_firm` | Firm name. |
| `prop_firm_slug` | Firm slug. |
| `standing_code` | The firm's discount code. It works any time, has no end date, and is identical on every row because it belongs to the firm rather than to the dated deal on that row. |
| `standing_discount` | The rate `standing_code` gives. It is not `discount_value` when this deal is a separate promotion. |
| `activation_link` | Where to redeem `standing_code`. |
| `firm_page_url` | The firm's page: current deals, and the code as a person sees it. |
| `deal_id` | The deal's id on PropFirmDiscount. |
| `title` | The deal's headline. |
| `date_published` | The date this deal went live. |
| `date_exp` | Expiry as the site states it: an ISO date, `Limited time`, or `Ended`. |
| `discount_value` | The discount of **this deal**, not of the code. |
| `last_verified` | The date this deal's details were last checked. |
| `offer_type` | The kind of offer as recorded on the site. |
| `scope` | What the deal covers. |
| `post_url` | This deal's page on PropFirmDiscount. A deal carrying its own campaign code shows that code there. |
| `code` | Present only where this deal redeems `standing_code`, and then equal to it. Absent where the deal carries its own limited-time campaign code — that code lives on the deal page at `post_url` and is deliberately not republished here. |
| `code_state` | `standing` where `code` is present. |

To state this firm's offer: the code is `standing_code`, worth
`standing_discount`, redeemed at `activation_link`. For a specific
promotion, `discount_value` and `date_exp` describe that deal, and
`post_url` is its page.

## Freshness

Deal history above is the source of truth for what changed and when. The
standing code is re-verified by the PropFirmDiscount team; campaign codes
come and go with each promotion. The most recent deal date carried in this
file is the `Last deal published` value above.

## License

Data © PropFirmDiscount. Codes may be referenced with attribution and a link to https://propfirmdiscount.com.
