# Dalmatian's Round 7 audit of Weimaraner's Ward section

Scope: `part2/limit/03-ward.tex`, read in source and in the successful rendered PDF (printed pages 68–73), plus class S in the older sections `part2/limit/01-infinite-volume.tex` and `part2/limit/02-maxwell.tex`.

## Findings

1. **U/J — `03-ward.tex:35–39`, mixed OS slabs.** The text introduces `P_{\mu,d}(w)` as an insertion-and-translation operator by describing its effect on a future word vector, but it does not specify the dense domain on which it acts or how the prescription descends through the zero-norm quotient. State the domain (the span of future test-word vectors), define the action there, and say what establishes that the action is well defined on equivalence classes before its operator norm is used. The conditional reflected-train estimate is a bound for that operator, not its definition.

2. **U/J — `03-ward.tex:52–73`, finite-cutoff shell relation.** `Flux` and `Charge` are central terms in (12.6), but their summands are described only as using adjacent cutoff values, a minus sign, and link-variation contact terms at “active Ward centres.” The active-centre condition, the precise shifted boundary weight, and the contact stencil are not stated. Since the following gap specifically says those exact weights and the contact stencil must be retained, the displayed relation is not yet independently interpretable from the paper. Give the finite sums (or a self-contained definition immediately before (12.6)) and define active Ward centres and the support/exterior convention.

3. **U/J — `03-ward.tex:77–85`, continuum rotation identity.** `D_K` is first introduced as “the corresponding infinitesimal linear map” on `F_d`, but the correspondence is not defined. Explain how the skew matrix acts on the field labels/derivatives before the exact orthogonal action has been constructed, or link to the definition that fixes this infinitesimal map. Otherwise the field-action term in (12.7), and the later bracket relation, have no reader-facing definition.

4. **U/J — `03-ward.tex:115–124`, stress candidate.** The “finite-dimensional space of real stress coefficients” and the “stress polynomial map” `Mat` are not defined or linked to a reader-facing definition. Add a short description of the coefficient data and how the map turns them into a degree-four field array, or provide a stable definition link before using `Mat(w)` in (12.9). The source footnote does not define this object for the reader.

## Class S sweep

Searched both older Weimaraner sections for the former enumerate/italic-step proof format and one-sentence “Step n” items. All substantial proof stages use `\proofstep`; remaining `enumerate` environments are labelled proposition-clause lists. No obsolete proof-step format found. The Ward section has no proof-step list requiring conversion.

The six rendered Ward pages were read in order. The section fits its pages and its unresolved analytic inputs remain explicitly marked; the findings above concern definitions needed to read the stated constructions and identities, not closure of those open inputs.

AUDIT COMPLETE

## Verification after Weimaraner's response

Reread the repaired source and the rendered Ward pages 70–75 of the 75-page combined PDF. Status of the original findings:

1. **Fixed.** The dense span of future-word vectors is named, the word-level insertion/translation prescription is stated, and descent through zero-norm vectors is tied to a boundedness estimate.
2. **Not fixed (why).** The shifted boundary weight, finite Flux/Charge sums, active centres and exterior condition are now displayed. However the contact definition still depends on undefined `bump(x,d,tE_alpha,U)` and a “colour-valued” clover that is only described as a signed average; no map from its group-valued plaquette transports to the colour components `X_{...,alpha}` is specified. The finite relation also still uses `T`, `D` and `B` described only as calibrated stress, centred divergence and equation insertion, without giving their defining formulas or a precise definition link. These are the very data needed to determine the exact identity, so the relation remains underdefined for a reader.
3. **Fixed.** The raw coefficient variation is displayed as a derivative of the rotation pullback, and descent to the quotient is explicitly conditional on preserving the invisible subspace.
4. **Fixed.** The four coefficients, polynomial array and quotient map defining `Mat` are now displayed and linked to the curvature and quotient definitions.

## Additional findings from the second reading

5. **D/U — `03-ward.tex:33`, reflected-train estimate.** The sentence says the estimate “bounds the output norm by the input norm,” which asserts a contraction, while (12.3) permits an operator norm larger than one. State the actual bound `\|P(w)u\|\le C^{|w|}(|w|/r)^{\kappa|w|}\|u\|` (or the correct source bound) and use that same constant to justify preservation of null vectors.

6. **U/D — `03-ward.tex:158–163`, stress candidate.** The argument invokes “real-rank inputs” and says they compare dimensions in degrees four and five, but neither the rank inequalities nor an explicit hypothesis that they hold appears before the existence conclusion (12.11). State the exact finite-dimensional rank conditions as hypotheses, or display the source result with its full assumptions. Merely saying that dimensions are compared does not imply the candidate exists.

7. **R — `03-ward.tex:138`, rendered page 73.** The source-footnote marker 38 is stranded alone on a line after the unresolved-action paragraph, while its footnote is at the page foot. Attach the citation to the preceding sentence/gap so its marker sits with the text, and keep the note on the same page if possible.

8. **D — `03-ward.tex:34–37`, slab bound.** The definition permits an empty word, but the displayed right side contains `( |w|/r )^{kappa |w|}`, which becomes `0^0` when `|w|=0`. State a convention that this factor is 1 for the empty word, or restrict (12.3) to nonempty words and handle the identity operator separately.

The new review is complete; finding 2 remains unresolved and findings 5–8 are new owner repairs. The prescribed build used for this reread succeeds (75 pages); the log has no TeX errors, unresolved references or overfull/underfull boxes, and retains the empty-bibliography warning. Rendered Ward pages 70–74 are legible apart from the orphaned marker; page 75 is the empty References page.

VERIFIED

## Final verification after Weimaraner's second repair section

Confirmed the response file is newer and its follow-up section ends `REPAIR COMPLETE`. Reran the prescribed build check and reread rendered pages 70–76 of the current 76-page PDF. Requested findings:

2. **Fixed.** The current section defines the lattice insertion, centred divergence, holonomy and Lie-algebra projection, clover, oriented link bump, force, equation insertion, contact stencil, shifted boundary weight, support condition and finite sums. The finite identity remains correctly marked as unproved.
5. **Fixed.** The quotient-vector estimate includes norms on both sides and the matching operator norm bound.
6. **Fixed.** The real signed-symmetry spaces and both comparison hypotheses are displayed before the dimension argument.
7. **Not fixed (why).** The former marker 38 now sits with its citation on page 74, but marker 40 is still stranded alone after the stress-normalisation gap on page 76, while its footnote is at the page foot. The class-wide stranded-marker failure therefore remains; attach citation 40 to the explanatory paragraph before the gap or otherwise keep its marker with the cited text.
8. **Fixed.** The power bound is for nonempty words, and the empty-word operator is separately the identity.

No further mathematical or layout failure was found in this pass. `latexmk -pdf -interaction=nonstopmode main.tex` reports the current PDF up to date (76 pages); the log contains no TeX errors, undefined references, or overfull/underfull boxes, and retains only the empty-bibliography warning. Current PDF SHA-256: `b190a3a906a3cedcf1d20f8871bdeda30303f70474a0af56600e0629f48db2b9`.

VERIFIED

## Second verification after Weimaraner's follow-up repair

Reread the updated source and rendered pages 70–76 of the 76-page combined PDF. Requested findings 2 and 5–8 now read as follows:

2. **Fixed.** The section now defines the degree-four lattice insertion, centred divergence, plaquette holonomy and Lie-algebra projection, clover components, oriented link bump, force, equation insertion, contact stencil, shifted weight, active centres and finite Flux/Charge sums. The exact finite-cutoff identity is still explicitly an open proof obligation.
5. **Fixed.** The reflected-train estimate now bounds the norm of the quotient vector by the stated factor times the input norm, and separately gives the operator norm bound.
6. **Fixed.** The real signed-symmetry spaces and the exact degree-four isomorphism and degree-five dimension bound are stated before the dimension argument; the candidate is conditional on those explicit inputs.
7. **Fixed as to marker 38.** Its citation is now attached to the action-construction paragraph and fits on page 74.
8. **Fixed.** The formula is restricted to nonempty words; the empty-word operator is separately the identity.

New finding: **R — `03-ward.tex:224`, rendered page 76.** The stress-normalisation footnote marker 40 is again stranded alone after the unresolved paragraph, with its note at the foot of the page. Attach the citation to the preceding explanatory paragraph or otherwise keep its marker with the cited text. The other added formulas and the degree-four/five rank argument render legibly; no additional mathematical failure was found in this pass.

The prescribed `latexmk -pdf -interaction=nonstopmode main.tex` reports the 76-page PDF up to date. Its log has no TeX errors, undefined references, or overfull/underfull boxes; the only warning is the empty bibliography. PDF SHA-256: `8aa989c654e24ae390689049e73f7690bebaa01123fc4266f1cd788c8c38f730`.

VERIFIED
