# Greyhound audit of Dalmatian's Round 7 section

Scope: first-reader review of `paper/part1/06-constants.tex`, plus class S review of Dalmatian's older Part I sections and the Part II opening. I checked the cited schedule and selected-trajectory statements against the pinned source at `3456e5e75cf8d4cd558955a5c7638fba2d68f464`.

## Findings

1. **S — blocking build errors, `part1/06-constants.tex:6,12`.** The source references inside `\texttt{...}` contain unescaped underscores (`continuum_with_position_tests`, `exists_above`). The combined `main.log` reports four `Missing $ inserted` errors on these two lines. The build emits a PDF only after TeX recovery and is not a valid successful build. Escape the underscores or use a source-name command that handles them. Check the entire section for the same source-name pattern, then rerun the prescribed build.

2. **U/J — first-use meanings, paragraphs “Choices made before the block ratios” and “Block ratios and later thresholds.”** “Stage profile” is only described as a list of kinds of data. The later “smallness exponents,” “post-block costs,” “entry thresholds,” “volume conditions,” “waiting windows” and “minimum period length” are named but their mathematical role is not stated. Give a short reader-facing meaning for each group (what is required or controlled, and at which stage), or link to a displayed definition that does so. The source `Sheet`/`Stage`, `Protection`, `Delays`, `Bar` and `Wait` names in footnotes are not definitions for the reader.

3. **D — cumulative drift deduction, paragraph after `eq:constants-schedule`.** The preceding displayed bound controls one increment by `omega_{J_{m+1}}`; the section then asserts a uniform `o(s_m)` estimate without showing the accumulation. Add the telescoping estimate
   `|beta_{N,p,m}-hat beta_m| <= sum_{i<m} omega_{J_{i+1}}`
   and explain why the high-index ratio bound makes this sum `o(s_m)`, while the finitely many initial terms vanish after division by `s_m`. Preserve the source quantifiers `N>=m` and all `p` in that deduction.

4. **U — order-of-choice wording, paragraph “Block ratios and later thresholds.”** “The logarithm of the stage cost divided by `log ell_j`” does not identify which displayed profile expression is meant. State it as a formula or name its terms in reader language, so the asserted `j^{-2}` payment can be checked against the preceding profile description.

## Class S sweep

Searched Dalmatian's older Part I sections and `part2/00-opening.tex` for the former enumerate/`\item \emph{...}` proof-step forms and one-sentence “Step n” items. The long proof stages in `part1/05-propositions.tex` use `\proofstep`; the remaining enumerates in Part I are labelled theorem/definition lists, not proof steps. I found no obsolete proof-step form in the reviewed older sections.

The audit is complete once findings 1–4 are repaired and the owner has rerun the build.

AUDIT COMPLETE

## Verification of Dalmatian's repair

1. **Fixed.** `\nolinkurl{...}` now safely typesets both underscore-containing identifiers. I searched the constants section for remaining raw source-name underscores and found none. The combined `latexmk -g -pdf -interaction=nonstopmode main.tex` exits 0. Its only warning is the existing empty bibliography environment. The rendered constants section (pages 17–18) has no malformed source names.
2. **Fixed.** The profile paragraph now explains the roles of its estimates, and the following paragraph explains the smallness, post-block, entry, volume, waiting and period choices. The stage cost has its own displayed definition and named terms.
3. **Fixed.** The telescoping estimate is displayed; the subsequent paragraph derives the uniform `o(s_m)` statement and retains `N>=m` and every `p`.
4. **Fixed.** The stage cost is explicitly defined and its logarithmic ratio is displayed.

I reran the older-section proof-step search and reread pages 17–19, including the Part II boundary. The class S conversion remains correct, and the repaired section renders legibly.

VERIFIED
