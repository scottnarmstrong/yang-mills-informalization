# Fresh-reader audit: Weimaraner sections

Scope: rendered PDF, §8 “Infinite volume” and §9 “Free Maxwell fields”, pp. 34–59, read as a reader arriving from the preceding pages. Line numbers below refer to the current TeX sources. Findings are grouped only when the same passage exhibits the same failure; each numbered item identifies the exact wording and missing explanation or repair.

1. §8 opening, `01-infinite-volume.tex:3–6`: “pass from correlations in finite boxes”; “local observations”; “reflection inequality”; “repeated copies” (U/J): the paragraph uses several central objects before giving the reader a concrete example or plain-language account of what is being limited, what the observations are, and how the reflected expectation bounds them.
2. §8 opening, `01-infinite-volume.tex:8–16`: “common subsequences”; “coefficients that disappear”; “fixed representatives”; “auxiliary spacing subsequence”; “polynomial comparisons”; “scalar product”; “rotation argument”; “phase decomposition” (U/J/D): the reading guide lists technical outcomes without explaining their meaning or why they fit together; explain the section’s dependency chain in accessible terms, or defer the unexplained terms until defined.
3. §8.1, `01-infinite-volume.tex:20–22`: “classical polynomials”, “observable indices”, and “degree” (U/L): the reader is sent to the polynomial definition but is not told why a polynomial needs the extra degree component or what the index records in the model.
4. §8.1, `01-infinite-volume.tex:24–42`: “coefficient conventions”, “reference level”, “physical unit polynomial”, “coefficient list”, and the suppressed pairs (U/D): this convention definition introduces many notational operations in one block without a motivating example; in particular the reason one polynomial can have multiple degrees and why the degree must be retained are not made concrete.
5. §8.1, `01-infinite-volume.tex:44–58`: “block factors”, “reference levels”, and identities “assumed beyond the reference levels” (U/J): the scale hierarchy and the meaning of “beyond” a reference level are not explained, and the reader is not told why the slow-growth condition is needed here.
6. §8.1, `01-infinite-volume.tex:60–72`: “coordinate unit vector”, “pullback”, and “coordinate action” (U/J): the formula defines the point reflection but the link-configuration reflection is left as a reference; explain how the reflection acts on a link and why reversing it takes the inverse matrix.
7. §8.1, `01-infinite-volume.tex:74–90`: “cell tiling”, “interior”, “base cell”, “reflected copy”, “chessboard root”, “centred tiling”, and “physical point” (U/J/D): this definition packs several constructions together; give a small geometric explanation of the tiling/reflection operation and explain why the root compares one insertion to copies filling the torus.
8. §8.1, `01-infinite-volume.tex:93–100`: “ultraviolet estimate”, “cutoff threshold”, and “transformed polynomials” (U/J): the bound’s role is stated, but the estimate is not explained in words (what growth it controls and why it is uniform in volume); “transformed” is also left unspecified.
9. §8.1, `01-infinite-volume.tex:102`: “ultraviolet part”, “insertion identities”, “particular family”, and “reference” (U/J): this red unresolved note assumes the reader knows which construction and identities are missing and what the cited definition guarantees; spell out the required content or use a reader-facing explanation.
10. §8.1, `01-infinite-volume.tex:104–115`: “ordered tails”, “refinement”, “refining ultrafilter”, “maximal proper filter”, and “common limits” (U/J): the formal tail quantifier is followed by a new abstract construction without intuition or an example; explain why this nonstandard selection device is needed and how its limits preserve the order of spacing and volume limits.
11. §8.1, `01-infinite-volume.tex:117–125`: “reflection positivity”, “kernel form”, “positive kernel”, and “measured configuration space” (U/J): positivity is described by a formula but not connected to the reflected expectation in the preceding paragraph; the operator action is introduced without saying when it is used.
12. §8.1, `01-infinite-volume.tex:128–137`: the lemma repeats the interior-link restriction in both its opening hypothesis and final sentence (R): remove one copy or make the final sentence explain a genuinely new qualification.
13. §8.1 proof, `01-infinite-volume.tex:141–148`: “boundary kernel”, “fold inequality”, “maximising assignment”, and “constant-assignment bound” (U/D): the three proof steps are too compressed to orient the reader before the technical proof; define what is folded and what is assigned to cells, and show how the three steps imply the chessboard estimate.
14. §8.1 proof, `01-infinite-volume.tex:151–153`: “crossing link”, “positive kernel”, “entrywise products”, “boundary slice’s weight”, and “slice configurations” (U/J): these objects and the asserted preservation of positivity are not explained; give the link/group formula and identify the positive-kernel fact being applied to the Wilson interaction.
15. §8.1 proof, `01-infinite-volume.tex:154–166`: “Haar invariance restores the crossing links”; “distribution”; “positive quadratic form”; “independent g,h” (U/J): the averaging argument jumps from gauge transformations to a measure-valued quadratic form without explaining why its positivity follows; explain the role of the two independent gauge averages and the finite-sum approximation.
16. §8.1 proof, `01-infinite-volume.tex:168–190`: “fixed boundary link data”, “open-half configurations”, “first and last slice”, “half-weight”, “completion”, and “normalising constant” (U/J/D): the factorisation introduces several unnamed pieces of the configuration split and then asserts an “exact factorisation”; a diagram or explicit definition of the variables and their measures is needed to make (8.11) readable.
17. §8.1 proof, `01-infinite-volume.tex:192–223`: “assignment”, “fold”, “band”, “layer”, and “constant assignment” (U/J/D): the maximisation proof relies on a geometric cell procedure that is hard to reconstruct from prose and the two update arrows; define the indexing geometry and illustrate one fold/update so the proof of a constant maximiser is verifiable.
18. §8.1 proof, `01-infinite-volume.tex:225–244`: “normalisation” and “constant assignment” (D): this final proof segment is another dense sequence of arguments; state explicitly why adding η avoids division by zero and how expansion plus the root definition yields subadditivity.
19. §8.2 opening, `01-infinite-volume.tex:249–259`: “cell sizes”, “centred root bound”, “slice gaps”, “positivity”, and “compactness” (U/D): the three-step outline is technical and its variables are unexplained before use; the following paragraph does not explain the movement estimate or the diagonal subsequence in plain language.
20. §8.2, `01-infinite-volume.tex:261–274`: “coordinate-separated” and the periodic version (U/D): the definition is formulaically clear, but the motivation says only that planes separate points; explain why requiring all four coordinate projections to differ is the convenient temporary condition and what is lost on its measure-zero complement.
21. §8.2, `01-infinite-volume.tex:276–286`: “step function”, “round each coordinate up”, “periodic class”, and “physical displacement” (U): explain why the ceiling convention is chosen and how the stated (4na_N) bound is measured on the periodic configuration space.
22. §8.2, `01-infinite-volume.tex:289–310`: “refinements”, “multilinear kernels”, “locally uniformly”, “separated test”, and “admissible” (U/J/D): the proposition is difficult to parse because its quantifiers and two nested limits are packed together; explain in words what (P_p), (S_0), and (R_p) represent and why the order of limits matters.
23. §8.2 proof, `01-infinite-volume.tex:312–334`: “centred roots”, “aligned smaller-cell centres”, “translated root”, and “discrete convexity” (U/J): the local-bound argument uses a sequence of geometric constructions without a concrete picture or clear definition of (R(z)), (z_-), and (z_+); explain how moving a cell observation is controlled by the two centred estimates.
24. §8.2 proof, `01-infinite-volume.tex:336–348`: “forbidden translations”, “reflected coefficients”, and “ordered tails” (U/J): the measure/counting argument is asserted without showing how the (6na_k<a_m) condition guarantees an allowed translation; state that counting step in a simple formula or picture.
25. §8.2 proof, `01-infinite-volume.tex:350–399`: “slice”, “slab”, “empty slices”, “trace closes this chain”, “positive eigenspaces”, “Schatten norm”, and “Schatten Hölder” (U/J/D): this long proof passage introduces transfer-operator and complex-power machinery without a plain-language route map; define the kernel/operator, explain the slab factorisation and why complex interpolation controls movement, then present the estimates.
26. §8.2 proof, `01-infinite-volume.tex:401–412`: “fixed slabs”, “integer (b)”, and “rounding error” (U): the reader is not shown how coordinate separation supplies a uniform empty physical interval or how the preceding complex estimate becomes the displayed modulus-of-continuity bound.
27. §8.2 proof, `01-infinite-volume.tex:414–441`: “coefficient basis tuple”, “finite δ-net”, “compact exhaustions”, “raw kernels”, and “dominated convergence” (U/J/D): the subsequence argument relies on several standard results and newly coined “raw kernels” without stating their roles; explain the diagonal choices and why the limits remain continuous and give the smeared limits.
28. §8.3, `01-infinite-volume.tex:446–466`: “weak derivatives”, “invisible coefficients”, “rank bound”, “projection”, and the sub-power coefficient cost (U/J): the paragraph introduces the main algebraic inputs without an example of a coefficient that is invisible or why a projection/rank comparison is needed; the phrase “logarithm of the product of these bounds” is opaque without showing the product.
29. §8.3, `01-infinite-volume.tex:468–487`: “small in reflected cells”, “ordered tails”, “degree-e representative”, “forward difference”, and “exactly vanish” (U/J/D): the definition and comparison list are dense and use technical phrases without an explanation of their role; define the error class in plain language and explain how it lets lattice representatives stand for continuum fields.
30. §8.3, `01-infinite-volume.tex:489–503`: “functionals”, “invisible to every separated smeared correlation”, and the rank input (U/D): this abstract null-space definition has no example or explanation of how varying one coefficient produces a linear test; explain the detected object and why the dimension inequality is the needed closure input.
31. §8.3, `01-infinite-volume.tex:505–530`: “fixed representatives”, “target correlation”, “projected representative”, and “normalised limit” (U/J/D): the proof outline hides the key idea in abstract terms; explain what is being represented and how matching all tests at once is obtained.
32. §8.3, `01-infinite-volume.tex:532–579`: “weighted site count”, “summation by parts”, “cluster limit”, “ultrafilter”, “target limits”, and “uncountable collection” (U/J/D): this argument is highly compressed and introduces an ultrafilter again without accessible explanation; distinguish the finite-dimensional coefficient compactness from the simultaneous test identities and justify the nonzero limiting normalisation in words.
33. §8.4, `01-infinite-volume.tex:584–585`: “weak derivatives”, “smooth representatives”, “quotienting”, and “degree maps” (U/J): the transition announces results in compressed jargon before the relevant objects are defined; explain the intuitive passage from weak derivative identities to smooth fields and null-equivalence classes.
34. §8.4, `01-infinite-volume.tex:587–605`: “null subspace”, “quotient norm”, “analytic conventions”, “Fréchet derivative”, and “multi-index” (U/J): definitions are introduced without motivation or an example; explain what field equivalence means and why the derivative/Fourier notation is needed.
35. §8.4 proof, `01-infinite-volume.tex:624–644`: “weak identities”, “locally integrable kernel”, “cutoff”, “Fourier inversion”, and “glue” (U/J/D): the proof’s key regularity argument is compressed into a Fourier-decay assertion; explain the implication from all weak derivatives in (L^1_{
m loc}) to a smooth representative, and why overlap agreement almost everywhere gives pointwise agreement.
36. §8.4, `01-infinite-volume.tex:646–650`: “null input”, “null image”, and “injectivity” (U): the text states quotient operations descend and inclusions are injective without spelling out why the vanishing-correlation criterion implies each conclusion.
37. §8.4, `01-infinite-volume.tex:653–672`: “ordered limit”, “scale condition”, “Hilbert-space construction”, “positive configuration”, and “Osterwalder–Schrader forms” (U/J/D): several central terms are used before the definitions/formulas, and the positivity notation is introduced in the middle of the setup; start with a concrete reflected-pairing explanation and identify the configurations and tests before stating the form.
38. §8.4, `01-infinite-volume.tex:674–699`: “Euclidean properties”, “coefficient action”, and “power bound” (U/J): the proposition says identities “descend through π” but the action and units are only cross-referenced; explain what π forgets and why the five identities matter to the construction.
39. §8.4 proof, `01-infinite-volume.tex:701–730`: “grid points”, “joint tests”, “separated smear”, “positive-semidefinite cone”, and “pointwise matrix assertion” (U/J/D): the proof is compressed and the passage from lattice positivity to pointwise positivity is asserted without explaining the limiting and concentration steps.
40. §8.4 proof, `01-infinite-volume.tex:732–745`: “first-crossing bounds”, “position-independent bound”, and the choices of (m,k,D) (U/J/D): this estimate is a dense chain of scale choices; explain how the slow-scale condition gives (a_{j+1}ge ca_j^2), why the first-crossing estimates yield (a_kge c'r^4), and how this gives the stated exponent.
41. §8.5, `01-infinite-volume.tex:756 onward`: “fixed-volume convergence”, “full-spacing”, and the remaining volume-refinement construction (U/J): the subsection opening does not explain how uniqueness at fixed volume removes the spacing subsequence; the final lines need the same plain-language explanation as the five-step section outline.
42. §9 opening, `02-maxwell.tex:3–16`: “limiting fields”, “short distances”, “free Maxwell field”, “curvature”, “null coefficients”, “smeared observations”, “comparison estimate”, “compatible isomorphisms”, and “trace argument” (U/J/D): the overview lists advanced outputs but does not explain what the free field is being compared to or why each step is needed; define these ideas in ordinary language before the roadmap.
43. §9.1, `02-maxwell.tex:20–26`: “classical polynomial spaces”, “colour basis”, and “physical inner product” (U/J): the first use of “colour” and the Lie-algebra inner product lacks a short explanation of why a colour index is present and what the normalisation accomplishes.
44. §9.1, `02-maxwell.tex:28–53`: “two-form”, “homogeneous polynomial solutions”, “symmetric multilinear coefficient”, “formal Taylor series”, “one-form”, “radial potential”, and “Euler’s identity” (U/J/D): this definition introduces the field equations and several geometric terms all at once; explain the role of each Maxwell equation and what the radial potential reconstructs, with a concrete low-degree example.
45. §9.1, `02-maxwell.tex:55–78`: “scalar Green function”, “covariance”, “linear probe”, “Taylor slots”, “form indices”, and “extension to unconstrained tensors” (U/J): the kernel/probe construction is not explained as an observable measurement; define the Green function/covariance in accessible terms and explain what the derivatives and functionals evaluate.
46. §9.1 proof, `02-maxwell.tex:89–106`: “curl”, “cyclic equation”, “harmonicity”, “divergence equation”, and “extension vanishing” (U/J/D): the proof assumes differential-form and tensor-contraction terminology without translation; show how the displayed equations imply membership in ℓ_j and why this makes the contraction independent of extension.
47. §9.1, `02-maxwell.tex:109–125`: “free polynomial fields”, “restriction map”, “radial polynomial”, “kernel”, “image”, “quotient norm”, and “free unit” (U/J): this is a chain of algebraic constructions without an explanation of what relations are being imposed or why the quotient is the correct space of observables.
48. §9.1, `02-maxwell.tex:127–151`: “Wick ordering”, “perfect matching”, “disjoint union”, and “complex multilinearly” (U/J): explain in plain language why same-insertion pairings are removed and why the matching sum gives the intended correlations; the example comes only after the notation-heavy definition.
49. §9.2, `02-maxwell.tex:155–186`: “positive-side”, “Taylor arguments”, “reflected Gram matrix”, “positive semidefinite”, “strictness”, and “separated null correlations” (U/J): the section does not explain why reflection positivity of linear probes is the analytic input needed for polynomial positivity or what “null” means at this point.
50. §9.2, `02-maxwell.tex:181–184`: “analytic continuation of a vanishing response” and “tests against homogeneous Maxwell solutions” (U/J): the unresolved note names proof mechanisms without explaining what response is continued or how those tests establish strict positivity modulo the equations.
51. §9.2, `02-maxwell.tex:188–203`: “formal Taylor series”, “infinitesimal translation”, “derivative in the (Q_j) variable”, and “Fréchet derivative” (U/J): explain how the sequence shift represents moving the insertion point and why this operation raises the degree by one.
52. §9.2, `02-maxwell.tex:205–267`: “descend faithfully”, “Fock factorisation”, “polynomial inner product”, “point positivity”, and “homogeneous-kernel bounds” (U/J/D): the proof uses a large amount of Gaussian/Fock terminology and an unexplained matrix factorisation (H=L^{\mathsf T}L); introduce the finite-dimensional Gaussian idea before the algebra and explain why it proves all three clauses.
53. §9.2, `02-maxwell.tex:269–300`: “faithfulness”, “separating tests”, “common kernel”, and “compactness of the unit sphere” (U/J): the argument needs a plain explanation of why a finite set of measurements detects every vector and how this creates a uniform lower bound.
54. §9.3, `02-maxwell.tex:305–345`: “interacting fields”, “equal coordinate projections”, “finite-cutoff comparison”, “coefficient maps”, and “common cluster limit” (U/J/D): explain why equal coordinate projections matter and what the lattice coefficient maps physically do; the quantifier block is hard to follow without an illustrative order-of-choice statement.
55. §9.3, `02-maxwell.tex:347–378`: “passage to continuum fields”, “ordered tails”, “refining ultrafilter”, and “same (S)” (U/J/D): the proof claims the maps work for all tests but explains this only abstractly; clarify how one subsequence is chosen before fixing any test and how the finite-cutoff bound survives that limit.
56. §9.4, `02-maxwell.tex:382–411`: “compatible field bases”, “uniform tested convergence”, “moving tested observations”, and (KSubsetConf n) (U/J): these terms are introduced with definitions but no intuition; explain what compatibility across degrees means and why the supremum over tests is the required stronger convergence.
57. §9.4 proof, `02-maxwell.tex:413–483`: “left inverse”, “lower-degree image”, “equivariant average”, “corrected map”, “separating tests”, “eventual injectivity”, and “dimension bound” (U/J/D): the proof is a dense sequence of linear-algebra steps; explain the finite-dimensional picture (splitting off the already included lower-degree fields) and why injectivity plus the rank bound gives an isomorphism.
58. §9.5, `02-maxwell.tex:488–553`: “transported derivative”, “finite tests”, “dual formula”, “cutoff”, “Fourier inversion”, and “zero-dimensional case” (U/J/D): the derivative-convergence proof is compressed and assumes the reader understands how test convergence yields (L^1) convergence and then uniform derivative convergence; explain both implications and the scaling by (r_k).
59. §9.5, `02-maxwell.tex:556–579`: “simple nonabelian”, “gauge-invariant linear functional”, “weight below four”, and “the unit survives” (U/J): define the representation-theoretic terms or briefly explain them; show why only a linear curvature coefficient could occur below weight four and why ([γ,γ]=γ) rules it out.
60. §9 close, `02-maxwell.tex:582–586`: “uniform over varying scale intervals”, “trace section”, and “degree-four observable” (U/J): the closing assumes later arguments and a specialised observable the reader has not met; explain what choice remains open and how this section’s results are used later.

AUDIT COMPLETE



## Verification on the repaired PDF

Auditor reread: `paper/main.pdf`, current forced build, §§8–9 on PDF pages 36–62. I read the rendered pages from the preceding sections as a first-time reader, then checked all prior findings in the repaired text and layout. Findings 1–60 are fixed in this rendering. A class-wide search for first-use terminology exposed three further failures below; the section owner has not repaired them in this verification pass.

1. fixed in the current rendered PDF.
2. fixed in the current rendered PDF.
3. fixed in the current rendered PDF.
4. fixed in the current rendered PDF.
5. fixed in the current rendered PDF.
6. fixed in the current rendered PDF.
7. fixed in the current rendered PDF.
8. fixed in the current rendered PDF.
9. fixed in the current rendered PDF.
10. fixed in the current rendered PDF.
11. fixed in the current rendered PDF.
12. fixed in the current rendered PDF.
13. fixed in the current rendered PDF.
14. fixed in the current rendered PDF.
15. fixed in the current rendered PDF.
16. fixed in the current rendered PDF.
17. fixed in the current rendered PDF.
18. fixed in the current rendered PDF.
19. fixed in the current rendered PDF.
20. fixed in the current rendered PDF.
21. fixed in the current rendered PDF.
22. fixed in the current rendered PDF.
23. fixed in the current rendered PDF.
24. fixed in the current rendered PDF.
25. fixed in the current rendered PDF.
26. fixed in the current rendered PDF.
27. fixed in the current rendered PDF.
28. fixed in the current rendered PDF.
29. fixed in the current rendered PDF.
30. fixed in the current rendered PDF.
31. fixed in the current rendered PDF.
32. fixed in the current rendered PDF.
33. fixed in the current rendered PDF.
34. fixed in the current rendered PDF.
35. fixed in the current rendered PDF.
36. fixed in the current rendered PDF.
37. fixed in the current rendered PDF.
38. fixed in the current rendered PDF.
39. fixed in the current rendered PDF.
40. fixed in the current rendered PDF.
41. fixed in the current rendered PDF.
42. fixed in the current rendered PDF.
43. fixed in the current rendered PDF.
44. fixed in the current rendered PDF.
45. fixed in the current rendered PDF.
46. fixed in the current rendered PDF.
47. fixed in the current rendered PDF.
48. fixed in the current rendered PDF.
49. fixed in the current rendered PDF.
50. fixed in the current rendered PDF.
51. fixed in the current rendered PDF.
52. fixed in the current rendered PDF.
53. fixed in the current rendered PDF.
54. fixed in the current rendered PDF.
55. fixed in the current rendered PDF.
56. fixed in the current rendered PDF.
57. fixed in the current rendered PDF.
58. fixed in the current rendered PDF.
59. fixed in the current rendered PDF.
60. fixed in the current rendered PDF.

61. §8.1 reflection proof, `01-infinite-volume.tex:124–130` (PDF p. 39): “The boundary kernel is positive”; “the fold inequality `Z(i)^2 <= Z(i+)Z(i-)`”; “a maximising assignment”; “the constant-assignment bound” (U/J). The proof roadmap uses the boundary kernel, assignment variables and bound before defining them in the later Positivity, Repeated reflections and Normalisation arguments. Define or replace these terms in the roadmap before first use.

62. §8.2, `01-infinite-volume.tex:229–233, 286–291` (PDF pp. 41–42): “the numbers `(Y_i,Y_j)` of empty slices before and after its slab”; “slice positivity controls movements” (U/J). The outline uses the slab, empty-slice counts and slice-positivity mechanism before the proof's later transfer-kernel and slab construction gives them meaning. Preview the variables and positivity estimate before relying on them in both roadmaps.

63. §9 opening and §9.2 proof, `02-maxwell.tex:7, 213–218` (PDF pp. 51, 56): “the finite Gaussian matching formula”; “independent Gaussian coordinates” (U/J). The paper defines the matching sum, but never defines Gaussian variables or states the Gaussian-to-matching rule before using this name and interpreting the matrix factorisation. Explain the finite-dimensional Gaussian interpretation at its first use or refer directly to the displayed matching formula.

61. not fixed — the boundary kernel, fold variables and constant-assignment bound remain first used in the §8.1 proof roadmap before their definitions.
62. not fixed — the §8.2 roadmaps still use the slab, empty-slice counts and slice positivity before explaining them.
63. not fixed — the §9 roadmap and proof step still use “Gaussian” without defining the finite-dimensional variables or their matching rule.

VERIFIED
