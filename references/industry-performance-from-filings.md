# Industry performance from company filings

Use this mode when the user wants to understand an industry's performance during a completed financial year. Build a comparable cross-company dataset from 5-10 representative annual reports or regulatory filings. The result is a sample-based industry signal, not a substitute for a complete industry census.

## Fix the boundary and period

Define before searching:

- industry and excluded adjacent activities;
- geography and whether the analysis covers domestic operations or global companies;
- value-chain scope, such as producers, distributors, platforms, or integrated groups;
- completed calendar or fiscal year;
- currency and nominal or constant-price basis;
- performance questions and decision audience.

Use the latest fully reported year, not a mixture of completed annual results and partial current-year results. If fiscal year-ends differ, choose the closest comparable periods and show the exact dates. Do not annualise interim data unless the user requests it and the method can handle seasonality.

## Select a representative sample

Choose 5-10 companies when enough comparable public companies exist. Do not select only the largest firms or the companies with the easiest reports.

Build a coverage matrix:

| Company | Selection role | Scale | Business model | Geography | Value-chain position | Pure-play share | Fiscal year-end | Accounting basis | Inclusion reason |
|---|---|---|---|---|---|---|---|---|---|

Balance the sample across factors that could produce different outcomes:

- leaders, challengers, and specialised operators;
- large and mid-sized firms;
- pure plays and integrated groups;
- relevant regions or customer markets;
- premium, mass-market, asset-heavy, asset-light, direct, and intermediary models where applicable;
- upstream, midstream, and downstream positions when the industry spans a value chain.

Document exclusions, unavailable filings, failed comparability tests, and survivorship or public-company bias. Use fewer than five only when the public universe is genuinely small, and state how this weakens the conclusion.

If authoritative industry revenue or volume totals exist, estimate sample coverage. Revenue coverage alone does not prove representativeness when the firms have different product, geographic, or value-chain mixes.

## Use primary company sources

For each company, prefer:

1. audited annual report and notes;
2. regulatory filing, such as a 10-K or 20-F;
3. full-year results release;
4. investor presentation and earnings transcript for operating explanation;
5. reputable secondary reporting only for context or unresolved events.

Record document URL, publication date, reporting period, page or note, currency, scale, accounting standard, and whether each metric is reported or calculated.

## Build a common extraction template

Extract only measures relevant across the sample. Candidate fields include:

### Scale and growth

- revenue and reported growth;
- organic or constant-currency growth;
- volume, price/mix, customer, subscriber, store, order, shipment, or utilisation growth;
- acquisitions, disposals, and currency contribution;
- orders, bookings, backlog, or recurring revenue where meaningful.

### Profitability

- gross profit and margin;
- EBITDA or another clearly defined operating measure;
- operating profit and margin;
- major cost drivers and restructuring or impairment items;
- segment profit using compatible definitions.

### Cash and investment

- operating cash flow;
- capital expenditure, with maintenance and growth split when disclosed;
- free cash flow using a stated common definition;
- working-capital movement and relevant days metrics;
- research, technology, capacity, or expansion investment.

### Financial capacity

- cash and committed liquidity;
- gross and net debt under stated definitions;
- leverage and interest coverage;
- debt maturities, covenants, and major commitments;
- dividends, buybacks, acquisitions, and debt repayment.

### Risk and outlook signals

- principal risks and changes from the prior year;
- credit, liquidity, rate, currency, commodity, operational, regulatory, and climate exposure where relevant;
- mitigation and sensitivity disclosures;
- management guidance or leading indicators for context, kept separate from the completed-year assessment.

Preserve the source wording for metric definitions. Do not assume that two companies' "adjusted EBITDA," "free cash flow," or "organic growth" are comparable.

## Normalise without erasing differences

Create both a reported dataset and a comparable dataset. Reconcile:

- fiscal year-end and number of weeks;
- presentation currency and exchange-rate method;
- IFRS, US GAAP, and local accounting differences;
- continuing operations and consolidation scope;
- leases, pensions, financial subsidiaries, and joint ventures;
- acquisitions, disposals, and discontinued operations;
- reported, organic, constant-currency, and pro-forma growth;
- management-defined measures and unusual items.

Keep metrics separate when no defensible reconciliation exists. Comparability is more important than filling every cell.

Do not add segment revenue across integrated companies if transactions inside the industry would be double counted. Do not convert currencies when only growth rates or margins are needed. State the exchange rate and date when conversion serves a real analytical purpose.

## Aggregate the evidence carefully

Use several views because no single average represents the industry:

- **Median:** the typical sampled company and protection against outliers.
- **Scale-weighted aggregate:** the performance of sampled economic scale. Calculate from compatible underlying totals.
- **Range or interquartile range:** dispersion and business-model differences.
- **Breadth:** number or share of companies showing growth, margin expansion, positive free cash flow, or another direction of change.
- **Contribution:** companies, segments, or drivers responsible for most of the sample's aggregate movement.

For a weighted margin, use:

`sample margin = sum(compatible profit numerator) / sum(compatible revenue denominator)`

Do not take a revenue-weighted average of incompatible margin definitions. Do not let one very large company define both the aggregate result and the claim about breadth.

## Analyse the industry signal

### Demand and growth

Separate volume, price/mix, currency, and portfolio change. Determine whether growth was broad or concentrated. Compare customer, product, geography, and channel indicators where available.

### Profit and cost

Explain margin movement through operating leverage, pricing, mix, input costs, labour, productivity, capacity utilisation, depreciation, and unusual items. Distinguish common industry pressure from company-specific execution.

### Cash and investment cycle

Compare earnings with operating cash flow, working capital, and capital expenditure. Determine whether companies expanded capacity, defended liquidity, harvested cash, or reduced investment. A stronger free cash flow year may come from lower growth investment or a one-time working-capital release.

### Divergence

Identify which company characteristics explain different outcomes. Test business model, scale, geography, customer mix, value-chain position, pricing power, balance-sheet capacity, and management execution. Do not label every outperformer a better company when its exposure was simply more favourable.

### Cross-company risk signals

Apply [financial-statement-analysis.md](financial-statement-analysis.md) to risks shared across the sample. Compare disclosed exposure, operating evidence, financial impact, mitigation, and headroom. Distinguish a widely disclosed risk from a widely manifested risk.

## Separate industry evidence from sample evidence

Use precise language:

- "Seven of the nine sampled companies reported lower volumes."
- "The sample median operating margin fell 1.2 percentage points."
- "The revenue-weighted sample grew 4.1%, largely because of two firms."

Do not write "the industry declined 8%" unless an authoritative industry total supports that number. Triangulate the company sample with official production, sales, trade, employment, capacity, price, or market-size data when available.

## Default report structure

1. Industry definition, completed year, sample design, and coverage.
2. Executive assessment of scale, breadth, dispersion, and confidence.
3. Demand and revenue, separated into volume, price/mix, currency, and portfolio effects.
4. Profitability and shared cost drivers.
5. Cash conversion, working capital, capital expenditure, and financial capacity.
6. Differences by business model, segment, geography, and value-chain position.
7. Common disclosed risks and evidence of financial manifestation.
8. Conclusions about the completed year, limitations, and indicators for the next period.
9. Appendix with company-source matrix, definitions, reconciliations, and calculations.

## Completion standard

The analysis is complete when the reader can see why each company was selected, which measures are comparable, whether the headline result is broad or concentrated, what drove common performance, why firms diverged, how disclosed risks appeared in the accounts, and where the sample cannot represent the full industry.
