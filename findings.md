# Clinical trial delivery and participant flow findings

Snapshot retrieved 2026-11-27 from the ClinicalTrials.gov API v2. The extract contains 94,549 unique interventional Phase II/III study records with start dates from 2010 onward.

## Headline results

- 13,504 of 55,927 closed records are terminated, suspended, or withdrawn (24.1%). This is the registry-record early-stop rate, not a participant-level rate.
- 12,400 early-stop records include sponsor-entered stop-reason text. The most common coded categories are:
  - Other stated reason: 3,836 (30.9% of early-stop records with a stated reason)
  - Enrollment / recruitment: 3,686 (29.7% of early-stop records with a stated reason)
  - Business / strategic: 1,643 (13.2% of early-stop records with a stated reason)
  - Funding / resources: 1,015 (8.2% of early-stop records with a stated reason)
  - Efficacy / futility: 631 (5.1% of early-stop records with a stated reason)
  - Safety / tolerability: 577 (4.7% of early-stop records with a stated reason)
  - COVID-19: 506 (4.1% of early-stop records with a stated reason)
  - Operational: 506 (4.1% of early-stop records with a stated reason)

- Median start-to-primary-completion interval among completed studies with both dates:
  - Phase II: 744 days (n=15,416)
  - Phase II/III: 604 days (n=1,373)
  - Phase III: 668 days (n=8,966)

- Participant-flow results support a trial-level dropout calculation for 26,609 records. Median dropout by phase:
  - Phase II: 10.9% across 16,517 records
  - Phase II/III: 11.8% across 971 records
  - Phase III: 10.8% across 9,121 records

Therapeutic-area medians with at least 10 participant-flow records (equal weighting per trial):

| Therapeutic area | Median dropout | Trials |
|---|---:|---:|
| Oncology | 22.1% | 7,556 |
| Mental health | 17.6% | 732 |
| Reproductive health | 14.3% | 184 |
| Hematology | 14.0% | 408 |
| Gastroenterology | 13.9% | 451 |
| Neurology | 13.8% | 1,067 |
| Dermatology | 13.5% | 455 |
| Immunology & autoimmune | 12.5% | 827 |
| Musculoskeletal | 10.2% | 299 |
| Renal & urology | 9.8% | 361 |

## Phase coverage

| Phase | Trials |
|---|---:|
| Phase II | 60,740 |
| Phase II/III | 5,698 |
| Phase III | 28,111 |

## How to interpret these measures

- The API snapshot does not provide historical baseline schedule dates, so it cannot identify schedule slippage or enrollment delays directly. Start-to-primary-completion is shown only as a timeline proxy.
- Dropout uses the participant-flow module where an overall-study period has STARTED and COMPLETED milestones. The rate is calculated as (started − completed) / started. Records with missing milestone counts are excluded. Counts aggregated across registry groups may not equal unique people in designs with overlapping groups.
- “Why stopped” is optional free text supplied by study submitters. Keyword categories are broad and can misclassify ambiguous text. The stated-reason denominator is only stopped records that contain this text.
- Therapeutic areas are assigned from condition keywords to one primary area per record. Multi-condition studies and unrecognized conditions are imperfectly represented.
- These are descriptive registry patterns. They do not establish why a delay or early stop occurred or support causal claims.

Source: [ClinicalTrials.gov API v2](https://clinicaltrials.gov/data-api). See the interactive dashboard for phase, area, status, year, country, and record-level filtering.
