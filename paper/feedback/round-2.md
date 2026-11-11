# Feedback, round 2 (from Amélie, after reading checkpoint 2)

All three agents read this whole file. `feedback/round-1.md` still holds in full.

## Overall

**Part I is beautiful. This is exactly the style we need, and the structure is great.** Part I is now the
reference for the style of the whole paper. Part II does not yet reach it, and needs some restructuring.

## Small fixes (dalmatian)

- **No `\clearpage` before a new section.** Remove them (a new *part* may still start on a new page).
- **Delimiters must be sized to their contents** so the formula renders nicely. Example, `part1/02-setting.tex`
  line 382: write
  `S^{\xi_*}\Bigl((4,\Theta),(4,\Theta);-\frac{r}{2}e_4,\frac{r}{2}e_4\Bigr)\,.`
  instead of `S^{\xi_*}((4,\Theta),(4,\Theta);-\frac{r}{2}e_4,\frac{r}{2}e_4)\,.` Check every display in the paper for
  the same problem (brackets around fractions, sums, integrals, tall subscripts).
- Rename the files of `part1/` so that their names and order match the sections they contain.

## Part II: what is wrong, for everyone writing it

1. **Too dense.** Two passages that fail:
   - in Lattice fields: "Probability Haar measure on a compact group is invariant under right translations and
     inversion as well as left translations. For example, its image under a fixed right translation is again left
     invariant …";
   - in Infinite volume: "A fold replaces the observables on one half of the torus by reflected copies of those on
     the other half. Cauchy--Schwarz bounds the square of the absolute expectation of a mixed cell assignment …".

   These are walls of sentences. Use mathematics to describe and support the intuitive ideas written in the text:
   say the idea in words, then show it in a display, not the reverse and not words alone.
2. **A proof needs intuitive ideas explained first, then the mathematics that carries them out.** Every proof of
   more than a few lines starts with its idea in plain words; then the steps, with displays.
3. **Too much jargon, everywhere.** Remove it. If a term is not standard, either replace it by plain mathematics
   or define and explain it. Do not coin new words.
4. **Remove redundancies.** Say each thing once. We want it as clean and clear as possible.
5. **A strategy and a reading guide are missing.**
   - **Part II as a whole** needs an opening: what is going on in the construction, how its sections fit together,
     and how to read it. Model it on the strategy section of Part I.
   - **Each section** (Lattice fields, Infinite volume, and every new one) opens with an outline: what the section
     does, why, what follows, and how it is structured.

## This round (round 3)

- **dalmatian**
  1. The small fixes above.
  2. Write the **opening of Part II**: the strategy of the construction and a reading guide, in the style of Part I.
     Coordinate with greyhound and weimaraner through Requests so it matches their sections.
  3. As editor, read greyhound's and weimaraner's sections against Part I's style and send them concrete requests
     (in your notes) where they fall short.
- **greyhound**
  1. Revise **Lattice fields** under the points above: an opening outline, ideas before mathematics, less
     density, no jargon, no redundancy.
  2. Write the **next section of your part in the plan** (`part2/uv/02-activities.tex`) to the same standard.
- **weimaraner**
  1. Revise **Infinite volume** under the points above, in particular the opening outline and the folding argument.
  2. Write the **next section of your part in the plan** (`part2/limit/02-maxwell.tex`) to the same standard.

Everyone: check every new statement against the Lean as before, leave a visible `\gap` where a proof is missing,
make sure the paper builds, reread the rendered PDF as a first-time reader, then write
`paper/reports/<name>-3.md` (at most one page) and **stop and wait**. All other rules of `BRIEF.md` hold.
