# Feedback, round 3 (from Amélie, after reading checkpoint 3)

All three agents read this whole file. Rounds 1 and 2 still hold in full. The rules marked **(standing)** hold for
every later round and every new section.

## 1. British spelling (standing)

Use British spelling throughout the paper, with *-ise* endings: normalise, renormalisation, centre, centred,
colour, behaviour, neighbourhood, analyse, modelling, and so on. This applies to prose, section titles, theorem
names and comments meant for readers. It does not apply to Lean identifiers, to the titles of cited works, or to
quotations. dalmatian converts Part I and the shared files and the Part II opening; each owner converts their own
sections.

## 2. Every object is defined and explained where the reader meets it (standing)

Examples Amélie found by skimming. They are examples only: the problem is general.

- **"its line integral of~$A^J$"** in the proof of Lemma `lem:uv-sampling` (`part2/uv/02-activities.tex` line 64).
  $A^J$ is defined in another section (`part2/uv/01-lattice.tex` line 220, inside a proof) and used here with no
  reference and no explanation. The reader cannot know what it is.
- **"labels", "classical labels".** These appear everywhere. Part I introduces "a set of labels for lattice
  observables" (`02-definitions.tex` line 81); Part II introduces "classical labels" (`01-lattice.tex`,
  Definition `def:uv-labels`); `\mathcal L` in the Wightman definition is a third kind of label. A reader cannot tell
  what a label is, how the three kinds relate, or why the word is used at all. Explain the idea once, in Part I,
  clearly (what is being labelled, and why labels are needed), and use the words consistently afterwards. If a
  better standard term exists (for instance *field*, *local observable*, *gauge-invariant polynomial*), use it.
- **"under left-link increments"** (`02-activities.tex` line 215): not explained anywhere.
- **"bond reflection", "site reflection"** (`01-infinite-volume.tex` line 40): explain them, with a picture or a
  formula (reflection in a hyperplane through lattice points versus a hyperplane halfway between them).
- **"site"**: say once, in the definitions, that the sites are the points of the lattice.
- **"The transfer argument separates insertions by coordinate hyperplanes."** This sentence makes no sense to the
  reader. Say what is meant.

Rules:
1. Every symbol and every technical word is defined before its first use, and explained: what it is, in which
   context, and what the idea is. Never use a technical word only to sound precise.
2. When an object is used again away from its definition, give a reference to its definition, unless it is
   obvious from the context.
3. Objects needed in more than one section are defined in a displayed definition, not inside a proof.
4. **Self-check (standing).** For each section you own, keep in your notes a table of every symbol and technical
   term the section uses, with where it is defined (label) and where it is first used. Fix every entry that is
   used before it is defined, defined only inside a proof, or never explained. Include the table's status in your
   report.

## 3. Outlines: what works and what does not

This outline paragraph of Infinite volume is **great**, and is the model for every section:

> The section follows five steps. Subsection~\ref{subsec:iv-lattice} proves these reflection estimates.
> Subsection~\ref{subsec:iv-compactness} uses them to bound changes in the insertion points and select common
> subsequences. […] Finally, Subsection~\ref{subsec:iv-full-spacing} uses the fixed-volume limit to remove the
> auxiliary spacing subsequence, leaving only a volume refinement.

This passage is **not clear**:

> The ultraviolet estimates used at these steps are stated where they enter, with three explicit deferred-proof
> markers. The phase decomposition of Proposition~\ref{prop:limit} requires the later Hilbert-space and rotation
> arguments.

The reader does not know which ultraviolet estimates are meant, what "deferred-proof markers" are, or what "the
Hilbert-space and rotation arguments" are. Say concretely which estimates (in words, with references), and what
the later arguments do. Do not mention the `\gap` markers in the prose: they are working notes for us, not part of
the mathematics.

## 4. Ideas first, technicalities in mathematics (standing)

Subsection `subsec:iv-compactness` (Infinite volume, §8.2 in the PDF) is the worst current example: the whole
explanation is technical, a dense wordy proof that is impossible to understand and hard to read. Amélie wants to
see the ideas. Rewrite it so that it is coherent, readable and pedagogical:

- begin with the idea in plain words (why the correlations are equicontinuous, and why that gives a convergent
  subsequence);
- then state the results in mathematics;
- put the technicalities inside proofs, expressed in mathematical language (displays), not in sentences.

Apply the same standard to every section. Remove all jargon and all redundancy.

## This round (round 4)

This round is **revision only**: do not start new sections. The aim is that everything written so far reaches the
standard of Part I.

- **dalmatian**: British spelling in your files; explain labels once in the definitions (see §2) and coordinate the
  terminology with both colleagues; define "site"; then, as editor, do a jargon and undefined-term audit of all
  four Part II sections and send each owner concrete requests. You decide the shared terminology.
- **greyhound**: Lattice fields and Polymer activities under §§1–4; fix `A^J` and "left-link increments" and every
  similar case your self-check table finds.
- **weimaraner**: Infinite volume and Maxwell comparison under §§1–4; rewrite §8.2 (`subsec:iv-compactness`) as
  described; fix the outline passage in §3, bond/site reflections and the "transfer argument" sentence.

Everyone: build, reread the rendered PDF as a first-time reader, write `paper/reports/<name>-4.md` (at most one
page, including the self-check table status), and **stop and wait**.
