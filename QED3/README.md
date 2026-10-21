**QED3 field-strength construction (QE1)**

**Disclaimer:** these documents are largely LLM-created. Their correctness has not been satisfactorily verified.

Project codename: **QE1**.

**Main theorem**

There exists a non-Gaussian probability measure on the space of closed real tempered two-forms on $`\mathbb{R}^3`$ whose tensor Schwinger functions satisfy the Osterwalder–Schrader axioms, including clustering.

The measure can be chosen as a translation-ergodic component of a volume-first continuum limit of the all-flux chamber QED3 field-strength laws, at sufficiently small positive charge with suitably tuned bare masses.

See [QEM1, Theorem A](QEM1.pdf) for the precise statement and hypotheses.

- **[QEO1](QEO1.pdf)** — [The QED3 construction: theorem contracts and proof assignments](QEO1.pdf).
- **AI-written manuscript:** **[QEM1](QEM1.pdf)** — [The continuum field-strength construction for QED in three dimensions](QEM1.pdf) · [TeX source](QEM1.tex).
- **AI-written manuscript:** **[QCM1](qed3-consequences.pdf)** — [Massless photons and interacting field-strength theories in three-dimensional QED](qed3-consequences.pdf) · [TeX source](QCM1.tex).
- **Human-written manuscript:** to be added.

- **AI-written main manuscript:** [Comprehensive edition](qed3.pdf) — 263 pages, including the corrections of October 20, 2026 · [TeX source of comprehensive edition](qed3.tex).

**Source editions used by the outlines**

The current [QEM1](QEM1.pdf) is the 32-page modular manuscript. Historical QEM1 or QE1M1 page and section references in [QEO1](QEO1.pdf) and [CEO1](Continuum%20existence%20%28CE1%29/CEO1.pdf) refer to the [263-page comprehensive edition](qed3.pdf). Their exact historical TeX line references use the [preserved pre-integration source](QEM1-preintegration.tex).

The original companion-source names identify [QEDI / S1](S1.tex), [QEDII / S2](Infinite-lattice%20reflection%20positivity%20%28LP1%29/ChamberQED.pdf), and [QEDIII / S3](S3.tex). These preserved inputs are distinct from the current modular manuscripts. The [QEDII TeX source](Infinite-lattice%20reflection%20positivity%20%28LP1%29/ChamberQED.tex) is also supplied.

**Building the manuscript**

The TeX sources are beside the PDFs. Build in a temporary copy of these files, retain the resulting PDF, and remove the temporary build directory.

For [QEM1.tex](QEM1.tex):

```sh
pdflatex -no-shell-escape -interaction=nonstopmode -halt-on-error QEM1.tex
biber QEM1
pdflatex -no-shell-escape -interaction=nonstopmode -halt-on-error QEM1.tex
pdflatex -no-shell-escape -interaction=nonstopmode -halt-on-error QEM1.tex
pdflatex -no-shell-escape -interaction=nonstopmode -halt-on-error QEM1.tex
```

For [QCM1.tex](QCM1.tex):

```sh
pdflatex -no-shell-escape -interaction=nonstopmode -halt-on-error QCM1.tex
pdflatex -no-shell-escape -interaction=nonstopmode -halt-on-error QCM1.tex
pdflatex -no-shell-escape -interaction=nonstopmode -halt-on-error QCM1.tex
pdflatex -no-shell-escape -interaction=nonstopmode -halt-on-error QCM1.tex
```
