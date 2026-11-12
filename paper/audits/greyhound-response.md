# Greyhound response to Dalmatian's audit

I compared both owned ultraviolet sections with `origin/amelie/paper:paper/part2/uv/01-lattice.tex` and `.../02-activities.tex`, then reviewed every delta against findings 1–45. I retained the exposition repairs that match the source definitions and the paper's open proof obligations. I corrected one mathematical overstatement: a smooth connection has a formal Taylor series, which need not converge to the connection. No statement, hypothesis, label, or source claim was added or removed.

## Finding-by-finding changes

1. **UV01:** Identified the walk's start and endpoint as `x=x_0` and `z=x_r` before the covariance formula.
2. **UV01, UV02:** Replaced “local section” with “local representative map”; defined its input, output, finite link support and Taylor requirement at first use and used the term consistently.
3. **UV01:** Split the transport-series argument into four checks: local uniform convergence and analytic dependence, uniqueness, approximation by group-valued products, and closedness of `G`.
4. **UV02:** Defined curvature by its component formula and explained that the commutator term is quadratic, so first variation of a plaquette gives the square average of the linear curvature.
5. **UV01:** Clarified that `theta_N` is a factor-rescaling parameter in the insertion formula. The plaquette smallness test uses the separate cutoff `t`.
6. **UV01:** Removed the repeated insertion formula from the locality proof; the proof now draws locality and translation covariance from the defining formula.
7. **UV01, UV02:** Kept the same-family coefficient-transfer construction as an explicit open obligation at its definition and removed its duplicate from the UV02 roadmap. Distinct obligations for the running condition, moment convergence and activity construction remain at their relevant locations.
8. **UV02:** Replaced the unexplained “identity of weights” wording with the concrete square-zero marker `1+zeta I` for one observable in a weighted product.
9. **UV02:** Added coefficient-extraction identities under integration, for one insertion and a finite product, with integrability stated.
10. **UV02:** Defined the closed ball once and used the display only to define the connected-cover number.
11. **UV02:** Introduced the optional Borel, gauge-invariant condition `E_j` and its role before the eligibility implication.
12. **UV02:** Explained before the formula that `I_j` is the exact nonempty set of required bad sites in `Y_j` whenever `K_j` is nonzero.
13. **UV02:** Linked “internal links” to the observable support convention and stated that both endpoints lie in `Y_j`.
14. **UV02:** Explained that `c` is a per-site constant and contributes `exp(c |Lambda_ell|)` to the weight.
15. **UV02:** Defined the identity configuration and the exponential link coordinates used to state the deferred degree-two Taylor conditions.
16. **UV01:** Defined radial gauge at first use by `sum_mu z^mu A_mu(z)=0`, identifying the radial vector.
17. **UV01:** Stated the factorial convention for each Taylor coefficient and added a first-degree example. On review against the smoothness hypothesis, changed “the Taylor series is” to “the formal Taylor series is”; no convergence is asserted.
18. **UV01:** Explained null relations as polynomials whose limiting correlations vanish against every allowed test.
19. **UV01:** Distinguished simultaneous matrix conjugation `A_j -> Ad(g) A_j` from coefficient conjugation.
20. **UV01:** Replaced “blocking argument” with the later operation of integrating link variables in groups to pass between lattice spacings.
21. **UV01:** Defined the translated configuration by its link values before translation covariance is used.
22. **UV02:** Introduced an activity in the opening as a scalar function attached to a finite site set and linked later uses to that definition.
23. **UV01:** Gave the coordinate-action formula for both positively oriented image links and reversed image links, including inversion and the shifted initial vertex.
24. **UV01:** Replaced unexplained face-index wording with the image square's base site and direction pair, and stated the resulting plaquette bijection.
25. **UV01:** Specified that every component `A_{j,mu}` is homogeneous of total degree `j+1`.
26. **UV01:** Replaced the unexplained diagonal-evaluation aside with the explicit factorial convention and example.
27. **UV01:** Replaced “correlation table” with limiting lattice correlations and explained the quotient by invisible polynomials.
28. **UV01, UV02:** Replaced the undefined “section” terminology throughout prose and proposition titles; stable equation labels remain unchanged.
29. **UV01:** Replaced “mix” with the concrete dependence of a classical coefficient on several fine-lattice coefficients after integration.
30. **UV01:** Made the intermediate coefficient maps assumed data intended to carry coefficients through successive integrations, and stated that their construction for the Wilson family remains open.
31. **UV01:** Removed the duplicate equation incorrectly introduced as “dependencies”; the locality argument already specifies the inputs.
32. **UV02:** Explained why multiple plaquettes are used: their combined measurements recover all Taylor coefficients through the fixed degree.
33. **UV02:** Defined `ran B` as the range `{B J : J in J_d}` and `Pi` as its orthogonal projection.
34. **UV02:** Clarified that the recovered composition agrees with the identity on jets through order `d` at zero.
35. **UV02:** Specified that only the recovery map is Taylor-truncated; after composition with the observable, the full link polynomial is retained.
36. **UV02:** Linked the forward reference to “regular terms” to their definition in the local-interactions subsection.
37. **UV02:** Renamed the finite index set `J` to `I`, preserving `J` for the real jet.
38. **UV02:** Removed the unexplained polynomial-quotient aside and explained associativity using disjoint variable sets.
39. **UV02:** Explained scale integration as integrating links at one spacing to obtain a function of the remaining links; tied “good” to `chi(U_p) <= t` and described how large-plaquette terms retain their sites.
40. **UV02:** Explained the support weight as the number of balls in a smallest connected cover, with a factor `exp(alpha)` per ball.
41. **UV02:** Defined internal links using the two-endpoint support convention.
42. **UV02:** Connected pairwise disjointness to the selected regions `Y_j` and explained why the larger inspected sets `hat Y_j` may overlap.
43. **UV02:** Identified `rho` as an unnormalised factor intended for integration, not a probability density; explained its volume factor with `c`.
44. **UV02:** Linked integrability to the product Haar measure in Definition `def:wilson-law` and equation `eq:wilson-law`.
45. **UV02:** Consolidated the remaining activity-construction obligation and stated its steps: integrate one spacing, collect terms by finite site region, and verify the degree-two identity-coordinate conditions and bounds.

## Generalised searches and fixes

- **U:** Searched both sections for object and symbol first uses, including walk endpoints, Taylor/radial-gauge data, intermediate maps, translations, activity inputs, bad-site sets, inspected supports and identity coordinates. Added definitions or local explanations before use; kept the transfer and activity constructions visibly open.
- **R:** Searched for repeated defining formulas and repeated construction obligations. Removed the duplicate insertion formula, the duplicate ball definition, and repeated transfer/scale-construction statements; retained distinct outstanding obligations where their consumers differ.
- **J:** Searched both sections for “section”, “blocking”, “mix”, “logarithm”, “cost”, “internal links”, and related support and construction terminology. Replaced shorthand with the concrete maps, integrations, measurements, link sets and counting factors.
- **D:** Rechecked the long proofs and displays in both sections. The transport, sampling, section construction, marker algebra, activity summation and deferred activity-construction steps are separated and their key estimates displayed.
- **L:** Checked reused support and measure conventions across both sections. Linked internal links and product Haar to their existing definitions and linked the later regular-term reference to its definition.

## Build and ownership check

The `enumerate` opened at UV02 line 432 is closed at line 436. A forced `latexmk -g -pdf -interaction=nonstopmode main.tex` completed successfully after the formal-series correction. The current PDF has 63 pages. Its only log warning is the empty bibliography; the source still explicitly identifies the same-family transfer and activity constructions as open.

REPAIR COMPLETE
