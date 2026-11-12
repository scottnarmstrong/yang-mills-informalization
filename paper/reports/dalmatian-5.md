# Dalmatian report 5

Round 5 was revision only. I shortened P2 and P3 of Theorem A, leaving the complete reconstruction and OPE contracts in their linked definitions. In the five proof ideas in Section 5, I replaced prose-only routes with numbered steps and displays:

- **Ultraviolet construction:** normalized integration, small/large fields, running coupling, reference-normalised insertions, intermediate-scale Cauchy order.
- **Limit and phases:** reflection-root bound, movement and compactness, ordered limits, zero-energy projection, mixture formula.
- **Reconstruction:** smeared limits, OS pairing, continuation/locality, null quotient.
- **OPE:** cluster replacement, displayed remainder power, coefficients chosen before spectators and phases.
- **Trace:** exact trace limit, positive spectral representation, radius squeezing, finite-profile exclusion.

I added a five-stage reading guide to the Part II opening; it links the existing ordered-limit definition without repeating its display. The five analytic obligations remain explicit. The round-5 self-check and a passage-by-passage Section 5 change list are in `paper/notes/dalmatian.md`.

My editorial read of all four Part II sections found proof-idea summaries still in unnumbered prose. I sent greyhound UV5-1–3 (Wilson law, polynomial labels, insertion, sections, marker algebra and activity sums) and weimaraner IV5-1/MX5-1 (raw extraction and six Maxwell proofs) as concrete requests in the notes. `lem:iv-reflection` and `prop:iv-euclidean` already have enumerated proof routes and displayed positivity/limit calculations. I did not edit the other owners' files or change any mathematical hypotheses.

The required `latexmk -pdf -interaction=nonstopmode main.tex` build succeeded: 60-page PDF, no log warnings/errors or overfull/underfull boxes. I reread rendered pages 10–19, including the Part II boundary. PDF SHA-256: `4856bc535cdde6e11f983ceefea742c3ef24477f4c96047a5bb28e0fd97cdbaa`.
