# Data Confidence Audit

Audit date: 10 June 2026

## Verdict

Confidence target: 95% defensible as a source-backed modeled dataset.

This target is met after the June 2026 audit because the public-facing dataset no longer presents weakly sourced point claims as hard facts. It separates credible source anchors from modeled estimates.

## What Is 95% Defensible

- The project uses credible public institutions for its source base: NSO/MoSPI PLFS, DGE/MoLE NCO-2015, ILO GenAI occupational exposure research, WEF Future of Jobs, ILO India Employment Report, RBI, NASSCOM, and McKinsey.
- The treemap occupation labels use NCO-style two-digit occupation groupings, with simplified display labels for student-readable exploration.
- The AI exposure ranking is directionally defensible: clerical, customer-service, ICT, business-administration, and routine document/data occupations are high exposure; agriculture, care, cleaning, construction, and other physical/informal occupations are lower exposure.
- The overall workforce anchor remains internally consistent at 5,630 lakhs across 40 visible occupation rows.

## What Is Modeled

- Worker counts by two-digit group are modeled from public labour-market anchors and occupational distributions.
- Median pay values are workforce-weighted estimates, not official salary figures for formal-sector employees.
- Outlook percentages are directional five-year bands, not measured forecasts.
- Education levels are typical-entry proxies and should be read comparatively.

## Changes Made For Confidence

- Changed visible labels from exact language to estimated/directional language.
- Removed weak commercial/private-source names from the public page.
- Replaced specific unsupported tooltip claims with source-backed occupational exposure explanations.
- Added a row-level `confidence_basis` field in the embedded dataset.
- Added direct links to primary/public sources in the footer and methodology.

## Remaining Risk

The dataset still cannot honestly claim 95% row-level numeric precision without PLFS microdata extraction and a reproducible NCO two-digit allocation workbook. The current version is strong enough for a public explanatory dashboard, portfolio project, and discussion tool, but not for policy-grade statistical publication.
