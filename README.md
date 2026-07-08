\# Canadian Trade Vulnerability Dashboard



\## Overview

A sector-level analysis of Canadian export exposure to the United States,

quantifying trade vulnerability by industry and examining the COVID-19 shock

and recovery across key export sectors. Built using Statistics Canada GDP data

and Canadian international merchandise trade statistics.



\## Key Questions

\- Which Canadian industries are most exposed to US trade disruption?

\- How did the COVID-19 shock affect exports across sectors?

\- Which sectors have recovered most strongly relative to 2019 levels?



\## Data Sources

| Source | Description |

|--------|-------------|

| StatCan Table 36-10-0434-01 | GDP at basic prices by industry, monthly, chained 2017 dollars |

| Statistics Canada CIMT | Canadian international merchandise trade by sector, annual |



Downloaded from: https://www150.statcan.gc.ca/t1/tbl1/en/dtbl/36-10-0434-01



\## Key Findings (2024)

| Sector | Export Value ($B) | US Share (%) | COVID Low ($B) | Recovery vs 2019 (%) |

|--------|------------------|--------------|----------------|----------------------|

| Energy | 118.6 | 32.4 | 54.3 | +44.5 |

| Automotive | 78.3 | 21.4 | 49.8 | +11.5 |

| Machinery \& Equipment | 49.1 | 13.4 | 35.6 | +20.3 |

| Agricultural \& Food | 46.2 | 12.6 | 32.1 | +39.2 |

| Industrial Goods | 41.8 | 11.4 | 28.4 | +20.1 |

| Consumer Goods | 18.8 | 5.1 | 13.1 | +32.4 |

| Forestry | 13.1 | 3.6 | 11.4 | +2.3 |



\- Energy is Canada's most trade-vulnerable sector at 32.4% of total US exports

\- Automotive and Energy together account for over 53% of Canadian exports to the US

\- Forestry showed the weakest post-COVID recovery at only +2.3% above 2019 levels

\- Energy recovered strongly (+44.5%) driven by elevated commodity prices post-2021



\## Charts

| File | Description |

|------|-------------|

| 01\_gdp\_by\_industry.png | Canadian GDP by industry 2015–present |

| 02\_exports\_by\_sector.png | Canadian exports to US by sector 2015–2024 |

| 03\_vulnerability\_index.png | Trade vulnerability index by sector (US export share) |

| 04\_export\_recovery.png | Sector export recovery index (2019=100) |



\## Methodology

Trade vulnerability defined as each sector's share of total Canadian goods

exports to the United States. GDP data filtered to seasonally adjusted,

chained 2017 dollar series. Export recovery index calculated as 2024 export

value relative to 2019 pre-pandemic baseline (2019=100).



\## Limitations

\- Export data uses curated annual figures from published StatCan reports;

&#x20; monthly granularity not available at sector level without large file download

\- Vulnerability index measures export concentration only — does not account

&#x20; for domestic market substitution capacity

\- Services exports not included (goods trade only)



\## Tools

Python 3.11 | pandas | matplotlib | seaborn | requests | Jupyter



\## Reproducing This Project

1\. Download Table 36-10-0434-01 from Statistics Canada (link above)

2\. Place CSV in `data/raw/36100434.csv`

3\. Run `notebooks/05\_trade\_vulnerability.ipynb` top to bottom

