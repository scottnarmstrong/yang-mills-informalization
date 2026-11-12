# Weimaraner audit of Greyhound's Round 7 section

Scope: `part2/uv/03-blocking.tex` and the proof-step conversion in §§6–7 (`part2/uv/01-lattice.tex`, `02-activities.tex`). I read the rendered pages 35–42 and the section source. The source correspondence was spot-checked against `YM/RG/Block.lean`, `YM/PCalc/Chart.lean`, and `YM/Work/F04.lean` at the pinned commit.

## Findings

1. **U/J — `03-blocking.tex:35–38`, “In the frame uniqueness region”, “route holonomy” and “centre axial gauge”.** The text introduces centre axial gauge by parallel transport, then uses “route holonomy” as the test for uniqueness without saying that this is the transport product around a closed route or linking it to the earlier walk definition. Define/link the route holonomy before using its chord to specify the uniqueness region.

2. **J — `03-blocking.tex:121`, “row-square contribution”.** This label for the term `\|\ell_W(U)_b\|^2/2` is not explained. Say what is being squared and why it is a row contribution, or replace the coined phrase with the concrete weighted path-sum square.

3. **R — `03-blocking.tex:48–49`, exact-kernel proof opening.** “The construction is a finite mixture of probability densities. The normalisation of the noise handles each tag choice; summing its likelihoods handles the mixture. Boundedness and Borel measurability follow…” restates the three numbered steps and the proposition conclusion. Remove the proof summary or retain only a distinct idea that the steps then develop.

4. **R — `03-blocking.tex:158–161`, local stationary-branch proof.** The opening says that the positive lower bound makes the vertical Hessian invertible and the implicit function theorem gives the branch; Step 1 repeats that entire argument. Keep the explanation once, in the substantial step.

5. **S — `03-blocking.tex:185–187`, volume-independent stationary ball.** This is a long proof but has no `\\proofstep`. Structure it into substantial steps as required by C6.

6. **D — `03-blocking.tex:185–187`, proof of the volume-independent radii.** The prose jumps from “the exponential distance sum is finite” to dimension-independent derivative norms and then to three radii and coordinate decay. Show the uniform lattice sum that uses the `K_0` occupancy bound, and state which derivative bounds feed the quantitative implicit-function estimate and how the radii are ordered. The current prose does not let a reader check the uniformity asserted in `eq:uv-uniform-radii`.

7. **U — `03-blocking.tex:176–182`, `r_{\\rm safe}`.** The proposition includes this third radius, but its role is not stated in the conclusion: uniqueness and the branch bound use `r_{\\rm zone}`, and the analytic domain uses `r_{\\rm hor}`. Explain what the safe radius controls or remove the unused parameter if it is not part of the intended source statement.

8. **J/U — `03-blocking.tex:201`, “common tag-branch condition” and “positive local chart ratio”.** These are listed as forest-comparison hypotheses without explaining what equality/ratio they describe. State that the same tag choices have the required local critical branches and define the chart ratio as the ratio of the two local Haar densities (with its positivity condition), or link to a displayed definition.

## Class S sweep of §§6–7

I searched both older UV sections and the new section for the former `enumerate[Step]`, `\\item \\emph{...}` and prose-labelled `Step n` forms. The converted lists in §§6–7 use the prescribed `\\proofstep` macro; the numbered lists in the activity-construction paragraph are a list of missing construction tasks, not proof stages. The long unnumbered proof in finding 5 is the remaining C6 failure identified in this sweep.

The class U/J/R/D/S findings above are to be read as failure classes and checked throughout the owner's text during repair, per RULES.md A0. Source-correspondence concerns not stated as findings are not a claim that the new section proves the full construction; its explicit gaps remain visible.

AUDIT COMPLETE

## Rendered-PDF verification of Greyhound's repairs

I reread the repaired section in the current rendered `main.pdf`, pages 37–43, against each finding and `r7-greyhound-response.md`.

1. **Fixed.** Page 37 defines route holonomy as transport around a closed walk in the centre axial gauge, links the walk convention, and explains the chord.
2. **Fixed.** Page 39 replaces the coined “row-square contribution” with the direct plaquette action and squared norm of the weighted path sum.
3. **Fixed.** Page 38 begins the exact-kernel proof directly with its three substantive steps; the redundant opening summary is gone.
4. **Fixed.** Page 40 begins the local stationary-branch proof with Step 1; the repeated implicit-function explanation is gone.
5. **Fixed.** Pages 41–42 divide the volume-independent stationary-ball proof into two substantial proof steps.
6. **Fixed.** Page 41 displays the uniform lattice sum using the `K_0` occupancy bound and derives coordinate-row bounds; pages 41–42 state the inverse-Hessian input, its role, and the ordered radii. The response correctly keeps the source-specific inverse-bound proof explicit as unresolved.
7. **Fixed.** Page 42 identifies `r_safe` as the safe ball for strict convexity and the uniform inverse bound, with the branch zone inside it.
8. **Fixed.** Page 42 defines the common tag-branch condition and the local chart ratio, including its positivity condition.

**New failures:** None observed in the rendered section pages inspected (37–43).

VERIFIED
