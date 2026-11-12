# Greyhound — round 5 report

Revised only the proofs in the two existing ultraviolet sections. In **Lattice fields**, the Wilson-law proof now separates normalisation, Haar changes and action invariance; the finite-polynomial-space proof separates finite spanning, invariant homogeneous pieces and basis choice; and the insertion proof separates locality, covariance and the reference unit. In **Local polynomials and activities**, the finite-sampling, section-construction, square-zero and activity-summation proofs now have enumerated steps with the key formulas displayed. No statement, hypothesis, label, or source correspondence changed, and no new section was started.

For the round-4 §5 reread, these were the passages whose proof structure or mathematical explanation needed repair. The UV01 and UV02 symbol/term self-check tables remain complete (46 and 51 rows); no new definition or first-use repair was needed. The one visible UV01 obligation, construction of same-family coefficient transfers, remains open. The activity-sum result remains conditional on its displayed majorants. No Lean/Lake run or fresh source audit was made for these exposition-only edits.

Ran `latexmk -pdf -interaction=nonstopmode main.tex` in `paper/`; it completed successfully. The final log has no errors, warnings, undefined references or citations. The 60-page rendered PDF was reread on pages 19–34, covering both owned sections and their shared boundary. UV01 touches pages 19–26 (8 pages; cap 10); UV02 touches pages 26–34 (9 pages; cap 9). The sections fit their caps.

I have completed round 5 and stop here.
