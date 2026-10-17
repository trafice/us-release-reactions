# US economic releases and the market reaction

How the Nasdaq 100 and the S&P 500 moved after every major scheduled US economic release,
2023-08-01 to 2026-10-15: 284 releases, 561 rows (one per release and index).

Source: [tradingcipher.com](https://tradingcipher.com/), where every row has its own page with
the minute-by-minute chart (the `page` column). Updated 2026-10-17.

## Releases
CPI, PPI, Nonfarm Payrolls, JOLTS, the FOMC rate decision, GDP, core PCE (Personal Income and
Outlays) and retail sales. Release dates and times come from the agencies' own calendars
(BLS, BEA, Census Bureau, Federal Reserve).

## Columns
| column | meaning |
|---|---|
| release | short key (cpi, ppi, nfp, jolts, fomc, gdp, core_pce, retail_sales) |
| release_name | full name |
| release_date | date of the release (US Eastern) |
| release_time_et / release_utc | scheduled release time |
| index | Nasdaq 100 or S&P 500 |
| move_5m_pct / move_30m_pct / move_60m_pct | change from the release minute's price to 5, 30 and 60 minutes later, in % |
| range_30m_pct | high minus low over the first 30 minutes, in % of the release price |
| first_5m_held_to_close | Nasdaq 100 only: 1 if the index closed the day (16:00 ET) on the same side of the release price as it was 5 minutes after the release, 0 if not |
| same_minute_as | other measured releases published in the same minute (their effects cannot be separated) |
| page | the release's page on tradingcipher.com |

## Method
One-minute index data, measured from the price at the release minute. Moves are percentages of
that price; raw index levels are not included. The full method is at
https://tradingcipher.com/methodology/.

These are counts of what happened, not forecasts, and nothing here is trading advice.

## Licence
CC BY 4.0: use it for anything, credit "tradingcipher.com" with a link.
