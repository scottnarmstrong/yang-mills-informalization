# Dalmatian response to the Part I and opening audits

Scope: the 18 findings in `weimaraner-on-dalmatian.md` and all 60 recovered findings in `supplementary-on-dalmatian.md`. Both audit inputs were read and left unchanged. Every finding below was checked against the current source; class-wide sweeps are recorded after the item lists. The supplementary item 11 quotes an exponent that is not present in the current source and is handled as a stale finding.

## Official audit: findings 1–18

1. **Fixed.** Removed the extra whole-paper route at the end of `01-result.tex`. Generalized: searched the result, strategy, propositions and opening for roadmap repetitions; retained only the orientation needed at each location.
2. **Fixed.** Replaced the route-summary opening of `04-strategy.tex` with its local purpose: the dependency diagram. Generalized the same roadmap search as in 1.
3. **Fixed.** Kept one sentence after the diagram stating the family/refinement dependency; removed the duplicated shared-choice summary. Generalized: checked the dependency prose against all five proposition sketches.
4. **Fixed.** The proposition-section introduction now says only that sketches give the mathematical steps and detailed estimates are in Part II. Generalized: searched adjacent sections for repeated proof-location statements.
5. **Fixed.** Removed the five-stage list from the Part II opening. Its subsections now explain their own operations and order. Generalized: removed duplicate high-level roadmaps across Part I and the opening.
6. **Fixed.** Removed the repeated “Phases and short distances” route summary from the Part II opening. Generalized: compared every remaining opening paragraph with the Part I strategy; retained only construction-specific details and reading advice.
7. **Fixed.** “Reading the construction” now gives the distinct advice to track fixed quantities, limit order and volume dependence. Generalized: checked that it no longer repeats the lattice-to-phase route.
8. **Fixed.** Defined Schwartz convergence by the seminorms `p_{M,alpha}`. Generalized: searched all topology/convergence introductions in the owned definitions for usable descriptions.
9. **Fixed.** Defined `x` as the insertion-position list and `o` as the replacement centre where `c_{j,kappa}(a;x,o)` first appears. Generalized: checked every hierarchy index and coefficient argument at first use.
10. **Fixed.** Identified `Theta` as the degree-four field used in the trace two-point test, then explained its stress-trace role before the trace-test definition. Generalized: searched every use of the distinguished field and trace terminology.
11. **Disposition: stale finding; no source change.** The current profile uses `q_{alpha beta}`, declared to be a natural number; `d_{alpha beta}` does not occur. Generalized: searched the mode and profile formulas for every exponent/index and checked their declarations.
12. **Fixed.** Named `sigma` as the positive spectral measure supplied by the spectral theorem for the selected trace two-point function and the energy operator from Proposition 5.2. Generalized: checked other spectral-measure language in the proposition sketches.
13. **Fixed.** Defined reflected cells, `Theta_C F_C`, and the one-cell bound `||F_C||_C` in the proof idea before the inequality, with references to the construction definitions. Generalized: checked each proof-idea symbol that is first defined later in Part II.
14. **Fixed by making the status explicit.** No rotation identity or proof of the required commutation occurs in the construction text. The proof idea now states the required `AB=BA` step is open and points to the following gap instead of asserting an unsupported identity. Generalized: searched all owned text for rotation-identity/commutation claims; the strategy is conditional (“once rotations are established”), and the reconstruction gap now also names the missing Euclidean rotation identities.
15. **Fixed.** Added the finite-difference movement estimate with other labels and positions fixed, stated the separation condition, and explained test-function summation by parts and the derivative limit. Generalized: checked all five proof ideas for compressed movement/extraction steps.
16. **Fixed.** Replaced “density expansions” and “large deviations” with the concrete coarse-link averaging and the treatment of plaquettes away from the identity. Generalized: searched the opening for technical shorthand and explained the operation at its first use.
17. **Fixed.** Explained integration over fine links, preservation of the integral, and the scale-dependent quadratic-curvature coefficient; removed “running coupling” shorthand from the opening. Generalized: checked every scale/coupling reference in the opening and strategy.
18. **Fixed.** The opening now defines the reflected-conjugate pairing, states its nonnegative finite-lattice inequality, and links both that inequality and its repeated-cell form. Generalized: checked all reflection-positivity uses in the owned overview and proof ideas for an explicit operation or precise pointer.

## Recovered supplementary audit: findings 1–60

1. **Fixed.** Explained component-state averages before naming their components phases. Generalized the first-use scan for state/phase terms.
2. **Fixed.** Translated positive energy, spacetime symmetry and spacelike commutation into reader-facing statements. Generalized the first-use scan for relativistic properties.
3. **Fixed.** Described nearby-product replacement, its centre, distant insertions and error before naming the OPE. Generalized the first-use scan for product terminology.
4. **Fixed.** Described finite sums/products of free-field kernels and linked the precise class to Definition 2.22. Generalized the comparison-class scan.
5. **Fixed.** Removed the source/revision status sentence from the result. Generalized: searched reader-facing Part I and opening prose for project/revision jargon.
6. **Fixed.** The definitions introduction says lattice limits may average component correlations and names those components phases. Generalized the first-use phase scan.
7. **Fixed.** Named the nearby-product estimate and the trace two-point comparison in the definitions introduction. Generalized the first-use scan for short-distance tests.
8. **Fixed.** Defined Lie algebra as infinitesimal matrix directions and explained simplicity as absence of a smaller nonzero commutation-invariant direction. Generalized the scan of group and representation terms.
9. **Fixed.** Explained the connection, its infinitesimal transport role, its Taylor data, and the relationship between classical polynomial and lattice insertion. Generalized the first-use scan for the local-observable map.
10. **Fixed.** Moved the expectation → moment → test-weighted lattice sum explanation before the display. Generalized the scan of definitions whose prose followed rather than prepared their formulas.
11. **Fixed with a precise distinction.** Stated `K_n` is indexed by `n,v`, while `R_p` may depend on `n,v,f`; the kernel cannot depend on `f` without changing the asserted correlation function. Generalized: checked all ordered-limit quantifiers against the displayed kernel and scalar limits.
12. **Fixed.** Explained strong continuity as continuity on each vector, the momentum meaning of the projection-valued measure, and finiteness of each diagonal measure. Generalized the scan of functional-analytic data.
13. **Fixed.** Described the represented transformations as continuous translations and orientation/time-preserving Lorentz transformations before identifying the group. Generalized the scan of transformation terminology.
14. **Fixed.** Explained countable additivity as convergence of finite projection sums on every vector. Generalized the measure-definition scan for convergence mode.
15. **Fixed.** Removed the unexplained double-cover aside and explained the Euclidean dot product versus the Minkowski cone condition. Generalized the scan of signature/group asides.
16. **Fixed.** Explained the continuation as the complex-time extension used for real-time expectations and the finite coefficient sets as the fields retained at each degree. Generalized the hierarchy-item scan for purpose, not just domain.
17. **Fixed.** Explained the map from lattice observable index to continuum field and then quantum-field label. Generalized the scan of maps between representations.
18. **Fixed.** Distinguished `xi_*`, which selects one phase, from `mix`, which denotes the average of all phase correlations. Generalized the phase-role scan across the definitions and theorem.
19. **Fixed.** Replaced “formal source” wording with the exact zero-if-nonintegrable boundary-value convention and explained that it defines the limit without asserting positive-height integrability. Generalized: searched the owned text for source-status conventions.
20. **Fixed.** Defined cluster, spectators and the data on which the radius threshold may depend before the cluster definition. Generalized the first-use scan of product geometry.
21. **Fixed.** Explained the fixed coefficient system, the data-dependent small-radius threshold, the finite degree cutoff and the resulting finite error estimate. Generalized the scan of OPE quantifiers and remainder language.
22. **Fixed.** Explained the mass/energy kernel, the homogeneity law for `h`, the natural exponents, and that the comparison class consists of finite sums and products of these kernels. Generalized the scan of profile symbols and their roles.
23. **Fixed.** Explained the stress tensor, its diagonal trace, vacuum centering, and why the public test singles out a degree-four field before stating the trace test. Generalized: checked every stress/trace use in the definitions and propositions.
24. **Fixed.** P2 identifies the selected point `xi_*` and says its phase supplies the Euclidean values of the continuation. Generalized: checked every theorem use of selected/mixed data against the hierarchy definition.
25. **Fixed.** P4 states zero vacuum expectation and points directly to T1. Generalized: checked “centred” in the theorem and trace proposition against that condition.
26. **Fixed.** Rewrote the nonclaims in ordinary terms: no extension to coincident-point smearings and no exclusion of all polynomial free-field combinations or a continuum of free-field masses. Generalized: searched the theorem for specialist exclusions and expanded only the scope needed to delimit the claim.
27. **Fixed.** Replaced “three ways of reading” with the concrete uses of one hierarchy in reconstruction, product replacement and the trace test. Generalized the redundancy/first-use scan in strategy.
28. **Fixed.** Specified retained coarse links, integrated fine links, the reference spacing and the quadratic coefficient fixed in the comparison. Generalized the first-use scan for scale and coupling language.
29. **Fixed.** Strategy explains positive reflected pairings, the long-time zero-energy part and that phase separation follows only after rotations are established. Generalized the scan of the compactness-to-phase chain; the proof sketch records the remaining commutation gap.
30. **Fixed.** Explained complex-time continuation, finite product replacement and the finite comparison class in the strategy. Generalized the scan of conclusion shorthand.
31. **Fixed.** The proposition-section introduction distinguishes proof sketches from detailed estimates in Part II without repeating the joint choices. Generalized the proof-location/dependency redundancy scan.
32. **Fixed.** Defined fine/coarse conditional averaging and displayed preservation of the total integral. Generalized the scan of integration and density symbols in the UV proof idea.
33. **Fixed.** Explained both sides of the plaquette split, the identity-distance threshold, curvature approximation and energy control without discarding either region. Generalized the scan of small/large configuration terminology.
34. **Fixed.** At the insertion formula, explained `P_d`, factor rescaling, reference transfer and physical power scaling. Generalized the scan of operators and parameters in the displayed insertion formula.
35. **Fixed.** Displayed the three-term cutoff comparison at a common intermediate spacing and explained the order of limits in the Cauchy argument. Generalized the scan of limit/extraction steps.
36. **Fixed.** Replaced project-status jargon with the explicit estimates and fixed-volume conclusion still needing proof. Generalized the gap-prose scan throughout the proposition sketches.
37. **Fixed.** Defined cell reflections, cell family and one-cell bound before the chessboard inequality. Generalized the scan of forward references to Part II objects.
38. **Fixed.** Added the finite-difference movement inequality and explained test-function summation by parts and derivative identification. Generalized the scan of dense movement arguments.
39. **Fixed.** Defined `H` and `P_0`; stated the required commutation relation and marked it open. Generalized the scan of introduced operators and unsupported identities.
40. **Fixed.** Explained the conditional joint spectral representation, compact joint-value space, coordinate functions and induced probability measure. Generalized the scan of abstract phase-space conclusions.
41. **Fixed.** The gap names the volume-independent local and derivative bounds, the far-away stress integral and the missing commutation. Generalized the gap scan for unnamed remaining work.
42. **Fixed.** Explained spectral damping and how imaginary time changes the exponential into unitary evolution. Generalized the first-use scan for reconstruction terminology.
43. **Fixed.** Enumerated the reflection construction, OS inner product, completion/null quotient, continuation, locality and domains in the four proof steps. Generalized the scan of all reconstruction proof ideas.
44. **Fixed.** Named the missing small-imaginary-time bound, equality of spacelike boundary values and quotient-domain checks. Generalized the gap scan for mathematical obligations rather than status language.
45. **Fixed.** Explained translation to the centre, selection of coefficients before spectators, finite truncation and the operator-bound role. Generalized the product-proof scan for suppressed quantifier logic.
46. **Fixed.** Stated the coefficient, remainder and operator bounds still required. Generalized the gap scan.
47. **Fixed.** Connected the centred stress trace to the degree-four field and specified the two-point law being compared. Generalized the trace terminology scan.
48. **Fixed.** Explained comparison with free Maxwell curvature fields and the two inverse-coupling factors. Generalized the trace-comparison scan.
49. **Fixed.** Explained the positive spectral measure, monotonicity, sequence squeeze and finite-profile asymptotic contrast. Generalized the spectral/profile scan; the spectral-source wording was further clarified under official finding 12.
50. **Fixed.** Named the trace normalisation, dense-enough radii, and kernel/profile asymptotics that remain unproved. Generalized the gap scan.
51. **Fixed.** Removed the five-stage list rather than leaving its unexplained terms in a roadmap. Generalized the roadmap scan across Part I and the opening.
52. **Fixed.** Explained Taylor data and the link-polynomial representation; replaced density-expansion and large-deviation shorthand with concrete operations. Generalized the first-use scan for UV terms.
53. **Fixed.** Explained the two plaquette regions, density from fine-link integration, volume-independent local bounds and reference quadratic coefficient. Generalized the scan for scale, density and coupling terms.
54. **Fixed.** Stated the full-spacing fixed-volume limit, volume-independent continuity bounds, common subsequence and ordered-limit identification. Generalized the limit-order/extraction scan.
55. **Fixed.** Gave the positive reflected pairing and links to its finite and repeated-cell inequalities; explained the null-correlation quotient and derivative estimates. Generalized the reflection/quotient scan.
56. **Fixed.** Explained the free Maxwell field as a free electromagnetic curvature field, the comparison-map purpose and the required separate dimension input. Generalized the comparison terminology scan.
57. **Fixed.** Named time-zero reflection and complex conjugation, stated the positive pairing, and linked both lattice and repeated-cell estimates. Generalized the reflection positivity scan.
58. **Fixed.** Removed the duplicate long-time/phase summary from the opening; those concepts are explained once in the strategy and proposition idea. Generalized the route-redundancy scan.
59. **Fixed.** Removed the unexplained navigation summary about trace/product sections; their distinct mathematical roles are stated in the Part I results and proofs. Generalized the navigation-label scan.
60. **Fixed.** Retained only concrete reading advice: identify fixed quantities, the limit order and volume dependence. Generalized the opening scan for scale-normalisation shorthand.

## Class-wide generalisation checks

- **U:** Reread each owned paragraph and searched first uses of phase/state, index/field maps, topology, measures, hierarchy entries, reflection, cluster, kernels, trace and proof symbols. Definitions now precede use or have a local explanation and link. The one stale exponent report is documented at supplementary finding 11.
- **R:** Compared the result, strategy, proposition introduction and Part II opening for every route summary. Removed repeated roadmaps and duplicate phase summaries; kept the dependency diagram and unique estimate-reading advice.
- **J:** Searched for source/revision terminology, undefined shorthand and specialist terms named in both audits. Replaced them with the operation or mathematical input; unresolved proof obligations remain stated as mathematical gaps.
- **D:** All five proposition ideas use enumerated steps. The spacing Cauchy comparison, cell bound, movement estimate, phase representation, reflection construction, OPE truncation and spectral squeeze now have formulas and explanatory order.
- **L:** Checked first and distant reuse of the observable maps, test spaces, cells, reflection inequalities, hierarchy fields and trace data. Where the cited rotation identity does not exist in the construction text, the paper now records it as an open proof obligation rather than implying a reference or proof.

Rendered reread covered the updated Part I and Part II opening. The 63-page PDF builds; no source changes were made to either incoming audit. The open estimates and proof gaps remain open.


## Follow-up to rendered verification: findings 19–20

19. **Fixed.** Removed the second sentence that repeated why the zero-if-nonintegrable convention makes the boundary-value limit defined. Generalized: searched the owned definitions and proposition text for repetitions of the same explanation; the convention now appears once, while the separate statement about ordinary integrability of the lattice and phase integrals remains because it makes a different claim.

20. **Fixed.** Kept the reflected positive form and its precise estimates in the first Part II opening paragraph. Replaced the later repeated Hilbert-space/pairing explanation with the distinct required stress-tensor input for continuous rotations. Generalized across the owned files: `04-strategy.tex` now only identifies the reflection estimate's role in the later construction, and the reconstruction proof idea points to the positive form in the construction guide instead of restating its formula. The spatial reflected-cell bound remains in the phase proof idea because it is a different estimate. A search across Part I and the opening leaves one explicit reflected-pairing explanation.

I rebuilt `main.pdf` with `latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex`; the build completed successfully.

REPAIR COMPLETE
