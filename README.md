# Debt Capacity & Credit Structuring Analysis

**Portfolio Project | Leveraged Finance / Acquisition Financing**

Python-based analysis of maximum sustainable leverage, debt service coverage, and covenant design for a mid-market industrial acquisition. Built to demonstrate quantitative credit skills transferable from risk management into investment banking / leveraged finance roles.

## Overview

This project models debt capacity for the acquisition of a stable industrial business under base and downside scenarios. It calculates the maximum leverage that preserves minimum interest coverage, derives Year-1 DSCR with mandatory amortization, and proposes a practical senior secured credit structure with covenants and an excess cash flow sweep.

**Target assumptions**
- LTM EBITDA: USD 80 million
- Year-1 EBITDA: USD 86 million (base) / USD 70 million (downside)
- Maintenance Capex: USD 8 million
- All-in cash interest rate: 7.5%
- Mandatory amortization: 5%

## Key Results

| Metric                        | Base Case    | Downside Case |
|-------------------------------|--------------|---------------|
| Maximum Leverage (on LTM)     | 7.17x        | 7.78x         |
| Year-1 Interest Coverage      | 2.00x        | 1.50x         |
| Year-1 DSCR                   | 1.09x        | 0.80x         |
| Implied Debt Capacity         | ~USD 574m    | ~USD 622m     |

**Proposed structure**
- USD 600 million senior secured term loan (~7.5x LTM EBITDA)
- USD 25 million undrawn revolver
- Covenants: 7.50x max total leverage, 2.00x min interest coverage, 1.15x min DSCR
- Excess cash flow sweep: 50% / 25% / 0% with leverage-based step-downs

At the theoretical maximum leverage, coverage and DSCR are tight. A more conservative 5.0–5.5x structure would produce robust coverage (≥2.8x interest coverage and ≥1.40x DSCR).

## Skills Demonstrated

- Financial modeling and scenario analysis in Python
- Debt capacity and interest coverage calculations
- DSCR and amortization mechanics
- Credit structuring and covenant design
- Identification of red flags for credit committees
- Use of pandas and numpy-financial

## Repository Contents

- `sr_sec_credit.ipynb` — Full interactive notebook with model, optimizer, results, and commentary
- `requirements.txt` — Python dependencies

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook sr_sec_credit.ipynb