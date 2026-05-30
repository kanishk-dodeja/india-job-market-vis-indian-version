# India Job Market Visualizer — Data Methodology & Sources

**Dataset version:** May 2026 rebuild  
**Total workforce represented:** 5,630 lakhs (563 million), per PLFS 2022-23

---

## 1. Primary Sources

### Worker Counts
- **PLFS 2022-23** (NSO/MoSPI): Periodic Labour Force Survey, Annual Report 2022-23. Used for major group totals and sub-group distribution ratios. Grand total anchored to 5,630 lakhs (563M) employed workforce.
- **ILO India Employment Report 2024**: Cross-check on sector shares, agricultural employment reversal post-COVID.
- **NASSCOM FY25 Annual Report**: IT-BPM sector headcount (5.8 million).
- **Economic Survey 2025-26**: PLI scheme job creation (12.6 lakh jobs by September 2025).

### Wages
- **PLFS earnings tables (2022-23)**: Usual principal status earnings by occupation group.
- **Labour Bureau Wage Rate Survey**: Agricultural and construction daily wages.
- **RBI Annual Report 2022-23**: Agricultural daily wage (Rs 323/day national average, year ended March 2022).
- **NASSCOM / Talent500 Salary Benchmarks**: IT sector median wages (Rs 6.5-7.5 lakh for ICT professionals).
- **PayScale India**: Nursing (Rs 3 lakh median), allied health roles.
- **FR8.in Truck Driver Salary Survey 2023**: Rs 3-3.6 lakh annually for truck drivers.
- **Glassdoor India / Indeed India**: Manager salary bands (Rs 13.6-21 lakh for administrative managers).
- **CollegeSearch / Shiksha 2023**: Teacher salary data (Rs 3.5-4.5 lakh government + private blended).
- **Flowace.ai BPO Salary Report**: Entry-level clerk wages (Rs 2.1-2.6 lakh annually).
- **MGNREGA official data**: Subsistence agricultural worker wage floor (Rs 225-374/day, 100 guaranteed days).
- **Central Government Minimum Wage Schedule 2022-23**: Construction skilled trades (Rs 600-900/day).

### AI Exposure Scores (1-10 scale)
- **ILO Working Paper 96** (Gmyrek, Berg, Bescond, 2023): "Generative AI and Jobs: A Global Analysis of Potential Effects by Occupation and Sector." Primary framework for occupation-level task exposure assessment.
- **ILO Working Paper 140**: Finance and business occupations exposure detail.
- **WEF Future of Jobs Report 2023**: Occupation displacement/creation projections, top 26 million at-risk roles by 2027.
- **Task-based scoring methodology**: Each occupation scored 1-10 on AI exposure using the ILO framework:
  - 1-2: Primarily physical, outdoor, or informal — negligible AI applicability
  - 3-4: Physical roles with some cognitive tasks; AI augments but cannot replace
  - 5-6: Mixed cognitive/physical; AI handles a meaningful portion of tasks
  - 7-8: Predominantly cognitive, routine-heavy; AI displaces significant task share
  - 9-10: Near-fully cognitive, routine, and text/data-based; AI handles majority of core tasks
- **India-specific calibration**: Scores adjusted downward from global baselines where (a) labour costs make automation economically non-viable, (b) informal employment context removes employer capacity to deploy AI tools, or (c) India-specific infrastructure gaps (no AV regulatory framework, rural digital infrastructure absent) delay realistic deployment.

### Outlook Percentages
- **ILO India Employment Report 2024**: Sector-level employment projections through 2030.
- **WEF Future of Jobs 2023**: Net job creation/destruction ratios by occupation cluster.
- **NASSCOM FY24 / FY25 data**: IT-BPM sector net hiring collapse (FY23: 270,000 net hires; FY24: 60,000).
- **Jefferies India BPO Research Note 2024**: 50% BPO revenue risk from AI over 5 years.
- **PM Gati Shakti / NIP data**: Construction and infrastructure employment projections (45 crore man-days).
- **PLI Scheme tracking (MoCI)**: Manufacturing employment (12.6 lakh jobs, September 2025).
- **Lancet (peer-reviewed)**: India nursing shortfall of 1.98 million by 2030.

---

## 2. Key Data Decisions

### Armed Forces (NCO Group 0) Removed
The NCO-2015 Group 0 (Armed Forces) is excluded from the visualizer. PLFS does not classify armed forces workers within the standard 9-group NCO framework for civilian labour market analysis. The 5,630 lakh total is the civilian employed workforce.

### Agriculture Worker Counts (Revised)
Previous dataset showed NCO 61 at 1,173 lakhs — significantly overstated relative to PLFS 2022-23 sub-major group data. Revised to 720 lakhs (market-oriented skilled agricultural workers), 174 lakhs (forestry/fishery), 276 lakhs (subsistence) = 1,170 lakhs total for Group 6. This aligns with the PLFS 2022-23 finding that agriculture accounts for ~45.76% of employment across all agricultural NCO codes including Group 9 labourers.

### Clerical Worker Counts (Revised Upward)
Previous dataset showed very low clerical counts (NCO 41: 38 lakhs, NCO 42: 45 lakhs) that understated India's formal BPO and back-office workforce. Revised to 80 and 90 respectively to reflect NASSCOM's documented 2-2.5 million call centre workforce plus broader back-office processing scale.

### Driver Wages (Corrected)
Previous wage of Rs 200,000 for NCO 83 was understated. FR8.in 2023 survey data confirms truck drivers earn Rs 3-3.6 lakh annually. Revised to Rs 300,000.

### ICT Professional Wages (Corrected Downward)
Previous median of Rs 1,100,000 overstated the workforce average by anchoring on senior/specialist salaries. Talent500 and NASSCOM data shows the workforce median is Rs 6.5-7.5 lakh. Revised to Rs 700,000 to represent the full distribution including junior roles.

### AI Exposure for NCO 33 and NCO 44 (Outlook Labels Corrected)
Previous dataset marked NCO 33 (Business/Admin Associate Professionals) outlook as "Slower than average" (-5%) and NCO 44 as "Slower than average" (-8%). Both corrected to "Declining" label to match the negative outlook_pct values — the label was inconsistent with the data.

---

## 3. Data Limitations and Caveats

1. **Informal sector estimation**: 90%+ of India's workforce is informal. PLFS captures employment status but wages for informal workers are self-reported and may understate true earnings due to piece-rate work and seasonal variability.

2. **Sub-major group granularity**: PLFS 2022-23 publicly available data provides major group totals more reliably than sub-major group (2-digit) breakdowns. Sub-major allocations use proportional distribution based on earlier PLFS waves and NSS 68th round ratios.

3. **AI exposure is task-based, not vacancy-based**: Scores represent the theoretical share of work tasks that current LLMs and automation could perform — not observed displacement. Actual displacement lags exposure due to capital investment cycles, regulatory barriers, and India-specific labour cost economics.

4. **Outlook percentages are illustrative growth bands**: The outlook_pct field represents approximate annual net employment change (%), synthesising ILO/WEF projections. They are directional indicators, not point forecasts.

5. **Wage figures are annual median estimates**: Wages represent estimated median annual earnings (including informal piece-rate and agricultural day labour converted to annual equivalent). They do not represent mode or mean, and formal-sector medians will be significantly higher than these workforce-weighted figures.

6. **Currency**: All wages are in nominal INR as of 2022-23. No inflation adjustment applied across sub-groups.
