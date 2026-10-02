# NYC311 Power BI Operations Case Study

Portfolio Slot 04 · Business Intelligence / Power BI

A reproducible dashboard case study using a pinned NYC Open Data 311 cohort: 287,186 service requests created in January 2024. It demonstrates a request-grain fact table, Agency/Problem/Borough/Channel/Status/Date dimensions, Power Query import and type correction, explicit DAX measures, and clear timing eligibility.

## Verified findings

- 287,186 requests; 285,297 are marked Closed.
- 284,017 rows qualify for valid, nonnegative recorded closure timing.
- Median recorded interval: 19.10 hours; P90: 668.55 hours.
- 152,789 timing-eligible requests (53.80%) are under 24 hours.

The measures are descriptive administrative records, not SLA compliance or proof of resolution quality.

## Reproducible package

Download `nyc311-powerbi-dashboard.zip` above. It contains the source extract and manifest, preparation and independent validation code, prepared fact and dimensions, verified results, M and DAX starter materials, interactive preview, limitations, and interview brief. Run `python prepare_powerbi.py`, `python validate.py results/`, and `node tests/test_dashboard.js` from the extracted project directory.

Native Power BI Desktop execution and Power BI Service publication are not verified in this environment. The live portfolio provides a clearly labeled web preview.

Portfolio: https://justin-pierite-data-work.kvngisaa.chatgpt.site/
