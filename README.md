# Clinical Trials Dashboard

Interactive analysis of ClinicalTrials.gov Phase II and Phase III interventional studies. The dashboard compares trial status, sponsor-entered early-stop reasons, timeline duration, participant-flow dropout, and countries. Filters let readers compare phases and therapeutic areas.

**Snapshot:** 94,549 unique trial records started from 2010 through November 27, 2026; 26,609 records have usable participant-flow measures. The dashboard is a standalone static page. Open `index.html` locally or view the [GitHub Pages site](https://vaishnavi-sonwane.github.io/clinical-trials-dashboard/) after Pages finishes publishing.

## Key findings

- 13,504 of 55,927 closed records were terminated, suspended, or withdrawn (24.1%).
- Among early-stop records with a reported reason, enrollment/recruitment was the most common specific category (29.7%); 30.9% were grouped as other stated reasons.
- Median start-to-primary-completion intervals were 744 days for Phase II, 604 days for Phase II/III, and 668 days for Phase III.
- Median reported dropout was 10.9% for Phase II and 10.8% for Phase III. Oncology had the highest median across therapeutic areas with at least 10 flow records (22.1%, n=7,556).

See [findings.md](findings.md) for the full descriptive summary.

## Definitions and limitations

- The source is the [ClinicalTrials.gov API v2](https://clinicaltrials.gov/data-api). The site includes interventional trials with study start dates from 2010-01-01 through the snapshot date. Future anticipated starts are excluded.
- The API snapshot does not preserve original planned schedule dates. Start-to-primary-completion duration is a timeline proxy, not a direct measurement of enrollment delay or schedule slippage.
- Dropout is calculated from participant-flow records as (participants started − completed) ÷ started. It is available only where the results module reports both milestones; records with missing counts are excluded.
- Early-stop reasons come from optional sponsor-entered text and are grouped by keywords. Therapeutic areas are assigned from condition keywords to one primary area per record.
- These are descriptive registry patterns and do not establish causation. Registry values may be amended after submission.

## Use

Open `index.html` to explore the dashboard. Choose phase, therapeutic area, status, or start-year cutoff to filter the visuals and record explorer. Use **Export filtered CSV** to save the current record selection.
