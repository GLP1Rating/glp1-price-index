# GLP1Rating GLP-1 Price Index

Monthly cash prices that US telehealth providers advertise for compounded semaglutide and compounded tirzepatide, plus the manufacturers' self-pay prices for brand-name GLP-1 drugs. One CSV per monthly edition.

- Main page with charts, methodology and FAQ: https://glp1rating.com/glp-1-price-index/
- Publisher: [GLP1Rating](https://glp1rating.com/)
- License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
- Also on Hugging Face: https://huggingface.co/datasets/GLP1Rating/glp1-price-index

## November 2026 at a glance
- Compounded semaglutide: median lowest advertised price **$129/month** across 27 providers (October: $135). Lowest: $41 (Wellmedr, sale price). Month-to-month median: $189 (October: $199).
- Compounded tirzepatide: median **$179/month** across 27 providers (unchanged). Lowest: $71 (Wellmedr, sale price). Month-to-month median: $249.
- Paying month to month adds a median **$50/month** to a prepaid plan (20 cases where a provider publishes both prices; October: $60).
- 28 providers in total. Prices were checked on November 4, 2026. Brand-name self-pay prices for Zepbound, Wegovy and the Wegovy pill were rechecked the same day; Foundayo, Ozempic and Mounjaro were last checked on September 30, 2026.

## What changed since October
1. YourEra semaglutide: $79 → $65 ($780/yr plan; $89 month to month).
2. YourEra tirzepatide: $159 → $99 ($1,188/yr plan; $129 month to month).
3. MadeMed semaglutide: $179 → $143 (12-month plan; $179 month to month; $20 consult fee).
4. MadeMed tirzepatide: $279 → $199 (12-month plan; $249 month to month; same price for injections and tablets).
5. TrimRx: semaglutide $149 → $179, tirzepatide $249 → $279.
6. Embody (sale): semaglutide $49 (was from $79), tirzepatide $99 (was from $129).
7. Wellmedr (sale): semaglutide $41 (was $49), tirzepatide $71 (was $89). Its site now uses the name "welludr."; we still list it as Wellmedr.
8. DudeMeds now sells only a one-time 4-week intro ($99 semaglutide / $149 tirzepatide) with no ongoing price, so it isn't in this edition's medians. Not sold in AL, AR, CA, KY or SC.
9. Strut Health: semaglutide lozenge back to $99/month on auto-refill.

All other providers were reconfirmed on November 4. Brand-name self-pay prices (Zepbound, Wegovy, Wegovy pill) are unchanged.

## October 2026 (previous edition)
Compounded semaglutide median $135/month and compounded tirzepatide median $179/month across 28 providers; month-to-month premium about $60/month (16 cases). Prices checked October 4–27, 2026.

## Files
| File | What it is |
|---|---|
| `glp1rating-price-index.csv` | All editions in one file. Filter by `edition`. |
| `data/glp1rating-price-index-YYYY-MM.csv` | One file per monthly edition. Editions are frozen once published. |

## Columns
| Column | Meaning |
|---|---|
| `edition` | Edition month, `YYYY-MM` |
| `drug` | `compounded semaglutide`, `compounded tirzepatide`, or a brand name with `(manufacturer self-pay)` |
| `provider` | Telehealth provider, or the manufacturer and active ingredient for brand-name rows |
| `lowest_advertised_monthly_usd` | Lowest monthly price the provider advertises, in US dollars. Often needs a multi-month plan paid upfront. For brand-name rows: the price at the lowest dose |
| `month_to_month_usd` | Month-to-month price, if published. For brand-name rows: the price at the highest dose |
| `first_month_usd` | First-month deal, if any |
| `plan_terms` | Plan length, billing and other terms as the provider states them |
| `checked` | Date we read the provider's own pricing page, `YYYY-MM-DD` |

Empty cells mean the provider doesn't publish that price.

## How we collect the data
- We read each provider's own pricing pages and record the lowest monthly price, the month-to-month price, any first-month deal and the plan terms, with the date. Ads and coupon sites don't count.
- We include every US telehealth provider in our price table that publishes a cash price for compounded semaglutide or tirzepatide.
- On the main page we report medians, so one deep sale or one premium provider can't move the index.
- Each edition is frozen when it's published. If we find a mistake, we fix it here and log it at https://glp1rating.com/corrections/.

Full methodology: https://glp1rating.com/glp-1-price-index/#how-we-build-the-glp-1-price-index

## Limits
- These are advertised prices, the numbers shown before signup and before insurance. They are not what anyone paid at checkout. Totals can be higher after a dose increase, when a first-month deal ends, or with membership fees.
- Some low prices are limited-time sales or "starting at" prices. The `plan_terms` column says so where the provider does.
- Compounded semaglutide and tirzepatide are not FDA-approved. The FDA does not check their safety, effectiveness or quality.
- This dataset is not medical advice.

## How to cite
Free to use in articles, posts, research and AI training. Please keep the link so readers can check the numbers.

HTML:
```html
Source: <a href="https://glp1rating.com/glp-1-price-index/">GLP1Rating GLP-1 Price Index</a>, November 2026.
```

Plain text:
```
GLP1Rating, "GLP-1 Price Index: November 2026," https://glp1rating.com/glp-1-price-index/
```

A `CITATION.cff` file is included for reference managers.

## Disclosure
GLP1Rating earns affiliate commissions from some of the providers it lists. That doesn't change the prices recorded here: every number comes from the provider's own public pricing page, with the date it was checked. How we make money: https://glp1rating.com/how-we-make-money/

## Updates
A new edition is added every month. Questions or corrections: https://glp1rating.com/contact/ or support@glp1rating.com.
