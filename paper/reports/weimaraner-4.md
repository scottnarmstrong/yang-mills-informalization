# Weimaraner — checkpoint 4

2026-11-11. Revision only, under round-3 feedback with rounds 1–2 retained.

Revised both existing limit sections. Converted reader-facing text to British spelling and adopted the editor's distinction between observable indices, classical polynomials and continuum fields. Preserved the mathematical reference labels.

Rebuilt the compactness subsection around its idea: moving an insertion changes the empty-slice propagation distances, positivity bounds that change, and boundedness plus equicontinuity gives common subsequences. The extraction statement now precedes the technical proof. Cell placement, trace estimates and finite-net arguments are displayed within the proof. The section opening identifies the actual ultraviolet inputs and explains the later scalar-product and rotation constructions.

Defined the reflection planes, centred cells, expectation notation, coefficient norms, ordered tails, cell errors and quotient fields explicitly. Maxwell now explains colour components, Taylor tensors, radial potentials, probes, restriction, reflected observations and Wick matchings. Shared free derivatives and moving tested observations are defined outside proofs. The derivative comparison displays its local L1 and Fourier steps.

**Self-check tables are complete:** 82 rows for Infinite volume and 62 for Maxwell in `notes/weimaraner.md`, giving definition locations, first uses and repairs. No unresolved definition or terminology finding remains in this source audit. All IV4-1–5 and MX4-1–5 editorial requests are addressed.

Rechecked the moved/expanded formulas against pinned Lean revision `3456e5e75cf8d4cd558955a5c7638fba2d68f464`; correspondence is recorded in the notes. All 13 earlier results and their quantifier, normalisation and limit conventions survive. Five visible proof obligations remain: chosen-family centred estimates; equation/comparison/rank inputs; full-spacing fixed-volume convergence; analytic Maxwell positivity/strictness; and chosen-family Maxwell comparison with its independent dimension cap. This revision closes none of those deferred proofs. No Lean/Lake run or independent proof audit is claimed.

The prescribed latexmk build exits 0 with no warnings, missing references/citations or overfull/underfull boxes. Reread every rendered page 32–56, including both section boundaries; rechecked all changed pages after the final repairs. Infinite volume touches 14 pages, within its approved cap 15; Maxwell touches 11, within cap 14. Static checks pass, and temporary previews were removed.

No decision requested. Report 4 is written; stopping and waiting.
