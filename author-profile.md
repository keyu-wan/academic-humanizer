# Personal academic writing profile

## Scope and calibration
This personal fork is calibrated to two author-supplied papers on forest change detection and coreset selection for remote-sensing segmentation. These are observed tendencies from a small, coauthored sample, not immutable author preferences. Use this profile by default for the owner's academic manuscripts; a current writing sample, explicit request, or venue constraint takes precedence. For another author, use their samples instead. Proposal-specific preferences have not been established by these paper samples.

## Research context
The author's work connects remote sensing, geospatial machine learning, and forest monitoring. Recurring concerns are geographic heterogeneity, cross-region generalization, dense prediction, class imbalance, and data efficiency. Relevant tasks include bi-temporal forest change detection, forest/tree-cover semantic segmentation, supervised one-shot coreset selection, and foundation-model adaptation.

Keep these distinctions explicit when relevant:
- Forest cover, tree extent, forest loss, and forest degradation depend on the supplied label definition; do not interchange them.
- Change detection compares observations over time; single-date segmentation assigns land-cover labels. Do not merge their datasets or protocols.
- Fewer unique training cases under fixed updates does not establish fewer optimization steps, lower annotation cost, or measured runtime savings.
- Supervised coreset selection from an annotated pool differs from active learning for annotation acquisition.
- Geographic holdout and random splits answer different generalization questions.
- From-scratch training and pretrained fine-tuning may respond differently to subset composition.

## Argument and paragraph structure
Start from a concrete domain constraint and derive the technical problem. Explain why an existing approach misses that constraint before introducing the proposed component. Favor a traceable sequence: observation, diagnostic evidence, design response, controlled comparison, bounded interpretation. This is a useful default for methods papers, not a required outline for every document.

Use paragraphs with a clear opening claim and connected explanatory sentences. Method paragraphs explain what an operation does and why it is needed. Results paragraphs usually identify the setting, compare the relevant methods using supplied values, and interpret the difference within that setting. Preserve useful explanations instead of compressing the text into disconnected short statements.

Related work should distinguish assumptions, selection stages, information sources, or learning regimes and explain their relevance to the current question. Contributions should identify concrete analyses, methodological decisions, or findings.

## Voice and rhythm
Use formal, measured, explanatory English. Preserve first-person plural for author actions and passive voice for procedures when natural. Retain technical terminology consistently rather than seeking decorative synonyms.

The samples use condition-first comparisons (Under..., At..., Compared with...) and synthesis transitions (Together..., These results suggest...). Use them where they clarify the argument, without imposing them on every paragraph. A purposeful contrast or a list of three actual property views is substantive, not automatically an AI tell.

Allow medium-length and longer sentences when a qualification or comparison remains easy to follow. Split competing ideas and deeply nested clauses, not sentences solely because they cross a word-count threshold. Preserve paragraph organization during ordinary polishing; restructure when the user requests it or when necessary to resolve a clear flow problem, explaining material changes.

## Evidence and limits
Prefer the more carefully qualified style of the coreset-selection sample when interpreting empirical evidence. Name the dataset, learner, budget, metric, and comparator needed to delimit a claim. Report unfavorable comparisons and strong random baselines directly. Do not turn a conditional advantage into universal superiority.

Keep observed effects separate from statistical significance and proposed mechanisms separate from demonstrated causes. Preserve the distinction between variability across independently selected subsets and training variability conditional on a fixed subset. A single-run point estimate is not a confidence claim.

Preserve supplied numbers, equations, citations, labels, and experimental conditions. Do not borrow numerical results from the calibration papers for a new manuscript. If wording conflicts with a table or protocol, flag the discrepancy rather than silently changing scientific content. Do not invent evidence pointers or tests to make an assertion sound supported.

## Illustrative patterns, not manuscript quotations
- Comparison: 'Under [budget], [method] obtains [metric], compared with [baseline value]. The difference is smaller on [other setting].'
- Interpretation: 'These results suggest that [component] is useful under [observed condition]; they do not establish [broader claim].'
- Limitation: 'The benefit depends on [dataset/learner/budget]. Further evaluation is needed to determine whether it extends to [untested setting].'
Use these as reasoning patterns, not sentence templates to repeat mechanically. Fill brackets only from the current manuscript or verified supporting material.

## Updating this profile
Refine it when the user supplies new writing samples or explicit corrections. Distinguish user-stated preferences from inferred tendencies. Keep updates narrow and retain contradictory evidence as context-dependent variation. Do not treat ordinary edited outputs as new author-approved training samples. This file guides inference-time editing; it does not train model weights or create automatic memory.
