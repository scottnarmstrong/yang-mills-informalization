# Weimaraner audit of dalmatian's sections

Scope: rendered PDF pages 1–18; source files `part1/*` and `part2/00-opening.tex`. Read as a first-time reader with only preceding pages available.

1. [R] §1, `part1/01-result.tex:18–22`: “Part I begins with definitions … The strategy then separates the proof … Part II develops their proofs …” repeats the paper route again in §4 and the Part II opening; the reader needs one whole-paper roadmap, then only genuinely new local orientation.
2. [R] §4, `part1/04-strategy.tex:3–7`: “two limiting operations and then three ways of reading the same limiting correlations” repeats the finite-volume, phase, field, product and trace route already given at `part1/01-result.tex:18–22`; this overview adds little to the five detailed proposition ideas below.
3. [R] §4, `part1/04-strategy.tex:46–52`: the diagram is followed by “the last three results all use estimates for the same lattice family” and then “one joint choice of the family … one joint choice of a refinement”; the same-family dependency is restated twice, so retain the distinctions without repeating the shared-choice point.
4. [R] §5, `part1/05-propositions.tex:3–4`: “The five propositions below use the joint choices described in Section 4” and “complete proofs belong to Part II” repeat the joint-choice and proof-location statements at `part1/04-strategy.tex:49–52`.
5. [R] Part II opening, `part2/00-opening.tex:3–16`: the two tasks and five-stage list restate the full construction route in §4 and the whole-paper route in §1; keep the information particular to how Part II is organised.
6. [R] Part II opening, `part2/00-opening.tex:52–74`: the sections 8–9 / phases summary repeats the box-to-phases and three-conclusions summaries at `part1/04-strategy.tex:18–31`; consolidate the repeated account or give only details unique to the construction guide.
7. [R] Part II opening, `part2/00-opening.tex:76–81`: “Reading the construction” again walks through the lattice, ultraviolet, Maxwell, symmetry, phase and reconstruction route already stated at `part2/00-opening.tex:3–74`; retain the distinct reading advice and remove the repeated roadmap.
8. [U] §2.3, `part1/02-definitions.tex:213`: “with the corresponding Schwartz topology” names a topology without specifying its defining seminorms or a usable description of convergence.
9. [U] §2.4, `part1/02-definitions.tex:292`: the coefficient function is written `c_{j,κ}(a;x,o)` on a product space, but the roles of `x` and `o` (the insertion list and its centre) are not explained here or before this first use.
10. [U] §2.4, `part1/02-definitions.tex:293`: “An element Θ∈F₄” introduces the distinguished trace field without saying what it represents or why the hierarchy singles it out; the stress-trace role is only alluded to later.
11. [U] §2.5, `part1/02-definitions.tex:424–426`: the profile formula uses the exponent `d_{αβ}` in each kernel power, but neither the mode nor the finite-profile definition declares `d_{αβ}` or its allowed values.
12. [U] §5, `part1/05-propositions.tex:139–143`: “positive-energy representation” introduces `dσ(E)≥0` without saying that σ is a positive measure or identifying its spectral source; the displayed integral alone does not explain this input.
13. [U] §5, `part1/05-propositions.tex:50–54`: the proof idea uses `Θ_C`, the cell family `C`, and `||F_C||_C` before those objects are defined in §8; the forward links to Definitions 8.2 and (8.6) do not explain the symbols at this first use.
14. [L] §5, `part1/05-propositions.tex:62–65`: “Rotation identities make those operators commute” has no reference to where the identities are stated or proved, nor to the integral identities used to obtain them.
15. [D] §5, `part1/05-propositions.tex:56`: “Slice integration bounds the change … Boundedness and this uniform continuity select a common subsequence … summation by parts then identifies derivatives” compresses movement, extraction and derivative identification into one step without the movement inequality or difference-quotient formula that would show the mechanism.
16. Part II opening, `part2/00-opening.tex:25–27`: “density expansions” and “plaquettes have large deviations” are unexplained technical terms [J]; state what is expanded and what counts as a large plaquette deviation.
17. Part II opening, `part2/00-opening.tex:22,29–35`: “short-distance variables are integrated out” and “running coupling” are reused as specialist shorthand [J/U] without a plain explanation at their first use in this guide; explain the averaging operation and the scale-dependent coupling coefficient.
18. Part II opening, `part2/00-opening.tex:53–66`: “reflection positivity” is used as the key bound and as the source of the inner product, but the defining positivity statement is not given and the pointer is only to Section 8 [L/U]; cite the precise reflection estimate and explain its positive quadratic form.

AUDIT COMPLETE

## Phase C — rendered verification

Reread the repaired rendered PDF, pages 1–19 (Part I and the complete Part II opening), after `dalmatian-response.md` ended with `REPAIR COMPLETE`.

1. **fixed.** The whole-paper route is stated once in §1; the revised strategy and Part II guide give local construction information.
2. **fixed.** §4 opens with the dependency diagram and proceeds to the distinct mathematical stages rather than restating the whole-paper route.
3. **fixed.** The diagram's dependency explanation is concise and distinguishes the family choice from the later common subsequence.
4. **fixed.** §5's introduction only describes the proof sketches and detailed estimates.
5. **fixed.** The Part II opening is organized around tracking observables, the ordered limit, fields, and reading advice; the former five-stage roadmap is gone.
6. **fixed.** The opening no longer repeats the §4 phase-and-conclusions route; it explains operations specific to the construction sections.
7. **fixed.** The reading advice is limited to fixed quantities, limit order, and volume dependence.
8. **fixed.** Definition 2.14 gives the Schwartz seminorms that generate the topology.
9. **fixed.** H7 identifies `x` as insertion positions and `o` as the replacement centre at first use.
10. **fixed.** H8 identifies Θ as the degree-four field used in the trace test, and the following text explains its stress-trace role before the test.
11. **fixed (stale finding).** The rendered profile uses the declared natural-number exponent `q_{αβ}`; `d_{αβ}` does not occur.
12. **fixed.** The proof idea identifies σ as the positive spectral measure from the spectral theorem for the selected trace two-point function and names the energy operator.
13. **fixed.** The proof idea explains the reflected cell, reflected-conjugate observable, and one-cell bound before using the cell inequality.
14. **fixed.** Rotation identities are explicitly conditional and recorded as an unproved step in the gap.
15. **fixed.** The proof idea gives the movement inequality, its fixed-data and separation conditions, and the summation-by-parts derivative argument.
16. **fixed.** The opening states what is averaged and describes both plaquette regions in ordinary terms.
17. **fixed.** Fine-link integration and the scale-dependent quadratic coefficient are explained without the former shorthand.
18. **fixed.** The opening states the reflected-conjugate nonnegative pairing and points to the finite-lattice and repeated-cell inequalities.

### New failures found in verification

19. **Not fixed [R] §2.4, `part1/02-definitions.tex`, R15 discussion:** “this convention makes the boundary-value limit a defined statement without asserting positive-height integrability” is immediately repeated by “It makes the displayed limit a defined statement even when integrability has not been proved.” Keep one sentence explaining the zero-if-nonintegrable convention.

20. **Not fixed [R] Part II opening, `part2/00-opening.tex`, “From correlation functions to fields” and following paragraph:** the first paragraph explains that reflection of a positive-time product gives a nonnegative pairing; the paragraph after the Maxwell comparison repeats that reflection positivity builds the Hilbert space and defines its inner product. The latter may retain the distinct missing-rotation-identities point, but the Hilbert-space construction and pairing should be stated only once.

VERIFIED
