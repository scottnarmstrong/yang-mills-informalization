# Feedback, round 6 (from Amélie, after reading checkpoint 6)

All agents read this whole file and `paper/RULES.md`, which now collects every standing rule. Rounds 1–5 still hold.

## Overall

**It looks good.** The cross-audit worked. Now:

- **Continue writing in this style.** The new sections must read exactly like the revised ones.
- **Catch your own errors.** Self-check against `RULES.md` before your section goes to its auditor (rule E1).
- **Stick brutally to the rules you have learnt**, and write consistently as you did in the last round.

## Proof steps: new format (standing; rule C6)

Replace the current design of proof steps (the enumerate lists with `Step 1.` labels, and the `\item \emph{…}`
lists used as steps) by:

```latex
\medskip\noindent\textit{Step~1: Explain the idea of the step.}
<the step's text and displays>
```

dalmatian adds to `macros.tex`:

```latex
\newcommand{\proofstep}[2]{\par\medskip\noindent\textit{Step~#1: #2}\enspace}
```

used as `\proofstep{1}{Bound the boundary kernel.}`. Everyone uses this macro.

**Steps should not be used excessively.** They structure a long proof. Each step is a substantial piece of the
argument, not one sentence. A proof idea of a few lines, or a short proof, has no steps. Where the current text has
one-sentence steps, merge them into fewer, meaningful steps or into ordinary paragraphs.

## This round (round 7)

### Part 1: the step format everywhere

Each owner converts the proof steps in their existing sections to the new format and removes excessive steps
(dalmatian: Part I and the Part II opening; greyhound: §§6–7; weimaraner: §§8–9).

### Part 2: the next sections

| writer | new section | file |
|---|---|---|
| dalmatian | The constants and the order of their choice (Part I) | `part1/06-constants.tex` |
| greyhound | the block-spin step, gauge coordinates and the stationary background field | `part2/uv/03-blocking.tex` |
| weimaraner | Ward identities, rotations and the stress tensor | `part2/limit/03-ward.tex` |

Follow `PLAN.md` for their scope. Write each section to the standard of `RULES.md` from the first draft. Check every
statement against the Lean; leave a visible `\gap` where a proof is missing.

### Part 3: self-check, cross-audit, repair, verify

1. **Self-check** your new section against `RULES.md`, rule by rule (E1). Then put a line `READY FOR AUDIT` at the end
   of your notes file.
2. **Audit** (once the section you audit is `READY FOR AUDIT`), in `paper/audits/r7-<auditor>-on-<owner>.md`:

   | auditor | audits |
   |---|---|
   | weimaraner | greyhound's new section `part2/uv/03-blocking.tex` |
   | dalmatian | weimaraner's new section `part2/limit/03-ward.tex` |
   | greyhound | dalmatian's new section `part1/06-constants.tex` |

   Also check the converted step format in the auditee's older sections (class **S**). Be exhaustive; end with
   `AUDIT COMPLETE`.
3. **Repair** in `paper/audits/r7-<owner>-response.md`, with the class-wide search (rule A0); end with
   `REPAIR COMPLETE`.
4. **Verify**: the auditor rereads and appends `fixed` / `not fixed (why)` and any new failures; end with `VERIFIED`.
   The owner fixes anything not fixed, and the auditor rechecks it.

Then build, check the PDF, write `paper/reports/<name>-7.md` (at most one page), and **stop and wait**.

Use `sleep 180` between checks when waiting for another agent's file. No subagents.
