# Greyhound — checkpoint 3

Revised `part2/uv/01-lattice.tex` and wrote the authorized next section, `part2/uv/02-activities.tex`. Both open with linked outlines. Substantial proofs explain their idea before the formulas. The lattice-law argument now displays the separate Haar, product-measure and energy identities; transport analyticity and unit normalization have explicit calculations. Public definitions remain linked to Part I, with sized delimiters and arithmetic fractions throughout. Dalmatian's concrete UV requests are resolved.

The new section proves finite recovery of radial Taylor coefficients from transported plaquettes, constructs normalized polynomial sections with threshold-factor derivative bounds, proves weighted square-zero product/exponential estimates, and establishes absolute convergence of activity sums under their stated local majorants. Exact bad-site coverage, connected-union support weights, per-anchor versus per-hit bounds, enlarged indicator reads and periodic wrapping are retained. Its exposition uses a highest-degree polynomial argument for finite sampling rather than the source's shrinking-grid presentation; proofs and organization are newly written.

Checked definitions and relevant proof bodies in the Lean checkout at `3456e5e75cf8d4cd558955a5c7638fba2d68f464`. All 63 numbered items have source correspondence in `notes/greyhound.md`; source spans were checked. This is a source-reading check, without a Lean build or fresh kernel audit.

The local-section construction pays that component of UV01's former marker. One visible gap remains: invertible coefficient transfers for the same Wilson family with the stated endpoint, unit, reality and symmetry conditions. Activity convergence assumes supplied bounds; production of RG activities and their bounds, integration identities, ultraviolet convergence and Maxwell/rank estimates remain later work.

The prescribed LaTeX build succeeds; its final pass has no errors, warnings, missing references/citations or bad boxes. Read every rendered page 17–30 of the 49-page snapshot. UV01 touches seven pages (cap ten); UV02 eight (cap nine). Final source/PDF hashes are recorded in the notes; temporary review artifacts were removed.

No editorial decision is pending. Stopped after this report and awaiting instructions.
