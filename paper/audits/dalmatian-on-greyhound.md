# Dalmatian audit of Greyhound's UV sections

Rendered review: `paper/main.pdf`, pages 19–34 (PDF timestamp 2026-11-12 06:48:47 UTC). I read the preceding Part I and then the assigned sections as a first-time reader. Locations below give the source lines and rendered page.

1. §6.1, `paper/part2/uv/01-lattice.tex:36–40` (PDF p. 19): “For a walk from~$x$ to~$z$” — **U**. Definition 6.1 names the start and successive sites $x_0,ldots,x_r$, but never identifies $x=x_0$ and $z=x_r$; the endpoints in the covariance formula are therefore unnamed.
2. §6.3, `paper/part2/uv/01-lattice.tex:249–252` (PDF p. 23): “The linear map making this choice for every~$v\in V_d$ is called a local section.” — **J**. “Section” is unexplained terminology here; say what choice the map makes in ordinary language, or explain the mathematical meaning of calling it a section.
3. §6.3, `paper/part2/uv/01-lattice.tex:291–306` (PDF pp. 23–24): “For a fixed real jet, $B$ is polynomial in~$\varepsilon$ … since~$G$ is closed, the links … are group valued.” — **D**. This is a run of several distinct arguments (convergence, analyticity, uniqueness, and group membership) with no enumerated steps or displayed conclusion for each; structure the proof idea and separate the checks.
4. §7.1, `paper/part2/uv/02-activities.tex:15–17,23–28` (PDF p. 27): “the curvature averaged over its square”; “extracts the leading curvature” — **U**. Curvature of the connection has not been defined. Give its formula or explain the object, and then explain how the displayed linearisation represents its square average.
5. §6.4, `paper/part2/uv/01-lattice.tex:348–358` (PDF p. 25): “Let~$\theta_N>0$ be the threshold that will distinguish small plaquette distances~$\chi$ … in the later estimates.” — **U**. The threshold is introduced without a rule or required relation that determines it; the reader cannot tell which distances count as small or how this parameter is chosen.
6. §6.4 proof, `paper/part2/uv/01-lattice.tex:412–415` (PDF p. 26): “In particular, the dependencies are” followed by the insertion formula — **R**. This repeats exactly the definition in (6.23); it neither lists dependencies nor adds a new consequence.
7. §6.4, `paper/part2/uv/01-lattice.tex:435–441` (PDF p. 26): “the requirements~Reg2–Reg4 are satisfied …; the reference unit is …” and then “The invertible coefficient transfers … must still be constructed” — **R**. The paragraph repeats Proposition 6.12's conclusions, while the unresolved paragraph repeats the outstanding transfer construction again in the opening of §7 (02-activities.tex:11). Keep the result and the remaining obligation once in the appropriate place.
8. §7.3, `paper/part2/uv/02-activities.tex:258–260` (PDF p. 31): “carry one insertion through an identity of weights” — **J**. “Identity of weights” is not explained; identify the weight as the function being integrated and state what identity is being carried through.
9. §7.3, `paper/part2/uv/02-activities.tex:328–337` (PDF p. 32): “These identities explain why an inserted observable must be integrated together with its weight.” — **U**. The displayed identities are pointwise coefficient-extraction formulas and contain no integration; show the corresponding integral identity or explain the extra integration step.
10. §7.4, `paper/part2/uv/02-activities.tex:350–363` (PDF p. 32): “let~$\mathbb B_{\ell,B}(a)$ be its closed ball” and then again “$\mathbb B_{\ell,B}(a)=\{x\in\Lambda_\ell: d_\ell(x,a)\le B\}$” — **R**. The ball is defined twice in the same definition; retain one definition and use the other line for the cover number.
11. §7.4, `paper/part2/uv/02-activities.tex:372–379` (PDF p. 32): equation (7.22) uses “$U\in\mathcal E_j$” before the next sentence, “The optional extra condition~$\mathcal E_j$ is Borel and gauge invariant.” — **U**. Define the extra condition before it appears in the eligibility formula and state what it restricts.
12. §7.4, `paper/part2/uv/02-activities.tex:372–379` (PDF p. 32): “nonempty sets~$I_j\subseteq Y_j$” and equation (7.22), followed by “Thus~$I_j$ specifies the exact bad sites” — **U**. The role of $I_j$ is explained only after it is used to restrict $K_j$; identify it before the formula.
13. §7.4, `paper/part2/uv/02-activities.tex:377–389` (PDF pp. 32–33): “the internal links of~$Y_j$” — **L**. Link this support notion to Definition 2.6, which defines support by requiring both link endpoints to lie in the site set; the phrase is reused here without that reference or explicit meaning.
14. §7.4, `paper/part2/uv/02-activities.tex:404–415` (PDF p. 33): “Let~$c\in\mathbb R$, and let~$S$ be the part of the action kept separate from the activities” — **U**. The role of the free constant $c$ in the exponential is not explained; say what it normalises or why it is included.
15. §7.4, `paper/part2/uv/02-activities.tex:470–472` (PDF p. 34): “impose the required conditions on their values and quadratic Taylor coefficients at~$U(e)=1$” — **U**. The identity configuration $U(e)=1$ and the meaning and purpose of these quadratic coefficients have not been introduced; explain them or link to their definition.

16. §6.2, `paper/part2/uv/01-lattice.tex:153–156` (PDF p. 21): “radial gauge: its component in the radial direction vanishes” — **U**. The reader has not been told what vector is radial or how to test this condition until equation (6.11); give the condition $z\cdot A(z)=0$ at first use.
17. §6.2, `paper/part2/uv/01-lattice.tex:170–174` (PDF p. 21): “Taylor coefficients, with the factorial normalisation” — **U**. No coefficient convention is specified (for example, the factor $1/(j+1)!$ in the degree-$(j+1)$ term); state the normalisation rather than naming it.
18. §6.2, `paper/part2/uv/01-lattice.tex:243–245` (PDF p. 23): “their null relations” — **U/J**. No null relation has been defined; explain that these are polynomials whose limiting correlations vanish against every test, so the quotient can be formed.
19. §6.2, `paper/part2/uv/01-lattice.tex:217–225` (PDF p. 22): “Conjugation acts linearly within each~$\mathcal A_j$” — **U**. “Conjugation” could mean coefficient conjugation or the simultaneous matrix action $A_j\mapsto\operatorname{Ad}(g)A_j$ defined above; name the latter explicitly.
20. §6.3, `paper/part2/uv/01-lattice.tex:333–335` (PDF p. 24): “derivative estimates needed for the later blocking argument” — **J**. “Blocking” has not been explained in the paper; say that the estimates are used when variables are integrated in groups to pass between lattice spacings.
21. §6.4, `paper/part2/uv/01-lattice.tex:386–388` (PDF p. 25): “$U(\cdot+z)$” — **U**. The translated configuration is not defined; specify its link values (or refer to the translation case $A(y)=y+z$ of Definition 6.2).
22. §7 opening, `paper/part2/uv/02-activities.tex:9–11` (PDF pp. 26–27): “local activity bounds” and “activity sums” — **U/J**. “Activity” first appears here, before §7.4 defines it; give the promised plain definition in this outline so the roadmap is understandable on arrival.
23. §6.1, `paper/part2/uv/01-lattice.tex:59–63` (PDF p. 20): “the pullback~$A^*U$ reads the transport along the image of each positive link” — **U/D**. This is the only definition of the coordinate action, but it does not say how the link value is computed when the image is reversed; give a formula or a concrete positive/reversed-link case before relying on it in the invariance proof.
24. §6.1 proof, `paper/part2/uv/01-lattice.tex:121–130` (PDF p. 21): “the positive-axis base of the image square” and “face indices” — **J/U**. These invented labels are not explained; say directly which base site and which plaquette labels are permuted by the signed permutation.
25. §6.2, `paper/part2/uv/01-lattice.tex:160–168` (PDF p. 21): “homogeneous polynomial one-forms of degree~$j+1$” — **U**. The definition does not explain that each coefficient $A_{j,\mu}(z)$ is a homogeneous polynomial of that degree; add this in words so the reader can interpret (6.11).
26. §6.2, `paper/part2/uv/01-lattice.tex:170–172` (PDF p. 21): “diagonal evaluations of symmetric~$(j+1)$-linear maps” — **J**. This technical equivalence is not explained and does not clarify the chosen Taylor convention; replace it with a brief example or remove the aside after stating the convention.
27. §6.2, `paper/part2/uv/01-lattice.tex:243–245` (PDF p. 23): “a limiting correlation table and its null relations” — **U/J**. “Correlation table” is another unnamed object here; say which limits are arranged in it, or replace the phrase with “the limiting correlations.”
28. §6.3, `paper/part2/uv/01-lattice.tex:249–252,312–335` and §7.2, `paper/part2/uv/02-activities.tex:130–133,175–177` (PDF pp. 23–24, 27, 29): “local section”, “normalised local section”, and “sections~$P_d$” — **J**. These repeat the undefined construction name across both sections; consistently call $P_d$ the map assigning a link polynomial to each classical polynomial, or explain “section” at its first use and retain that explanation at later uses.
29. §6.4, `paper/part2/uv/01-lattice.tex:339–343` (PDF p. 24): “different classical observable polynomials can mix” — **J**. “Mix” is not explained in this setting; state that integration can make the coefficient of one polynomial depend on several fine-scale coefficients.
30. §6.4, `paper/part2/uv/01-lattice.tex:365–371` (PDF p. 25): “maps from coefficients at the finest level~$N$ to coefficients at level~$j$” — **U**. No intermediate coefficient lists or rule producing them are defined; make clear these maps are assumed data for this definition and that their construction remains open, rather than describing them as already given levels.
31. §6.4 proof, `paper/part2/uv/01-lattice.tex:407–415` (PDF p. 26): “In particular, the dependencies are” — **J**. The displayed equation repeats (6.23) and does not state dependencies; delete it or state the actual input variables the insertion depends on.
32. §7.1, `paper/part2/uv/02-activities.tex:44–45` (PDF p. 27): “rather than a logarithm of a single plaquette” — **J**. Matrix logarithms have not been introduced, and the contrast does not explain why several plaquettes are used; state the reason in terms of the measurements needed to recover all Taylor coefficients.
33. §7.1 proof, `paper/part2/uv/02-activities.tex:114–116` (PDF p. 28): “preserves~$\operatorname{ran}B$ … Its orthogonal projection~$\Pi$” — **U**. Define $\operatorname{ran}B$ as the range of $B$ and state explicitly that $\Pi$ projects onto that subspace before using it.
34. §7.2 proof, `paper/part2/uv/02-activities.tex:195` (PDF p. 29): “makes the Taylor polynomial reproduce the identity through degree~$d$” — **U**. It is unclear whether “identity” means the identity map on jets or the constant observable $1$; say explicitly that $R_d^{[d]}\mathcal Q_d(J)$ agrees with $J$ through order $d$.
35. §7.2 proof, `paper/part2/uv/02-activities.tex:207–209` (PDF p. 30): “The final polynomial is not truncated again.” — **J**. “Truncated” has no stated referent here; explain which Taylor polynomial is truncated and why later composition is left as an exact polynomial.
36. §7.2, `paper/part2/uv/02-activities.tex:252–254` (PDF p. 31): “regular activities below” — **L**. “Regular activities” are defined later in §7.4; identify that forward reference or describe the future use without introducing the term as though already defined.
37. §7.3, `paper/part2/uv/02-activities.tex:328–335` (PDF p. 32): “let~$J$ be a finite index set” — **U/J**. $J$ has denoted the real jet throughout §§6–7.1; reuse of the same letter for an index set makes the insertion formula harder to follow. Rename the index set and keep the jet notation distinct.
38. §7.3, `paper/part2/uv/02-activities.tex:276–277` (PDF p. 31): “quotient of~$\C[\zeta_v:v\in V]$ by those monomials” — **J**. This algebraic shorthand is not explained and is unnecessary after the multiplication rule; either name the excluded monomials and explain the quotient, or omit the aside.
39. §7.4, `paper/part2/uv/02-activities.tex:341–348` (PDF p. 32): “After integration over a scale, the effective weight is a sum of interactions on finite regions. Where all nearby plaquettes are small…” — **U/D**. “Scale”, “effective weight”, “nearby” and “small” precede their precise meaning and make the four-sentence outline hard to picture; state which variables are integrated, what function results, and connect “small” to the threshold test already defined.
40. §7.4, `paper/part2/uv/02-activities.tex:345–348` (PDF p. 32): “The support weight will measure … the cost of joining its separated pieces.” — **U/J**. The “cost” is not an actual cost but the exponential of the number of covering balls; explain that concrete counting interpretation before Definition 7.4.
41. §7.4, `paper/part2/uv/02-activities.tex:377–389` (PDF pp. 32–33): “Both~$K_j$ and~$\mathcal E_j$ depend only on the internal links of~$Y_j$” — **L/U**. Cite Definition 2.6 and state explicitly that these are links whose two endpoints lie in $Y_j$; “internal links” has no definition of its own.
42. §7.4, `paper/part2/uv/02-activities.tex:389` (PDF p. 33): “Two of the regions~$Y_j$ may occur together only when they are disjoint; this condition uses~$Y_j$, while~$\widehat Y_j$ contains the endpoints…” — **D/U**. The distinction is stated before the selection formula and without saying why overlaps of inspected supports are allowed; connect the statement to the pairwise-disjoint condition in (7.25) and explain the role of $\widehat Y_j$.
43. §7.4, `paper/part2/uv/02-activities.tex:404–415` (PDF p. 33): “$\rho(U)=\exp( c|\Lambda_\ell|-S(U)-E_t(U))\mathcal Z_K(U)$” — **U**. The text calls $\rho$ a weight but does not say whether it is a probability density or an unnormalised factor; explain what its later use is and how $c$ affects its volume normalisation.
44. §7.4, `paper/part2/uv/02-activities.tex:432` (PDF p. 33): “integrable against product Haar” — **L**. This reuses the product reference measure without a link; refer to the product Haar measure in Definition 2.4 / equation (2.4).
45. §7.4, `paper/part2/uv/02-activities.tex:470–472` (PDF p. 34): “The integration over a scale and subsequent regrouping must still construct those activities” — **R/J**. This repeats the open construction statement at the start of §7 (lines 7–11) and uses “regrouping” without saying what is grouped; consolidate the open obligation and state which terms are collected by region.

AUDIT COMPLETE (second pass)

## Verification on the repaired PDF

Rendered review: `paper/main.pdf`, pages 19–35 after the round-6 build. I reread both assigned UV sections against the preceding pages and checked each original finding in the rendered text and layout.

1. fixed (p. 20): walk start and endpoint are explicitly `x=x_0` and `z=x_r` before the covariance formula.
2. fixed (p. 24): “local representative map” names the choice and explains its input, output, support and Taylor condition.
3. fixed (pp. 24–25): transport convergence, uniqueness, approximation by group-valued products and closedness of `G` are four separate steps.
4. fixed (p. 28): curvature is defined by its component formula; the commutator is identified as quadratic and the plaquette first variation as a square average of linear curvature.
5. fixed (p. 26): `theta_N` is only a factor-rescaling parameter; the independent plaquette cutoff `t` is referenced.
6. fixed (p. 26): the repeated insertion formula is absent from the proof.
7. fixed (pp. 26–27): the transfer construction remains an explicit open task at its definition; it is not restated as a duplicate in the activity-section introduction.
8. fixed (p. 33): the square-zero variable marks one observable in the weighted product.
9. fixed (p. 33): coefficient extraction is followed by the integral identity, including its integrability condition.
10. fixed (p. 34): the ball is defined once; the display defines the connected-cover number.
11. fixed (p. 34): optional `E_j` is introduced as a Borel gauge-invariant condition before the activity eligibility implication.
12. fixed (p. 34): `I_j` is identified as the exact nonempty set of required bad sites before the formula.
13. fixed (p. 34): internal links are tied to Definition 2.6 and explicitly require both endpoints in `Y_j`.
14. fixed (p. 35): the constant `c` is explained as a per-site term giving the factor `e^{c|Lambda_ell|}`.
15. fixed (p. 35): the identity configuration and exponential coordinates for its quadratic Taylor terms are defined.
16. fixed (p. 22): radial gauge is given by the radial-vector condition `z·A(z)=0` before its use.
17. fixed (p. 22): the Taylor coefficient factorial convention and first-degree example are stated.
18. fixed (p. 23): null relations are described as polynomials invisible to every allowed limiting correlation.
19. fixed (p. 23): simultaneous matrix conjugation is distinguished from coefficient conjugation.
20. fixed (p. 25): “blocking” is replaced by integrating link variables in groups between lattice spacings.
21. fixed (p. 26): the translated configuration is defined by its link values before the covariance identity.
22. fixed (p. 27): an activity is introduced as a scalar function attached to a finite site region; the later roadmap links back to it.
23. fixed (p. 20): the coordinate action specifies both positive and reversed image links, including inversion and shifted start.
24. fixed (p. 21): the image square base site and pair of directions are specified, giving a plaquette bijection.
25. fixed (p. 22): each component `A_{j,mu}` is stated to have homogeneous degree `j+1`.
26. fixed (p. 22): the factorial convention and its degree-zero example replace the unexplained diagonal-evaluation aside.
27. fixed (p. 23): the continuum spaces are described as limits modulo polynomials with zero tested limiting correlations.
28. fixed (pp. 24–26): the undefined “section” terminology is replaced consistently by the described local representative map.
29. fixed (p. 26): the earlier “mix” shorthand is replaced by the concrete dependence of a classical coefficient on several fine-lattice coefficients.
30. fixed (pp. 26–27): coefficient transfers are identified as intended data whose construction for this Wilson family remains open.
31. fixed (p. 26): the spurious dependency display is removed; locality is already explicit.
32. fixed (p. 28): the reason for several plaquette measurements is stated as recovering all coefficients.
33. fixed (p. 29): `ran B` and the orthogonal projection onto it are defined.
34. fixed (p. 31): the recovery composition is said to agree with the identity through the required Taylor order.
35. fixed (p. 31): only the recovery map is Taylor-truncated; the composed link polynomial is kept in full.
36. fixed (p. 32): later regular terms point back to their definition in Subsection 7.4.
37. fixed (p. 33): `I` names the auxiliary variable set, leaving `J` for a real jet.
38. fixed (p. 33): associativity is explained directly by disjoint variable sets.
39. fixed (pp. 34–35): scale integration, effective weight, good configurations and retained bad-site contributions are described before use.
40. fixed (p. 34): the support weight is explained as a factor per ball in a smallest connected cover.
41. fixed (p. 34): internal links are defined by the two-endpoint support convention.
42. fixed (p. 35): the activity formula distinguishes disjoint selected regions from possibly overlapping inspected link sets.
43. fixed (p. 35): `rho` is identified as an unnormalised scalar factor, not a probability density.
44. fixed (p. 35): integrability is linked to the product Haar measure of Definition 2.4.
45. fixed (p. 35): the remaining construction task lists scale integration, collection by finite region and degree-two identity-coordinate conditions.

No new failures were found in the rendered reread. The repaired text preserves the outstanding mathematical obligations rather than claiming them proved.

VERIFIED
