# Supplement Label Overlap & Daily Totals: examples and FAQ

## Can supplement labels contain duplicate ingredients?

Yes. Matching label names can overlap. List those overlaps and calculate daily mass totals for verified names with complete quantities.

**Example:** 200 mg/day calcium from A plus 0.5 g/day from B equals 700 mg/day. This is arithmetic, not a safety threshold.

[Run the task](https://www.nutriaudit.com/tools/supplement-label-tools?task=duplicate&utm_source=github&utm_medium=referral&utm_campaign=label_overlap&utm_content=guide). Examples are synthetic; enter actual labels to check your input.

## Does this mean my supplements are safe?

No. This organizes labels and arithmetic. It cannot rule out interactions or determine individual safe doses. Ask a qualified clinician or pharmacist about personal risks.

## What happens to unknown ingredients or quantities?

They stay unknown. Literal names may overlap; unverified names do not receive daily totals. D2 and D3 stay separate. Salt mass is not treated as elemental mass.

## Are labels uploaded?

Not in the local demo. It makes no analytics or upload requests. CSV files and printouts can remain on your device. The hosted NutriAudit service has its own privacy and account rules.

## Can I open the file directly?

Use the local HTTP server in the README; browser ES modules may be blocked on file URLs. No install or account is needed.

## What should I do after the result?

Use the stack-audit link to check your actual supplement stack on NutriAudit. The link carries only fixed tags, not labels or notes. Preview is free; the full report is paid.

## Does a separate repository guarantee search or AI visibility?

No. This is an independently runnable task with citable examples. It shares a MIT core. Publication does not prove indexing, citation, ranking or traffic.

## Which nutrition references inform normalization?

The core links verified names to NIH ODS [calcium](https://ods.od.nih.gov/factsheets/Calcium-HealthProfessional/), [vitamin C](https://ods.od.nih.gov/factsheets/VitaminC-HealthProfessional/) and [vitamin D](https://ods.od.nih.gov/factsheets/VitaminD-HealthProfessional/). These references do not validate a personal result.
