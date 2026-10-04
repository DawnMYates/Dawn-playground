# Sunday Reading — October 4, 2026

**Series:** Exceptional recent long-form on financial-system risk  
**Focus this week:** public-debt stock, the non-bank footprint, and the distribution of Treasury-market dysfunction

---

## The piece

**Mathias Drehmann and Sonya Zhu, “High public debt, NBFIs and the risk of market dysfunction”**  
*BIS Bulletin No. 136*, September 29, 2026  
https://www.bis.org/publications/bulletin-136-high-public-debt-nbfis-and-risk-market-dysfunction  
PDF: https://www.bis.org/publications/bulletin-136-high-public-debt-nbfis-and-risk-market-dysfunction.pdf

Eight pages. Not a crash call and not a valuation essay. A distributional forecast of U.S. Treasury market conditions, asking how the government-debt stock and the non-bank footprint change the odds of future market dysfunction — including in states where today’s liquidity still looks fine.

September 20 was Sgambati on the political economy of that release valve. September 27 was Filia on equity prices as the margin loan. This week is the official-sector quantification of the sovereign-market tail those two essays describe.

---

## Why it is worth reading

The Friday dashboard already says the surface is calm and the pressure gauges are not. FINRA debit balances are $1,453.8 billion (August), still +37.2% year over year. CAPE is 41.07 and the Buffett indicator is about 234%. Funding is amber: SOFR has plateaued in the high 3.80s to 3.90s, equity-financing terms are rich, and Treasury repo has not seized. Credit has only just left the fully calm zone (HY OAS 3.24%). VIX closed at 15.31 in contango.

Those readings tell you *today’s level*. Drehmann and Zhu tell you what today’s debt stock and non-bank share do to the *three-month-ahead distribution* of Treasury-market functioning. The useful result is not “high debt is bad.” It is that a large non-bank footprint makes very good liquidity more likely *and* dysfunction more likely. Orderly repo and a green VIX are compatible with a fatter left tail. That is the mismatch the overall read already flags, stated as a probability rather than a vibe.

---

## Main thesis

Near-record government debt and a larger non-bank role have reshaped government-debt markets. High public debt worsens expected future liquidity in general and raises the risk of market dysfunction. A large NBFI footprint heightens that dysfunction risk while also making unusually favourable liquidity more likely. The two together are a fiscal–financial stability nexus: a yield jump can be amplified by non-bank fire sales, which further strains fiscal space.

How they measure it:

- **Sample.** U.S. only, July 2004–May 2024. Debt is debt-to-GDP. The NBFI footprint is the share of government bonds held by money-market funds, investment funds, pension funds, and insurers (flow of funds). Hedge funds are discussed and then left out of the regression, because the historical holdings series does not exist.
- **Target.** The Treasury market-conditions indicator (MCI) from Aldasoro et al. (2025): the first principal component of the MOVE index, a government-securities liquidity index, quoted spreads and time-to-quote, the on-the-run premium, the absolute OIS–Treasury spread, and the absolute Treasury futures basis. Mean zero, unit variance. Higher is worse. March 2020 is about a six-standard-deviation shock; November 2008, February 2016, and October 2022 are about two.
- **Method.** A random forest trained to the full three-month-ahead conditional distribution of the MCI, rolling out of sample after an initial seven-year window. Debt-to-GDP and the NBFI share are added to the existing predictor set. High and low are top and bottom terciles.

The numbers that matter:

- In the top debt-to-GDP tercile, the probability of a GFC-like stress event — MCI above the October–December 2008 range — within three months is **3%**, against **0.02%** in the bottom tercile. Average MCI is 0.40 in the top debt tercile versus 0.23 in the bottom.
- A high NBFI share widens both tails. The probability that MCI is below its 20th percentile (−0.78, unusually good liquidity) is essentially zero when the share is low and **7%** when it is high. The probability it is above the 80th percentile (0.75) is essentially zero when low and **12%** when high.
- In the top NBFI-share tercile, the probability of a GFC-like event is **1.5%**, versus close to zero when the share is low. In the top decile of the NBFI share that probability rises to **6%**.
- Shapley values rank debt-to-GDP and the NBFI share among the predictors that actually move the right tail. The NBFI share is eighth overall for the 95th percentile of MCI.

The mechanism is the one the project has already been circling, now with a feedback loop attached. High debt means a fiscal shock is priced as a larger risk premium, so yields rise and liquidity worsens. Non-banks then amplify the move, but not all in the same way: open-ended and money-market funds via redemption runs (March 2020), insurers and pension funds via margin and collateral calls on hedges (the 2022 LDI template, where forced gilt sales accounted for about half the peak-to-trough price drop), and hedge funds via repo-funded basis and cash–futures books that supply liquidity in calm markets and dump it when the arb is a few basis points against them. Hedge-fund exposure to U.S. government debt has more than doubled since 2022; in European electronic government-debt markets they account for over half of trading. The bulletin’s line is that market functioning is especially at risk “if the initial jump in yields is amplified by any of the discussed NBFI vulnerabilities, which in turn can further undermine fiscal space.”

Policy close, not a trade: credible medium-term fiscal frameworks, and “congruent regulation” — same stringency for the same risk, whatever the legal wrapper — aimed at leverage, liquidity mismatch, and fragile funding that can amplify stress in the government-bond market.

---

## What it adds beyond the market-cycle signals already tracked

Mapped against the October 2, 2026 Margin Debt Cycle Dashboard:

| Dashboard gauge | What you already have | What Drehmann and Zhu add |
| --- | --- | --- |
| Funding Stress Watch (SOFR 3.87%, Treasury repo not seized, equity-financing terms rich; Amber) | A spot check that the pipes are not seized this week | A three-month-ahead distribution. High debt shifts the whole future MCI worse. A large non-bank share fattens both tails, so “repo not seized” is the good-liquidity state their model says is *also* more likely — it does not clear the dysfunction state |
| Rate of Change (FINRA debit $1,453.8bn, +37.2% YoY) | The visible brokerage-margin stock | A different leverage stock: the sovereign market as collateral for non-bank books. Their empirical NBFI share excludes hedge funds. The 1.5% GFC-like probability is therefore a lower bound on the non-bank channel the September SCOOS is already flagging (more than three-fourths of dealers say equity-oriented hedge-fund leverage is above the decade midpoint) |
| Credit Stress (HY OAS 3.24% Yellow; CCC 12.15%; IG 0.86%) | Index credit has started to leak, still not broad | Dysfunction in their sense is a Treasury-market event — MOVE, on-the-run premium, futures basis, OIS–Treasury — not a high-yield event. Tight IG does not contradict a fatter sovereign-liquidity tail |
| VIX 15.31, contango, Green | Equity implied vol is calm | MCI loads on MOVE and on basis dislocations, which can gap while equity vol stays in contango. A green VIX is not a clean bill of health for the collateral market |
| CAPE 41.07 / Buffett ~234%, both Dark Red | Extreme starting valuations for equities | Separates the equity-valuation problem from the fiscal-financial one. The crash ingredients can be an equity-collateral break (last week) *or* a sovereign-liquidity break that reprices the funding of that equity leverage. The bulletin dates neither |
| Deleveraging (Yellow; August debt rose after July’s flush) | No confirmed forced-selling regime in customer margin | Names the forced-selling regime that would not show up in FINRA first: repo-funded basis books and liability-driven gilt/Treasury sales. October 2022 is in their MCI as a two-standard-deviation event without a classic equity-margin cascade |

Practical watch-items the bulletin implies that the dashboard does not yet score:

1. **MCI components, not just SOFR.** On-the-run premium, Treasury futures basis, and MOVE versus VIX. A basis widening with SOFR still inside the Standing Repo Facility corridor is the early print their model is built on.
2. **Debt-to-GDP tercile as a regime variable.** The 3% versus 0.02% gap is a stock effect. It will not flash on a Friday SOFR print. It changes how much weight to put on an amber funding gauge.
3. **NBFI share by type.** Their regression footprint is funds, pensions, and insurers. The missing series is hedge-fund Treasury repo and cash–futures. Track that separately; do not treat the bulletin’s 1.5% as the whole non-bank tail.
4. **The feedback, not the level.** The risk they want scored is a yield jump that forces non-bank sales that worsen the fiscal premium that caused the jump. A calm week does not retire that loop.
5. **Do not wait for HY OAS or VIX.** In this model the first dysfunction print is a government-bond liquidity indicator, which can arrive while IG is at 0.86% and VIX is in contango.

---

## Honorable mention (case study, not the mechanism piece)

**Maureen Farrell, “Troubles at Situational Awareness Point to Record Stock Market Leverage,”** *The New York Times*, September 30, 2026  
https://www.nytimes.com/2026/09/30/business/situational-awareness-stock-market-leverage.html

Reporting, not an essay. Useful as the week’s concrete failure of the equity-margin structure from September 27: a one-way AI book, prime brokers including Goldman Sachs and Bank of America lending tens of billions, leverage requests from 4x toward 10x, then a forced sale of about $20 billion of stock to Citadel at a discount. Treasury data in the piece put hedge-fund borrowing from banks near $3.7 trillion at midyear, more than triple the pandemic starting point. Read it as a dealer-intermediated case, not as a replacement for the distribution in the bulletin.

---

## One-line takeaway for the project

The Friday gauges already say Treasury repo is orderly and equity vol is calm. Drehmann and Zhu’s addition is that this is the good tail of a distribution that high debt and a large non-bank footprint have widened. Score the next three months on basis, on-the-run premium, and MOVE — not on whether SOFR seized this week.
