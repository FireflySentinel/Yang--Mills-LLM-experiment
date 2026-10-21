# QED3 field-strength construction (QE1)

**Disclaimer:** these documents are largely LLM-created. Their correctness has not been satisfactorily verified.

Project codename: **QE1**.

## Main theorem

There exists a non-Gaussian probability measure on the space of closed real tempered two-forms on $`\mathbb{R}^3`$ whose tensor Schwinger functions satisfy the Osterwalder–Schrader axioms, including clustering.

The measure can be chosen as a translation-ergodic component of a volume-first continuum limit of the all-flux chamber QED3 field-strength laws, at sufficiently small positive charge with suitably tuned bare masses.

See [QEM1, Theorem A](QEM1.pdf#page=1) for the precise statement and hypotheses.

- **[QEO1](QEO1.pdf)** — [The QED3 construction: theorem contracts and proof assignments](QEO1.pdf).
- **AI-written manuscript:** **[QEM1](QEM1.pdf)** — [The continuum field-strength construction for QED in three dimensions](QEM1.pdf) · [TeX source](QEM1.tex) · [Compilation instructions](#building-the-manuscript).
- **AI-written manuscript:** **[QCM1](qed3-consequences.pdf)** — [Massless photons and interacting field-strength theories in three-dimensional QED](qed3-consequences.pdf) · [TeX source](QCM1.tex) · [Compilation instructions](#building-the-manuscript).
- **Human-written manuscript:** to be added.

- **AI-written main manuscript:** [Comprehensive edition](qed3.pdf) — 263 pages, including the corrections of October 20, 2026 · [TeX source of comprehensive edition](qed3.tex).

## Source editions used by the outlines

The current [QEM1](QEM1.pdf) is the 32-page modular manuscript. Historical QEM1 or QE1M1 page and section references in [QEO1](QEO1.pdf) and [CEO1](Continuum%20existence%20%28CE1%29/CEO1.pdf) refer to the [263-page comprehensive edition](qed3.pdf). Their exact historical TeX line references use the [preserved pre-integration source](QEM1-preintegration.tex).

The original companion-source names identify [QEDI / S1](S1.tex), [QEDII / S2](Infinite-lattice%20reflection%20positivity%20%28LP1%29/ChamberQED.pdf), and [QEDIII / S3](S3.tex). These preserved inputs are distinct from the current modular manuscripts. The [QEDII TeX source](Infinite-lattice%20reflection%20positivity%20%28LP1%29/ChamberQED.tex) is also supplied.

## Role in the [QEM1](QEM1.pdf) assembly

Shared model, parameter admission, closed-field covariance, tensor extension and final same-component OS assembly.

[QEO1](QEO1.pdf) contracts: [D0](QEO1.pdf#page=47), [T16](QEO1.pdf#page=40), [A2](QEO1.pdf#page=23), [M18](QEO1.pdf#page=70), [Z](QEO1.pdf#page=2).

Related inputs: [LPM1](Infinite-lattice%20reflection%20positivity%20%28LP1%29/LPM1.pdf), [CEM1](Continuum%20existence%20%28CE1%29/CEM1.pdf), [ECM1](Continuum%20components%20and%20clustering%20%28EC1%29/ECM1.pdf), [CVM1](Cover%20agreement%20and%20common%20tuning%20%28CV1%29/CVM1.pdf), [VTM1](Volume%20transfer%20%28VT1%29/VTM1.pdf). Read their hypotheses at the cited results.

## Assembly index

The current construction has thirteen manuscript units. This index follows the current [QEO1](QEO1.pdf) document assembly; a written draft does not certify correctness.

[Assembly overview](QEO1_assembly_overview.pdf) · [Full QEO1 outline](QEO1.pdf).

| Part | Manuscript / outline | Role |
| --- | --- | --- |
| [Overall assembly](README.md) | [QEM1](QEM1.pdf) / [QEO1](QEO1.pdf) | Shared model, parameter admission, closed-field covariance, tensor extension and final same-component OS assembly |
| [Infinite-lattice reflection positivity (LP1)](Infinite-lattice%20reflection%20positivity%20%28LP1%29/README.md) | [LPM1](Infinite-lattice%20reflection%20positivity%20%28LP1%29/LPM1.pdf) / [LPO1](Infinite-lattice%20reflection%20positivity%20%28LP1%29/LPO1.pdf) | Finite real-curvature laws, Gaussian domination and nine RP families |
| [Maxwell block analysis (MB1)](Maxwell%20block%20analysis%20%28MB1%29/README.md) | [MBM1](Maxwell%20block%20analysis%20%28MB1%29/MBM1.pdf) / [MBO1](Maxwell%20block%20analysis%20%28MB1%29/MBO1.pdf) | Photon minimization and constrained Gaussian primitives |
| [Chamber fermion block analysis (FB1)](Chamber%20fermion%20block%20analysis%20%28FB1%29/README.md) | [FBM1](Chamber%20fermion%20block%20analysis%20%28FB1%29/FBM1.pdf) / [FBO1](Chamber%20fermion%20block%20analysis%20%28FB1%29/FBO1.pdf) | Chamber inverses, locality, determinant gains and local integration |
| [Relevant extraction and normalized contraction (RN1)](Relevant%20extraction%20and%20normalized%20contraction%20%28RN1%29/README.md) | [RNM1](Relevant%20extraction%20and%20normalized%20contraction%20%28RN1%29/RNM1.pdf) / [RNO1](Relevant%20extraction%20and%20normalized%20contraction%20%28RN1%29/RNO1.pdf) | Relevant normalization, contraction and conditional reconstruction |
| [Nonlinear renormalization step (NL1)](Nonlinear%20renormalization%20step%20%28NL1%29/README.md) | [NLM1](Nonlinear%20renormalization%20step%20%28NL1%29/NLM1.pdf) / [NLO1](Nonlinear%20renormalization%20step%20%28NL1%29/NLO1.pdf) | Exact conditional nonlinear step and connected logarithm |
| [Positive probes and free response (PR1)](Positive%20probes%20and%20free%20response%20%28PR1%29/README.md) | [PRM1](Positive%20probes%20and%20free%20response%20%28PR1%29/PRM1.pdf) / [PRO1](Positive%20probes%20and%20free%20response%20%28PR1%29/PRO1.pdf) | Positive compact probe and free second/fourth response coefficients |
| [Continuum existence (CE1)](Continuum%20existence%20%28CE1%29/README.md) | [CEM1](Continuum%20existence%20%28CE1%29/CEM1.pdf) / [CEO1](Continuum%20existence%20%28CE1%29/CEO1.pdf) | Gaussian/correlation stability, compactness, structural inheritance and prescribed-parent recovery |
| [Cover agreement and common tuning (CV1)](Cover%20agreement%20and%20common%20tuning%20%28CV1%29/README.md) | [CVM1](Cover%20agreement%20and%20common%20tuning%20%28CV1%29/CVM1.pdf) / [CVO1](Cover%20agreement%20and%20common%20tuning%20%28CV1%29/CVO1.pdf) | Exact cover agreement, stopping arithmetic and one common tuned pair |
| [Reference response (RR1)](Reference%20response%20%28RR1%29/README.md) | [RRM1](Reference%20response%20%28RR1%29/RRM1.pdf) / [RRO1](Reference%20response%20%28RR1%29/RRO1.pdf) | Early source identities and later normalized reference response |
| [Continuum components and clustering (EC1)](Continuum%20components%20and%20clustering%20%28EC1%29/README.md) | [ECM1](Continuum%20components%20and%20clustering%20%28EC1%29/ECM1.pdf) / [ECO1](Continuum%20components%20and%20clustering%20%28EC1%29/ECO1.pdf) | Clustering and reflection/Gaussian inheritance for the same components |
| [Terminal measure and pressure (TP1)](Terminal%20measure%20and%20pressure%20%28TP1%29/README.md) | [TPM1](Terminal%20measure%20and%20pressure%20%28TP1%29/TPM1.pdf) / [TPO1](Terminal%20measure%20and%20pressure%20%28TP1%29/TPO1.pdf) | Terminal measure, pressure and two-torus comparison |
| [Volume transfer (VT1)](Volume%20transfer%20%28VT1%29/README.md) | [VTM1](Volume%20transfer%20%28VT1%29/VTM1.pdf) / [VTO1](Volume%20transfer%20%28VT1%29/VTO1.pdf) | All-volume products, prescribed-parent finite-periodic moments and component cumulants |

The early source identities in [RRM1](Reference%20response%20%28RR1%29/RRM1.pdf) enter [TPM1](Terminal%20measure%20and%20pressure%20%28TP1%29/TPM1.pdf); the later response estimate in [RRM1](Reference%20response%20%28RR1%29/RRM1.pdf) uses [TPM1](Terminal%20measure%20and%20pressure%20%28TP1%29/TPM1.pdf). These are distinct stages within one manuscript. [CEO1](Continuum%20existence%20%28CE1%29/CEO1.pdf) covers the compactness part of [CEM1](Continuum%20existence%20%28CE1%29/CEM1.pdf); the latter also supplies structural inheritance and prescribed-parent recovery.

## Navigation

The published PDFs retain their mathematical text. Document and numbered-result links open the published PDFs; assembly links open the topic READMEs. Citations to material outside this assembly remain visible without a download link.

## Building the manuscript

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
