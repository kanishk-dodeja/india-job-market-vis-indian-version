# India Job Market Visualizer - Data Methodology and Sources

Dataset version: June 2026 confidence-audited copy

This visualizer is a modeled dashboard, not an official statistical release. It combines public Indian labour-market statistics with occupation-level AI exposure research to make the India job-market picture easier to explore.

## Confidence Standard

The dataset is intended to be 95% defensible as a source-backed model, not 95% precise as a row-level official dataset. That means:

- High confidence: source choice, occupation taxonomy, overall labour-market anchor, relative AI exposure bands, and the distinction between measured data and modeled estimates.
- Medium-high confidence: directional comparisons across occupations, such as clerical work being more exposed than agricultural or care work.
- Bounded confidence: exact two-digit worker counts, wage point estimates, and five-year outlook percentages. These are modeled values used for visualization and should be read as approximate.

To preserve that confidence standard, the public page labels worker counts, wages, and outlook as estimated or directional, and tooltip text avoids unsupported company-specific or private-source claims.

## Credible Source Base

### Employment Counts and Occupation Taxonomy

- Periodic Labour Force Survey (PLFS) Annual Report 2022-23, National Statistical Office, Ministry of Statistics and Programme Implementation: https://mospi.gov.in/sites/default/files/publication_reports/AR_PLFS_2022_23N.pdf
- National Classification of Occupations (NCO-2015), Directorate General of Employment, Ministry of Labour and Employment: https://dge.gov.in/dge/index.php/nco-2015
- India Employment Report 2024, Institute for Human Development and International Labour Organization: https://www.ilo.org/publications/india-employment-report-2024-youth-employment-education-and-skills

### AI Exposure Framework

- ILO Working Paper 96, "Generative AI and Jobs: A Global Analysis of Potential Effects on Job Quantity and Quality" (2023): https://www.ilo.org/publications/generative-ai-and-jobs-global-analysis-potential-effects-job-quantity-and
- ILO Working Paper 140, "Generative AI and Jobs: A Refined Global Index of Occupational Exposure" (2025): https://www.ilo.org/publications/generative-ai-and-jobs-refined-global-index-occupational-exposure
- World Economic Forum, "The Future of Jobs Report 2023": https://www.weforum.org/reports/the-future-of-jobs-report-2023/

### Wage and Sector Cross-Checks

- PLFS 2022-23 wage and employment-status tables, NSO/MoSPI: https://mospi.gov.in/sites/default/files/publication_reports/AR_PLFS_2022_23N.pdf
- Reserve Bank of India Annual Report 2022-23: https://rbi.org.in/Scripts/AnnualReportPublications.aspx?year=2023
- NASSCOM Strategic Review 2025 for technology-sector context: https://community.nasscom.in/communities/nasscom-insights/technology-sector-india-strategic-review-2025
- McKinsey future-of-work research for broad automation and labour-demand context: https://www.mckinsey.com/Featured-Insights/McKinsey-Explainers/What-is-the-future-of-work

## Modeling Approach

### Worker Counts

The treemap areas are anchored to PLFS employment data and mapped into NCO-2015 occupation groups. Where public PLFS tables do not expose a clean two-digit NCO split, the dashboard uses proportional allocation from available occupation and sector distributions. Those sub-group counts should be read as approximate estimates.

### AI Exposure

AI exposure is scored on a 1-10 scale:

- 1-2: Primarily physical, outdoor, informal, or highly context-specific work with negligible near-term GenAI applicability.
- 3-4: Physical or interpersonal work where AI can assist but cannot perform the core job.
- 5-6: Mixed cognitive and physical work where AI handles some meaningful tasks.
- 7-8: Predominantly cognitive, routine, text, software, data, or administrative work.
- 9-10: Highly routine clerical, customer-service, or document/data work where current GenAI and workflow automation can handle a large share of tasks.

The scoring is derived from ILO occupational exposure research and adjusted for India-specific adoption constraints: informality, lower labour costs, fragmented employer capacity, rural digital gaps, and the slower deployment path for robotics and autonomous systems.

### Outlook and Pay

Employment outlook and wage fields are directional, not point forecasts. They synthesize PLFS wage/employment tables, ILO India employment analysis, WEF job-transition projections, and sector evidence from RBI, NASSCOM, and McKinsey. Because India's informal workforce is large, wage estimates are workforce-weighted medians and will usually be lower than formal-sector salary benchmarks.

## Key Caveats

- The dashboard is explanatory and comparative. It should not be used as a job-loss forecast.
- AI exposure does not equal displacement. Exposure often means task augmentation, not replacement.
- Sub-major occupation counts are estimates when public data does not provide exact two-digit NCO counts.
- Informal earnings are difficult to estimate and may be under-reported in survey data.
- Some occupation summaries mention examples from companies or sectors to make the risk intuitive; the source base above is the evidence foundation for the dashboard.
- Do not interpret the numeric fields as official point statistics. They are midpoints used to size and color an explanatory visualization.

## Attribution

This hosted copy is based on the public `Kashdodeja/india-job-market-vis` project and keeps the India-focused visualizer concept while tightening the public source references for GitHub Pages publication.
