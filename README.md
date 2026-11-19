# Dell Technologies × F5, Inc. — LLM-Driven M&A Analysis

A course project for **AI in Finance** at Duke University. The goal was to test how far large language models can carry a full buy-side M&A analysis, with humans acting as reviewers rather than authors: checking the AI's data, testing whether its numbers make sense, and presenting the results.

The acquirer (Dell Technologies) and the target (F5, Inc.) were assigned by the instructor. The transaction is hypothetical.

## Deliverables

| File | Description |
|---|---|
| [`Deal Research Report.pdf`](Deal%20Research%20Report.pdf) | 15-page research report: company profiles, market sizing, synergies, valuation, financing, stakeholders, risks, and recommendation |
| [`Pitch Book.pptx`](Pitch%20Book.pptx) | 12-slide pitch book summarizing the deal case for an M&A committee |

## Workflow: AI Drafts, Humans Review

**LLMs used:** ChatGPT (OpenAI), Claude (Anthropic), and Gemini (Google).

| Stage | Done by | What it involved |
|---|---|---|
| Research & drafting | LLMs | Company and industry research, TAM sizing, comps and precedent selection, DCF build, synergy estimates, financing analysis, report and slide drafting |
| Data verification | Team | Checking AI-cited figures (10-K / 10-Q data, market sizes, multiples, credit ratings) against original sources |
| Reasonableness checks | Team | Testing assumptions and outputs: premium baseline, synergy sizing vs. F5's cost base, leverage limits, consistency of figures across both documents |
| Reporting | Team | Final edits and presentation of results |

One example of a correction made during review: the first version computed the control premium off F5's post-incident share price (~$296), which was depressed by the October 2025 cyber incident. After instructor feedback, the offer was re-anchored to the **undisturbed pre-incident price (~$343)**, and the offer price, synergy figures, and price ceiling were updated consistently across the report and the pitch book.

## Deal Summary

| Item | Result |
|---|---|
| Recommended offer | **$445 / share** (30% premium to undisturbed price; ~50% to current price) |
| Implied equity value | ~$25.9B |
| DCF standalone value | $384.16 / share (WACC 9.04%, terminal growth 2.5%, SBC added back) |
| Net synergy NPV | $4.5B ($200M/yr cost + $150M/yr revenue, after ~$1.0B integration costs) |
| Max non-destructive price | $461.48 / share (standalone equity + synergy NPV) |
| Consideration | 40% cash/debt (~$10.4B) / 60% Dell stock (~$15.5B), to keep leverage below 2.0x and preserve Dell's BBB+ rating |
| Key risk | October 2025 cyber incident liabilities — addressed via indemnification and escrow |

## Methods

- **Market sizing:** ADC + WAAP + multi-cloud networking, with a 15% overlap adjustment → ~$16B net 2026 TAM
- **Valuation:** trading comparables, precedent transactions (HPE–Juniper as the main benchmark), and a 5-year unlevered DCF
- **Sensitivity analysis:** implied share price across WACC (8.04%–10.04%) and terminal growth (1.5%–3.5%)
- **Synergy analysis:** SG&A rationalization, supply chain savings, and cross-selling into Dell's ISG channel
- **Financing analysis:** all-cash vs. mixed consideration, measured against Dell's credit rating thresholds

## Takeaways

- The LLMs were fast at producing a complete, well-structured first draft across all sections.
- Its main weaknesses were judgment calls a practitioner would catch, such as choosing the right price baseline for a premium, and keeping figures consistent when one number changes.
- Human review was most valuable in source checking and in testing whether each output was reasonable, not in writing.

## Disclaimer

This is an academic exercise. It is not investment advice and does not reflect any actual transaction or the views of Dell Technologies or F5, Inc. Market data is as of early 2026.
