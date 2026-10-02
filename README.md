# Supplement Label Overlap & Daily Totals

Find duplicate ingredients across supplement labels. A focused MIT-licensed browser tool: **no account, no dependencies and no label uploads**.

**Can supplement labels contain duplicate ingredients?** Yes. Matching label names can overlap. List those overlaps and calculate daily mass totals for verified names with complete quantities.

[Try the task on NutriAudit](https://www.nutriaudit.com/tools/supplement-label-tools?task=duplicate&utm_source=github&utm_medium=referral&utm_campaign=label_overlap&utm_content=readme) · [Examples & FAQ](docs/examples-and-faq.md) · [MIT license](LICENSE)

## Run locally

Requires Python 3 to serve static files. Node.js 22 or 24 is only needed for tests.

```sh
git clone https://github.com/JinHanAI/nutriaudit-label-overlap.git
cd nutriaudit-label-overlap
python3 -m http.server 8080 --bind 127.0.0.1
```

Open http://127.0.0.1:8080/index.html. Select **Load example** or enter your own labels. Label comparison and arithmetic stay in the browser.

## Worked example

200 mg/day calcium from A plus 0.5 g/day from B equals 700 mg/day. This is arithmetic, not a safety threshold.

The sample is synthetic and is not a personal assessment. Changing inputs clears the previous result.

## Included tasks

This project shows only duplicate, daily-total. It reuses the MIT core from [NutriAudit Label Tools](https://github.com/JinHanAI/nutriaudit-label-tools) at commit `ec9615a2212c3cce01c98e2fdf5dbba85dab1f7f`; it is not a new medical algorithm.

## Limits

- A name overlap is not proof of the same chemical form or harmful interaction.
- Verified daily mass arithmetic covers calcium, vitamin C, D2 and D3. Other names can be listed without a numerical total.
- Only mcg/mg/g conversions. IU, %DV and volume are not guessed. Missing amounts stay unknown.
- This cannot assess drug interactions, abnormal lab results, clinical safety or personal suitability.

## Continue with your full supplement stack

The result includes [a NutriAudit stack-audit link](https://www.nutriaudit.com/scan?utm_source=github&utm_medium=referral&utm_campaign=label_overlap&utm_content=result). It transfers **no labels or notes**. Add actual products on the main site; start with the free preview and decide whether to buy the full report. The hosted service is outside this MIT package.

Links have fixed channel tags: `github`, `label_overlap` and the link position. The standalone demo sends no analytics requests. Hosted-site analytics can distinguish project referrals; blocking analytics or losing tags can leave the origin unknown.

## Tests and provenance

```sh
node --test tests/*.test.mjs
```

[Source provenance](provenance.json) · [Attribution links](docs/attribution.md) · [Security](SECURITY.md). Never put private labels, notes or credentials in issues.
