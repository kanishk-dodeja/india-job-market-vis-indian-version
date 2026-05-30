# AI Exposure Scoring Notes — India Job Market Visualizer

## Methodology

AI exposure scores (1.0–10.0) represent the estimated degree to which a sub-major occupational group's tasks can be augmented or displaced by current and near-term generative AI systems (LLMs, computer vision, robotic process automation, agentic AI). Scores were assigned using a triangulation framework across three primary research streams:

1. **Task decomposition analysis**: Each occupation's task bundle (from NCO-2015 task descriptions and O*NET crosswalks) was evaluated for the proportion of tasks classified as "routine cognitive," "non-routine cognitive," or "physical/manual." Routine cognitive tasks (data entry, document processing, standard analysis) receive higher exposure scores.

2. **Research-backed sector findings**: Published ILO, WEF, and Oxford research provided quantitative exposure estimates for specific occupational clusters. Where direct India-specific data existed (ILO Working Paper 96 on India, ILO India Employment Report 2024), those findings were prioritized over global averages.

3. **India-specific structural adjustments**: Scores were moderated for India's unique context — informal economy prevalence (90%+ of workers), low wage floors (reducing automation ROI), digital infrastructure gaps in rural and semi-urban areas, and sector-specific regulatory environments.

**Score anchors:**
- 1.0–2.0: Near-zero AI relevance (subsistence agriculture, street vendors, sanitation workers)
- 2.5–3.5: Low exposure — physical presence essential, AI augments minimally (construction, caregiving, protective services)
- 4.0–5.5: Moderate exposure — AI handles portions of the task bundle but human judgment or physical work is central (drivers, plant operators, craft trades)
- 6.0–7.5: High exposure — AI handles significant task share; job content shifting materially (ICT technicians, business professionals, engineers)
- 8.0–10.0: Critical exposure — AI displaces the primary task bundle; headcount contraction underway or imminent (clerical workers, data entry, BPO call centre agents)

---

## Score Ranges by Major Group

| Major Group | NCO Code | Sub-majors | Score Range | Rationale |
|---|---|---|---|---|
| Armed Forces | 0 | 01, 02, 03 | 2.5 – 3.5 | Classified operational contexts, physical readiness requirements, and nascent defence AI adoption insulate this group |
| Managers | 1 | 11–14 | 4.5 – 6.5 | Administrative and commercial management faces significant LLM augmentation; operational leadership retains human primacy |
| Professionals | 2 | 21–26 | 3.5 – 8.5 | Wide range: ICT professionals (8.5) at peak exposure; health professionals (3.5) insulated by physical care and India's doctor shortage |
| Technicians and Associate Professionals | 3 | 31–35 | 3.5 – 7.5 | BPO-adjacent business associate roles (7.5) and ICT technicians (7.5) highly exposed; healthcare associates (3.5) resilient |
| Clerical Support Workers | 4 | 41–44 | 8.0 – 9.0 | Highest-exposure group per ILO WP96; general clerks and numerical recorders face near-critical displacement risk |
| Services and Sales Workers | 5 | 51–54 | 2.5 – 5.5 | Personal care (2.5) and protective services (3.0) resilient; formal retail sales (5.5) faces AI-driven inventory/recommendation pressure |
| Skilled Agricultural, Forestry and Fishery Workers | 6 | 61–63 | 1.5 – 2.5 | Lowest-exposure professional group; subsistence farmers (1.5) structurally immune to AI deployment |
| Craft and Related Trades Workers | 7 | 71–75 | 2.5 – 4.5 | Physical trades insulated by unstructured environments and India's low labour costs; handicraft GI-tag premium protects artisans |
| Plant and Machine Operators and Assemblers | 8 | 81–83 | 4.0 – 5.5 | Medium exposure; India's low assembly wages give a 5–10 year buffer vs developed economy automation timelines |
| Elementary Occupations | 9 | 91–96 | 1.5 – 2.5 | Very low; physical variability, informal employment, and wage floors below automation ROI threshold |

---

## Primary Sources

**ILO Research (International Labour Organization)**
- ILO Working Paper 96: "Generative AI and Jobs: A Global Analysis of Potential Effects on Job Quantity and Quality" (2023) — Provides occupation-level exposure estimates for developing economies including India.
- ILO India Employment Report 2024: "Youth Employment Trends and Pathways" — India-specific sector analysis and automation risk quantification.
- ILO Working Paper 140: "The Impact of Artificial Intelligence on Employment: A Global Perspective" — Identifies clerical occupations as highest-exposure cluster globally.

**WEF Research**
- World Economic Forum Future of Jobs Report 2023 — Provides 26M job displacement estimates by 2027 for clerical and administrative roles; identifies fast-growing AI/ML roles offsetting losses.

**Oxford / ILO Research**
- Banga & te Velde (ODI/ILO), "Preparing for the Digital Economy" — Automation susceptibility estimates for South Asian occupational clusters cross-referenced with NCO-2015 codes.
- Frey & Osborne (2013/2017 updates) — Foundational occupation-level automation probability estimates, adapted for India's task distribution and wage context.

**McKinsey Global Institute**
- McKinsey Global Institute India 2023: "India's Turning Point" and "Generative AI: The Next Productivity Frontier" — Sector-level productivity impact and workforce transformation projections for India's IT, BFSI, and manufacturing sectors.

**India Government Data**
- PLFS 2022-23 (Periodic Labour Force Survey, NSO/MoSPI) — Primary source for workers_lakhs estimates and employment structure by NCO major group.
- NCO-2015 (National Classification of Occupations, MoSPI) — Occupational hierarchy and task descriptions used for group-level exposure analysis.

---

*Scoring last reviewed: May 2026. Scores should be reassessed annually as AI capability and adoption evolve.*
