# Feedback, round 4 (from Amélie, after reading checkpoint 4)

All three agents read this whole file. Rounds 1–3 still hold in full. Rules marked **(standing)** hold for every
later round and every new section.

## 1. The main theorem is too long (dalmatian)

Theorem `thm:main` (`part1/03-theorem.tex`) should be **shorter**. We do not have to be overly explicit inside the
theorem: the definitions it links to carry the details. Examples:

- "The continuation $\mathsf F_n$ is holomorphic in ordered complex times, equals $S^{\xi_*}$ at ordered imaginary
  times, and has the selected vacuum expectations as its boundary values tested against products of Schwartz
  functions." is too long.
- "These assertions have exactly the domains and quantifiers in~\ref{recon:1}--\ref{recon:15} of
  Definition~\ref{def:reconstructed}." is not required.

Each of P1–P4 should be a short, readable statement: the key formula where there is one (the ordered limit, the
mixture identity, the trace law), and otherwise a sentence that says what holds with a link to the definition
that makes it precise. Keep the quantifier structure (for every $G$, there is $\W$; for every $p$, there are $q$ and
a hierarchy) and the links. Do not change what is claimed.

## 2. Proof ideas: structured, enumerated, with mathematics (standing)

Amélie likes the ideas, but they must be **structured better**:

- **Enumerate the steps** of a proof idea (Step 1, Step 2, … or an enumerated list).
- **Use more mathematics to express the ideas**: a short display or formula for each step is often clearer than a
  sentence. Words carry the intuition; the formula shows what is meant.

Example to rewrite (Part I, the idea of the proof of Proposition `prop:limit`, `part1/05-propositions.tex`):

> Reflection positivity bounds an average of several separated observables by averages of reflected copies of each
> individual observable. The ultraviolet estimates bound these individual averages independently of box size.
> Integrating between successive lattice slices controls changes in the correlations when their points move […]
> The average state is split into phases by examining observables separated by a very long time. […]

Rewrite it as enumerated steps, each with its formula (for instance, the chessboard bound as an inequality, the
equicontinuity estimate, the projection $e^{-tH}\to P_0$ as $t\to\infty$, the commutation of the limiting operators,
the mixture identity). Do the same for **all five** proof ideas in Part I and for every proof idea in Part II.

## 3. Proofs: more mathematics, fewer sentences (standing)

Example: the proof of Proposition `prop:iv-euclidean` (`part2/limit/01-infinite-volume.tex`, around line 690):

> Exact lattice symmetries and unit identities pass at grid configurations […] and grid translations. Density and
> continuity give these identities throughout $\Conf n$ […] For reflection positivity, fix finitely many joint
> tests […] Normalised smooth bumps concentrating at fixed positive configurations give point reflection
> positivity.

This is a sequence of sentences. Write it with mathematics: state what is being shown for each property, display
the identity or inequality at the lattice level, display its limit, and say in one line why the limit passes.

## 4. Undefined words are still there (standing)

In the proof of Lemma `lem:iv-reflection` (`part2/limit/01-infinite-volume.tex`, lines 140–181):

- **"crossing links"**: defined only in passing on line 151, after first use on line 150. Define them before use,
  with a formula (the links $\{x,x+a_Ne_\mu\}$ with $x$ and $x+a_Ne_\mu$ on opposite sides of the reflection plane).
- **"Interiority"**: what does it mean? Not explained. Define it or replace it with plain mathematics.

## 5. Consistency (everyone)

Amélie asks whether the principles of the previous rounds (no jargon, no redundancy, every object clearly defined and
explained, ideas before technicalities, mathematics instead of sentences) have been applied **consistently
throughout the file**. The examples above show they have not. The symbol tables of round 3 checked definitions,
but not density, structure or jargon in proofs.

This round, each agent rereads **every paragraph** it owns, start to finish, as a first-time reader, against all
four feedback files, and fixes every passage that fails. In your notes, keep a list of the passages you changed
for this reason (section, line, what was wrong). dalmatian, as editor, then rereads all of Part II for the same
faults and sends concrete requests.

## This round (round 5)

**Revision only**: no new sections.

- **dalmatian**: §1 (the theorem); §2 for all five Part I proof ideas and the Part II opening; §5 for Part I; then
  the editorial read of Part II.
- **greyhound**: §§2–5 for Lattice fields and Polymer activities.
- **weimaraner**: §§2–5 for Infinite volume and the Maxwell comparison, including the proof of
  `prop:iv-euclidean` and Lemma `lem:iv-reflection`.

Everyone: build, reread the rendered PDF, write `paper/reports/<name>-5.md` (at most one page, including the list of
§5 changes in summary), and **stop and wait**.
