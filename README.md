# Credit price calculator

Private tool. Live page: GitHub Pages on this repo (`Settings -> Pages`).

Per-widget credit pricing against live fal provider cost, with gross margin on all
three subscription plans at once.

- **12 Month** - $49.99/yr, 8,000 cr/mo -> $0.000520729 per credit
- **Monthly** - $14.99/mo, 8,000 cr/mo -> $0.001873750 per credit
- **Weekly** - $5.99/wk, 2,000 cr/wk -> $0.002995000 per credit

Rule of thumb: at 20% gross margin on Monthly, price = provider cost x 667 credits.
That same price yields about -188% on 12 Month and +50% on Weekly. The Monthly
margin has to reach 72.2% before 12 Month breaks even.

Costs captured 2026-09-01 from the fal model catalog and model pages; credit
prices from the production persona endpoint. Re-run the audit to refresh - the
dataset is inlined as `const DATA` in `index.html`.

Contains provider costs and margins. Keep this repository private.
