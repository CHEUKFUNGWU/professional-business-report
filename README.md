# Professional Business Report

A portable Agent Skill for turning business questions, datasets, and source material into evidence-led reports that support a decision.

The skill combines two complementary research traditions:

- PwC-style problem framing, mixed-method research, value-chain analysis, and action planning
- Goldman Sachs-style baseline comparison, driver decomposition, scenario analysis, and explicit invalidation conditions

It borrows analytical discipline, not brand identity. This project is independent and is not affiliated with, endorsed by, or produced by PwC, Strategy&, or Goldman Sachs.

## What it helps with

The skill can plan, analyse, draft, and review:

- data-analysis reports
- risk-oriented financial statement analysis
- full-year industry performance from representative company filings
- business performance diagnostics
- strategy and transformation reports
- industry and market studies
- business outlooks
- business cases
- executive briefings
- implementation and progress reviews

It adapts its method to the assignment. A university data report will emphasise reproducibility, method justification, and rubric compliance. A strategy paper will emphasise choices and trade-offs. An outlook will emphasise drivers, scenarios, and what would change the forecast.

The financial statement mode takes a different route from standard ratio analysis. It starts with risks disclosed in the annual report and notes, then tests each risk against the company's business model, operating indicators, financial accounts, cash flow, mitigation, and capacity to absorb a shock.

```text
disclosed risk
  -> business exposure
  -> operating mechanism
  -> leading indicator
  -> financial account
  -> cash and liquidity effect
  -> mitigation
  -> residual risk
```

## Core method

```text
decision question
  -> baseline
  -> evidence
  -> drivers
  -> finding
  -> scenario
  -> implication
  -> choice
  -> action
  -> monitoring
```

The skill requires claims to trace back to cited evidence or reproducible calculations. It separates observations, interpretations, forecasts, and recommendations. It also checks definitions, samples, denominators, units, assumptions, sensitivities, and causal language.

## Install across agent harnesses

The repository follows the standard `SKILL.md` format and is recognised by the open `skills` CLI. You need Node.js and `npx`.

Run the interactive installer and choose any detected agents:

```bash
npx skills@latest add CHEUKFUNGWU/professional-business-report
```

Install globally for selected harnesses without prompts:

```bash
npx skills@latest add CHEUKFUNGWU/professional-business-report \
  --skill professional-business-report \
  --agent claude-code cursor codex \
  --global \
  --yes
```

Install globally for every supported harness detected on the machine:

```bash
npx skills@latest add CHEUKFUNGWU/professional-business-report \
  --skill professional-business-report \
  --agent '*' \
  --global \
  --yes
```

The installer supports many agents and writes or links the Skill to the correct directory for each selected harness. Omit `--global` to install it only in the current project.

To disable anonymous installer telemetry:

```bash
DISABLE_TELEMETRY=1 npx skills@latest add \
  CHEUKFUNGWU/professional-business-report
```

### Manual installation

You can also clone the repository into the skills directory used by your agent. For Codex:

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/CHEUKFUNGWU/professional-business-report.git \
  ~/.codex/skills/professional-business-report
```

Restart or reload your agent session if the skill does not appear immediately.

### Update

Update installations managed by the `skills` CLI:

```bash
npx skills@latest update professional-business-report --global
```

Update a manually cloned Codex installation:

```bash
git -C ~/.codex/skills/professional-business-report pull
```

## Use

Invoke the skill as `$professional-business-report` and provide the decision, audience, evidence, and required output.

### General business report

```text
Use $professional-business-report to analyse the attached customer-retention data
and write a report for the executive team.

Identify where churn is concentrated, test the leading explanations, quantify the
main drivers, and recommend actions. Use only results supported by the supplied
data. Deliver the report in English with an executive summary, findings, actions,
limitations, and source notes.
```

### Course data-analysis report

```text
Use $professional-business-report to write a 1,200-1,500 word data-analysis report
from the assignment brief, dataset, and executed Jupyter notebook.

Treat the rubric and required headings as the governing structure. Every number
must match the notebook output. Explain the descriptive statistics, overall
correlations, and group-based correlations. Distinguish correlation from causation,
justify the methods used, and state the limitations. Write the final report in
academic English.
```

### Strategy report

```text
Use $professional-business-report to assess whether our company should enter the
Australian home-energy-management market.

Define the market, estimate the opportunity with transparent assumptions, compare
the strategic options, identify the capabilities and risks, and recommend a path.
Separate evidence, estimates, and judgement. Include base and downside scenarios
because regulation and adoption are uncertain.
```

### Business outlook

```text
Use $professional-business-report to prepare a 2027 outlook for the regional
construction market.

State the baseline forecast, compare it with the current business plan, break the
forecast into demand, cost, labour, and policy drivers, and show what is temporary
versus structural. Include scenarios, leading indicators, and conditions that
would invalidate the conclusion.
```

### Risk-oriented financial statement analysis

```text
Use $professional-business-report to analyse the attached annual reports from a
risk perspective.

Begin with the principal risks, risk factors, Financial Risk Management note,
sensitivity tables, credit concentrations, liquidity maturity analysis, covenants,
and capital-management disclosures. Link each material risk to the affected
business segments, operating indicators, financial statement accounts, and cash
flow. Test whether the risk is already visible in the data, assess management's
mitigation and remaining exposure, and perform reverse stress tests where the
disclosures support them. Do not organise the report as a generic ratio review and
do not infer fraud or provide an investment recommendation.
```

### Full-year industry performance from company filings

```text
Use $professional-business-report to analyse the global airline industry's
performance during the latest fully reported financial year.

Select 5-10 representative listed airlines using documented criteria that cover
different scales, regions, and business models. Use annual reports and regulatory
filings as the primary sources. Normalise fiscal periods, currencies, accounting
definitions, acquisitions, and alternative performance measures before comparing.

Assess revenue growth, volume and price/mix, margins, cash generation, working
capital, capital expenditure, balance-sheet capacity, and common risk disclosures.
Show the sample median, a compatible scale-weighted result, dispersion, and the
number of companies moving in the same direction. Explain whether performance was
broad or driven by a few firms. Distinguish evidence from the representative
company sample from complete industry statistics.
```

## Repository structure

```text
professional-business-report/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── analytical-methods.md
    ├── evidence-and-research.md
    ├── financial-statement-analysis.md
    ├── industry-performance-from-filings.md
    ├── method-synthesis.md
    ├── quality-gates.md
    ├── report-modes.md
    └── writing-and-exhibits.md
```

`SKILL.md` contains the portable workflow and routing rules. Compatible agents load the reference files only when the current report needs them. `agents/openai.yaml` provides optional Codex interface metadata and does not change the core Skill instructions.

## Design principles

- The user's brief, rubric, and required format take priority over the default structure.
- No statistics, quotations, sources, or findings may be invented.
- A forecast is optional unless the decision requires one.
- A recommendation must follow from the evidence.
- Correlation does not establish causation.
- Named frameworks must clarify the decision, not decorate the report.
- Plain language beats consulting jargon.
- The final report should say what evidence or event would change its conclusion.

## Language

The skill instructions are written in English for portability across agent harnesses. Reports can be produced in any language requested in the prompt.

```text
Use $professional-business-report to produce the final report in Chinese.
```

## Scope and limitations

This skill provides a research and writing method. It does not supply proprietary data, replace subject-matter review, or guarantee that incomplete evidence can support a firm conclusion. It must not claim institutional authorship or provide personalised investment advice.
