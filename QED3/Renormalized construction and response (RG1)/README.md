# Renormalized construction and response (RG1)

**Disclaimer:** these documents are largely LLM-created. Their correctness has not been satisfactorily verified.

Project codename: **RG1**.

- **RGO1** — [Renormalized construction and non-Gaussianity in QED3](RGO1.pdf).
- **AI-written manuscript:** to be added.
- **Human-written manuscript:** to be added.

RGO1 organizes the nine renormalization and response parts of the QEM1 assembly. It is a stage outline, not an additional manuscript unit.

| Part | Outline status |
| --- | --- |
| [MBM1](../Maxwell%20block%20analysis%20%28MB1%29/README.md) / [MBO1](../Maxwell%20block%20analysis%20%28MB1%29/README.md) | PDF available |
| [FBM1](../Chamber%20fermion%20block%20analysis%20%28FB1%29/README.md) / [FBO1](../Chamber%20fermion%20block%20analysis%20%28FB1%29/README.md) | PDF available |
| [RNM1](../Relevant%20extraction%20and%20normalized%20contraction%20%28RN1%29/README.md) / [RNO1](../Relevant%20extraction%20and%20normalized%20contraction%20%28RN1%29/README.md) | PDF available |
| [NLM1](../Nonlinear%20renormalization%20step%20%28NL1%29/README.md) / [NLO1](../Nonlinear%20renormalization%20step%20%28NL1%29/README.md) | PDF available |
| [CVM1](../Cover%20agreement%20and%20common%20tuning%20%28CV1%29/README.md) / [CVO1](../Cover%20agreement%20and%20common%20tuning%20%28CV1%29/README.md) | PDF available |
| [PRM1](../Positive%20probes%20and%20free%20response%20%28PR1%29/README.md) / [PRO1](../Positive%20probes%20and%20free%20response%20%28PR1%29/README.md) | PDF available |
| [RRM1](../Reference%20response%20%28RR1%29/README.md) / [RRO1](../Reference%20response%20%28RR1%29/README.md) | PDF available |
| [TPM1](../Terminal%20measure%20and%20pressure%20%28TP1%29/README.md) / [TPO1](../Terminal%20measure%20and%20pressure%20%28TP1%29/README.md) | PDF available |
| [VTM1](../Volume%20transfer%20%28VT1%29/README.md) / [VTO1](../Volume%20transfer%20%28VT1%29/README.md) | PDF available |

All nine focused outlines are available. Full hypotheses remain in the linked statements. Green in the PRO1, RRO1 and VTO1 flowcharts marks an existing proof draft, not verified correctness.

## Stage target

The target below is reproduced from **RGO1/A3**, with formatting adapted for GitHub.

Expanded statement: [VTO1/A3](../Volume%20transfer%20%28VT1%29/VTO1.pdf#page=1).

**Target of this stage.**

Fix the standard-weight chamber cutoff, $`0<\rho<1`$, and
$`0<\bar m\le1`$, as in
[QEO1/D0](../QEO1.pdf#page=47).
The construction selects one real bare mass and vacuum pair
$`P_N(e)=(m_{0,N}(e),\epsilon_{0,N}^{\rm v}(e))`$, independently
of the outer construction volume. Its total fine mass is
$`\bar m L^{-N}+m_{0,N}(e)`$. Every interacting construction,
reference and transfer law uses this pair. The free comparisons
retain the unshifted positive reference mass.

For a real compact smooth two-form $`\beta`$, set

```math
f=dd^*\beta,\qquad
 b(f)=-6\mathrm{Tr}
 [(\bar m+\gamma\cdot\partial)^{-1}i\gamma\cdot d^*\beta]^4.
```

The probe theorem [B7](RGO1.pdf#page=13) supplies a choice with $`b(f)>0`$.
The desired conclusion is that there are $`C_f<\infty`$,
$`\sigma>0`$, and $`e_f>0`$, independent of the chosen parent
and its component, such that for $`0<e\le e_f`$, every
volume-first parent law $`\mu`$ of this construction has

```math
|\kappa_4^{\mu_\xi}(f)-e^4b(f)|\le C_fe^{4+\sigma}
```

on one full-measure set of its translation-ergodic components.
Reducing $`e_f`$ so $`C_fe^\sigma\le b(f)/2`$ gives
$`\kappa_4^{\mu_\xi}(f)\ge e^4b(f)/2>0`$.
Here $`\kappa_4(X)=\mathbb E[(X-\mathbb EX)^4] -3\mathbb E[(X-\mathbb EX)^2]^2`$.

**The main estimate.**

The workhorse is [T17](RGO1.pdf#page=19): a bound for every finite set of
distinct translated Wick probes, uniform in the construction
volume and fine mesh. A parent fourth-moment estimate alone
does not give the component conclusion.

**Inputs and scope.**

Use [A1](RGO1.pdf#page=20) to retain each prescribed parent and its moment
limits, [B2](RGO1.pdf#page=21) for the Gaussian bound on the same components,
and [B5](RGO1.pdf#page=22) to pass translated-product bounds to conditional
expectations. The final parameter choice is [T16](RGO1.pdf#page=23).
The tensor OS conclusions remain in QEO1's structural branch.
Intersect its component set with the one obtained here.

**Exact contracts.**

[QEO1/A3](../QEO1.pdf#page=43),
[QEO1/T18](../QEO1.pdf#page=122), and
[QEO1/Z](../QEO1.pdf#page=2).
This is the target of a working proof outline, not a new proof.
The diagram's ordinary statement pages describe the assignments;
their external links open the complete existing contracts.


[QEM1 assembly index](../README.md).
