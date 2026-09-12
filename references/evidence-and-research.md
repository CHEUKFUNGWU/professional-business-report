# Evidence and research

## Start with an evidence plan

For each report question, record:

| Field | Required content |
|---|---|
| Decision use | The decision this answer informs |
| Initial hypothesis | The expected answer |
| Alternative | A credible competing explanation |
| Required evidence | The minimum evidence needed |
| Method | Dataset, desk research, survey, interview, case, or model |
| Comparison | Time, target, peer, segment, geography, or scenario |
| Limitation | Expected bias or blind spot |

Search for claims and tests, not simply for the broad topic.

## Source order

Prefer:

1. official statistics, laws, regulators, standards, and public datasets;
2. audited filings, company disclosures, product documentation, and first-party records;
3. peer-reviewed or methodologically transparent research;
4. reputable industry datasets and specialist research;
5. original surveys and interviews;
6. reputable reporting for recent events and context.

Use summaries to locate original sources. Record publication date and underlying data period separately. Multiple pages repeating one press release form one evidence chain.

## Evidence ledger

Maintain this while working:

`claim_id | claim | evidence_class | source | URL/file | publication_date | data_period | geography | population/base | definition | method | limitation | confidence | used_in`

Set confidence from source authority, directness, recency, sample quality, method transparency, and corroboration. Use high, medium, or low with a short reason.

## Structured data

Before analysis, document:

- row grain and unit of analysis;
- fields, types, units, categories, and target variables;
- missingness, duplicates, impossible values, outliers, and inconsistent labels;
- transformations, filters, exclusions, joins, and derived variables;
- whether the sample represents the population of interest;
- analysis code and outputs required for reproducibility.

Every number in the report must trace to a cited source or a reproducible calculation. If a notebook or workbook is the analytical record, ensure the report agrees with its final executed outputs.

## Surveys

Disclose field dates, collection mode, target population, achieved sample, geography, quotas, weighting, exclusions, missing-data handling, exact question wording, response scale, base size, and whether respondents could select multiple answers.

Compare subgroups only when base sizes support the claim. If no statistical test was run, write "directionally higher" rather than "significantly higher." Do not present small or unstable cuts as firm findings.

## Interviews

Use interviews to explain mechanisms, barriers, decision logic, and emerging practices. Recruit across roles, performance levels, and the value chain. Record attribution and consent. Code notes into themes, counter-themes, mechanisms, cases, and quotations.

Interview frequency is not population prevalence. Use quotations for explanation or texture, not as proof of scale.

## Cases

Choose cases because they test a proposition. Capture the starting state, intervention, mechanism, result, time period, context, and transferability. Distinguish announced plans from implemented outcomes.

## Triangulation

Strong business findings often combine different evidence types:

- data establishes scale and direction;
- survey results establish reported behaviour or sentiment;
- interviews explain why;
- cases show how a mechanism works;
- models estimate future or financial impact.

Do not require two sources for every minor fact. Seek independent support for conclusions that carry the recommendation.

## Research stopping rule

Stop when every critical question has a defensible answer, key definitions are stable, the strongest alternative explanation has been tested, major evidence conflicts are understood, and further searching is unlikely to change the decision. Report unresolved gaps.
