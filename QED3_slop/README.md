# QED3 field-strength construction (QE1)

**Disclaimer:** these documents are largely LLM-created. Their correctness has not been satisfactorily verified.

Project codename: **QE1**.

- **QEO1** — [The QED3 construction: theorem contracts and proof assignments](QEO1.pdf).
- **QEM1** — *The continuum field-strength construction for QED in three dimensions* (manuscript to be added).

## Role in the QEM1 assembly

Shared model, parameter admission, closed-field covariance, tensor extension and final same-component OS assembly.

QEO1 contracts: [D0](QEO1.pdf#page=47), [T16](QEO1.pdf#page=40), [A2](QEO1.pdf#page=23), [M18](QEO1.pdf#page=70), [Z](QEO1.pdf#page=2).

Related inputs: [LPM1](Infinite-lattice%20reflection%20positivity%20%28LP1%29/README.md), [CEM1](Continuum%20existence%20%28CE1%29/README.md), [ECM1](Continuum%20components%20and%20clustering%20%28EC1%29/README.md), [CVM1](Cover%20agreement%20and%20common%20tuning%20%28CV1%29/README.md), [VTM1](Volume%20transfer%20%28VT1%29/README.md). Read their hypotheses at the cited results.

## Assembly index

The current construction has thirteen manuscript units. This index follows the current QEO1 document assembly; a written draft does not certify correctness.

[Assembly overview](QEO1_assembly_overview.pdf) · [Full QEO1 outline](QEO1.pdf) · [RGO1](Renormalized%20construction%20and%20response%20%28RG1%29/README.md) stage outline.

| Part | Manuscript / outline | Role |
| --- | --- | --- |
| [Overall assembly](README.md) | QEM1 / QEO1 | Shared model, parameter admission, closed-field covariance, tensor extension and final same-component OS assembly |
| [Infinite-lattice reflection positivity (LP1)](Infinite-lattice%20reflection%20positivity%20%28LP1%29/README.md) | LPM1 / LPO1 | Finite real-curvature laws, Gaussian domination and nine RP families |
| [Maxwell block analysis (MB1)](Maxwell%20block%20analysis%20%28MB1%29/README.md) | MBM1 / MBO1 | Photon minimization and constrained Gaussian primitives |
| [Chamber fermion block analysis (FB1)](Chamber%20fermion%20block%20analysis%20%28FB1%29/README.md) | FBM1 / FBO1 | Chamber inverses, locality, determinant gains and local integration |
| [Relevant extraction and normalized contraction (RN1)](Relevant%20extraction%20and%20normalized%20contraction%20%28RN1%29/README.md) | RNM1 / RNO1 | Relevant normalization, contraction and conditional reconstruction |
| [Nonlinear renormalization step (NL1)](Nonlinear%20renormalization%20step%20%28NL1%29/README.md) | NLM1 / NLO1 | Exact conditional nonlinear step and connected logarithm |
| [Positive probes and free response (PR1)](Positive%20probes%20and%20free%20response%20%28PR1%29/README.md) | PRM1 / PRO1 (planned) | Positive compact probe and free second/fourth response coefficients |
| [Continuum existence (CE1)](Continuum%20existence%20%28CE1%29/README.md) | CEM1 / CEO1 | Gaussian/correlation stability, compactness, structural inheritance and prescribed-parent recovery |
| [Cover agreement and common tuning (CV1)](Cover%20agreement%20and%20common%20tuning%20%28CV1%29/README.md) | CVM1 / CVO1 | Exact cover agreement, stopping arithmetic and one common tuned pair |
| [Reference response (RR1)](Reference%20response%20%28RR1%29/README.md) | RRM1 / RRO1 (planned) | Early source identities and later normalized reference response |
| [Continuum components and clustering (EC1)](Continuum%20components%20and%20clustering%20%28EC1%29/README.md) | ECM1 / no separate outline | Clustering and reflection/Gaussian inheritance for the same components |
| [Terminal measure and pressure (TP1)](Terminal%20measure%20and%20pressure%20%28TP1%29/README.md) | TPM1 / TPO1 | Terminal measure, pressure and two-torus comparison |
| [Volume transfer (VT1)](Volume%20transfer%20%28VT1%29/README.md) | VTM1 / VTO1 (planned) | All-volume products, prescribed-parent finite-periodic moments and component cumulants |

The early source identities in RRM1 enter TPM1; the later response estimate in RRM1 uses TPM1. These are distinct stages within one manuscript. CEO1 covers the compactness part of CEM1; the latter also supplies structural inheritance and prescribed-parent recovery.

Earlier manuscript editions remain in the GitHub repository; the QEM1 entry above identifies the current assembly.

## Principal statement

Notation and numbered references below follow **QEM1**.

### Setting

The observable in this paper is the field strength. We regard it as a real tempered two-form on $`\mathbb{R}^3`$, and write $`F(f)`$ for its pairing with a test two-form $`f`$. The regularization uses a noncompact gauge field and four-component chamber fermions, with all flux sectors included. The order of limits is part of the construction: the volume tends to infinity at a fixed lattice spacing, and the spacing then tends to zero.

For a lattice curvature $`u`$, the physical field $`F^\sharp`$ is the centered plaquette step interpolation of $`\eta^{-3/2}u`$ at spacing $`\eta`$; see Section 2, Section 3 for the finite law and interpolation. A volume-first limit is a weak limit of fixed-spacing infinite-volume laws as $`\eta\to0`$. We take these weak limits on the Hilbert space $`H_{-4}`$ of tempered two-forms defined in Section 2.2. In the following statement $`\gamma_j=\mathrm{diag}(\sigma_j,-\sigma_j)`$, where $`\sigma_j`$ are the Pauli matrices, and $`d^*`$ is the Euclidean adjoint of $`d`$.

### The finite law and the limit topology

We use the all-flux chamber model of (**LPM1**, Section 2). The following definitions fix its normalization and its relation to the physical scales in (2). All cochain norms and pairings sum over positively oriented cells. Reversing the orientation changes the sign of a cochain.

### The chamber matrix and the flux sum

Let $`O_{\rm cub}`$ be the signed permutation matrices in three dimensions. A chamber label is $`(c,g)`$, where $`c\in\mathbb{Z}^3`$ and $`g\in O_{\rm cub}`$. There are $`48`$ labels at each photon site. Let $`s_0`$ reverse coordinate three, let $`s_1,s_2`$ exchange coordinates $`(2,3)`$ and $`(1,2)`$, and let $`r_{e_1}`$ reverse coordinate one. With the Pauli matrices $`\sigma_j`$, put $`\gamma_j=\mathrm{diag}(\sigma_j,-\sigma_j)`$ and

```math
\begin{gathered}
 (w_0,w_1,w_2,w_3)=(6,6\sqrt2,6\sqrt2,6),\\[0pt]
 (\mathbf n_0,\mathbf n_1,\mathbf n_2,\mathbf n_3)
 =(e_3,(e_2-e_3)/\sqrt2,(e_1-e_2)/\sqrt2,-e_1),\qquad
 M_i(g)=\tfrac12w_i(\rho+\gamma\cdot g\mathbf n_i).
 \end{gathered}
```

For a bond phase $`B`$, the unit-mesh massless matrix is

```math
\begin{split}
 (D^{\rm ch}[B]\psi)(c,g)={}&
 \sum_{i=0}^2M_i(g)[\psi(c,g)-\psi(c,gs_i)]\\[0pt]
 &+M_3(g)[\psi(c,g)-e^{iB(c,c+ge_1)}
                         \psi(c+ge_1,gr_{e_1})].
 \end{split}
\tag{8}
```

On $`C(n)=\mathbb{Z}^3/n\mathbb{Z}^3`$ the bond fields are periodic and spinors satisfy $`\psi(c+ne_j,g)=-\psi(c,g)`$. The massive matrix $`D^{\rm ch}[B]+\boldsymbol\mu`$ is the matrix in (**LPM1**, Section 2) at diagonal parameter $`\boldsymbol\mu+\frac\rho2\sum_iw_i`$, where $`\boldsymbol\mu`$ is the total lattice mass. The chamber inner product has weight $`1/48`$; this constant weight does not change a finite-dimensional determinant.

For $`q>0`$, put $`r_q=2\pi/q`$. A photon configuration is a pair $`(A,z)`$ with $`A`$ a real one-cochain and $`z`$ a closed integer two-cochain, modulo

```math
(A,z)\sim(A+r_q k,z-dk),\qquad k\text{ an integer one-cochain}.
```

Its curvature is $`u=dA+r_qz`$. With the representative $`A(b)\in[0,r_q)`$, define

```math
Z_{C(n)}[G]=
 \sum_{\substack{z\in C^2(C(n);\mathbb{Z})\\dz=0}}
 \int_{[0,r_q)^{3n^3}}
 G(A,z)e^{-\|u\|^2/2}
 \det(D^{\rm ch}[qA]+\boldsymbol\mu)\,\mathrm{d} A.
\tag{9}
```

The determinant is nonnegative and $`0<Z_{C(n)}[1]<\infty`$ for every real $`\boldsymbol\mu`$, by (**LPM1**, Propositions 2.2–2.3). We write $`\mathbb{E}_n^{\rm af}=Z_{C(n)}[\,\cdot\,]/Z_{C(n)}[1]`$. Rectangular tori carry the same periodic photon and antiperiodic fermion conventions. No flux class is excluded from this law.

At the physical cutoff, $`q=e\sqrt\eta`$ and $`\boldsymbol\mu=\boldsymbol\mu_N=\bar m\eta+m_{0,N}(e)`$. The physical field $`F^\sharp`$ is the centered step interpolation of $`\eta^{-3/2}u`$, defined precisely in Section 3. For a fixed mass sequence, $`P_{N,T}`$ denotes its law on $`H_{-4}`$. Let $`\mathcal V_N`$ be the set of its weak limits as $`T\to\infty`$. A volume-first limit is a weak limit of $`\mu_i\in\mathcal V_{N_i}`$ with $`N_i\to\infty`$.

Write $`h_\kappa=h_k e_{ij}`$ for the real Hermite two-forms, $`k\in\mathbb{Z}_{\ge0}^3`$, $`i<j`$, with eigenvalues $`\lambda_\kappa=2|k|_1+4`$ for $`1+|y|^2-\Delta`$. Set

```math
\|F\|_{-s}^2=\sum_\kappa\lambda_\kappa^{-2s}|F(h_\kappa)|^2,
 \qquad H_{-s}=\{F\in\mathcal S':\|F\|_{-s}<\infty\}.
```

All weak convergence of laws on $`H_{-4}`$ uses its norm topology.

Write $`\eta=L^{-N}`$, $`R=8hL^T`$, and $`n=R/\eta`$, as in (2). A plaquette of the unit covering lattice is $`\sigma=(x;\mu\nu)`$, with $`\mu<\nu`$ and centre $`y_\sigma=x+(e_\mu+e_\nu)/2`$. Its averaging cube is

```math
Q_\eta(\sigma)=\eta\bigl(y_\sigma+[-1/2,1/2)^3\bigr).
```

For each fixed orientation these cubes partition $`\mathbb{R}^3`$. If $`u`$ is a real lattice curvature, its physical step field is $`\eta^{-3/2}u(\sigma)`$ on $`Q_\eta(\sigma)`$ in component $`\mu\nu`$. For a Schwartz two-form $`f`$, define

```math
f_{[\eta]}(\sigma)
   =\eta^{-3/2}\int_{Q_\eta(\sigma)}f_{\mu\nu}(y)\,\mathrm{d} y,
\tag{10}
```

```math
f^R(y)=\sum_{k\in\mathbb{Z}^3}f(y+Rk),
```

```math
f_\eta([\sigma])
   =\eta^{-3}\int_{Q_\eta(\sigma)}f^R_{\mu\nu}(y)\,\mathrm{d} y.
\tag{11}
```

Here $`[\sigma]`$ is the plaquette class modulo $`n\mathbb{Z}^3`$. The torus cochain norm is $`|v|_\eta^2=\eta^3\sum_{[\sigma]}|v([\sigma])|^2`$. The covering cochain norm $`\|\cdot\|`$ is the unweighted $`\ell^2`$ norm. For the periodic extension $`\widetilde u`$ of $`u`$,

```math
F^\sharp(f)=\eta^{3/2}\sum_{[\sigma]}f_\eta([\sigma])u(\sigma)
            =\sum_\sigma f_{[\eta]}(\sigma)\widetilde u(\sigma).
\tag{12}
```

The normalization in the first equality combines the cell volume $`\eta^3`$ with the physical field factor $`\eta^{-3/2}`$.

**Theorem A (Field-strength OS theorem).**

Fix $`0<\rho<1`$ and $`0<\bar m\le1`$, the chamber Wilson parameter and reference mass parameter in physical units. Use the standard chamber weights $`(6,6\sqrt2,6\sqrt2,6)`$. There are an odd scale factor $`L\ge5`$, numbers $`e_{\mathrm{phys}},\sigma>0`$, and real volume-independent bare mass shifts $`m_{0,N}(e)`$ for $`N\in\mathbb{Z}_{\ge0}`$ and $`0<e\le e_{\mathrm{phys}}`$, with $`|m_{0,N}(e)|<1/8`$, with the following property.

Fix a real $`\beta\in C_c^\infty(\mathbb{R}^3;\Lambda^2)`$ such that $`f=dd^*\beta`$ has

```math
b(f):=-6\mathrm{tr}\bigl[(S_{\bar m}\,i\gamma\cdot d^*\beta)^4\bigr]>0,
 \qquad S_{\bar m}=(\bar m+\gamma\cdot\partial)^{-1}.
\tag{1}
```

Such probes exist. There is $`e_\beta\in(0,e_{\mathrm{phys}}]`$ such that, for $`0<e\le e_\beta`$, the all-flux chamber laws on the coordinate cubic tori of unit side $`n=R/\eta`$, with periodic gauge fields and fermions antiperiodic in all three coordinate directions, and with

```math
\eta=L^{-N},\quad R=8hL^T,\quad
 h=L^{\lfloor\log_L\bar m^{-1}\rfloor},\quad
 q=e\eta^{1/2},\quad \boldsymbol\mu_N=\bar m\eta+m_{0,N}(e)
\tag{2}
```

with $`N,T\in\mathbb{Z}_{\ge0}`$ have volume-first limit points. Every such limit point is carried by closed tempered two-forms, satisfies Gaussian domination with constant one, and has tensor Schwinger functions satisfying (E0′)–(E3) below. Let $`\mu`$ be any such limit point and $`\mu=\int\mu_\xi\,\mathrm{d}\nu(\xi)`$ its decomposition into translation-ergodic laws. For $`\nu`$-almost every $`\xi`$, $`\mu_\xi`$ is carried by closed tempered two-forms and satisfies

```math
\int e^{F(g)}\,\mathrm{d}\mu_\xi(F)\le e^{\|g\|_{L^2}^2/2}
 \qquad(g\in\mathcal{S}(\mathbb{R}^3;\Lambda^2)\text{ real}).
\tag{3}
```

Its Schwinger functions $`S_n^\xi(g_1\otimes\cdots\otimes g_n) =\int\prod_{a=1}^nF(g_a)\,\mathrm{d}\mu_\xi(F)`$ extend to the complex tensor Schwartz spaces $`\mathcal{S}_n=\mathcal{S}(\mathbb{R}^{3n};(\Lambda^2\mathbb{C}^3)^{\otimes n})`$ and obey the following conditions, with $`S_0^\xi=1`$.

**(E0′)** For $`n\ge1`$ and $`\Psi\in\mathcal{S}_n`$,

```math
|S_n^\xi(\Psi)|\le2\,66^n\sqrt{n!}\,q_{6n}(\Psi),\qquad
 q_m(\Psi)=\max_{|\alpha|\le m}\sup_y
 (1+|y|^2)^{m/2}|\partial^\alpha\Psi(y)|,
\tag{4}
```

where the maximum is also over tensor components.

**(E1)** For every Euclidean motion $`g(x)=Qx+a`$, $`Q\in O(3)`$, $`S_n^\xi(g\cdot\Psi)=S_n^\xi(\Psi)`$, where

```math
(g\cdot\Psi)(x_1,\ldots,x_n)
 =(\Lambda^2Q)^{\otimes n}\Psi(g^{-1}x_1,\ldots,g^{-1}x_n).
```

**(E2)** Let $`r`$ be reflection in a plane through the origin and $`H`$ either closed half-space bounded by that plane. If $`\Psi_0\in\mathbb{C}`$ and $`\Psi_k\in\mathcal{S}_k`$, $`1\le k\le M`$, have $`\mathrm{supp}\Psi_k\subset H^k`$, then

```math
\sum_{k,l=0}^M S_{k+l}^\xi
 \bigl(\Theta_k\Psi_k\otimes\Psi_l\bigr)\ge0,
 \qquad \Theta_k\Psi_k=\overline{r\cdot\Psi_k},\quad
 \Theta_0c=\overline c.
\tag{5}
```

**(E3)** $`S_n^\xi`$ is unchanged by simultaneous permutation of the arguments and their tensor indices.

**(E4)** For $`\Psi\in\mathcal{S}_k`$ and $`\Phi\in\mathcal{S}_l`$,

```math
S_{k+l}^\xi(\Psi\otimes\tau_a^{\otimes l}\Phi)
 \longrightarrow S_k^\xi(\Psi)S_l^\xi(\Phi)
 \quad\text{as }|a|\longrightarrow\infty,
\tag{6}
```

where

```math
(\tau_a^{\otimes l}\Phi)(x_1,\ldots,x_l)
 =\Phi(x_1-a,\ldots,x_l-a).
```

Moreover, for a constant $`C_f`$ depending only on the fixed construction, reference mass and probe, and independent of $`0<e\le e_\beta`$, the limit point and $`\xi`$,

```math
\bigl|\kappa_4^{\mu_\xi}(f)-e^4b(f)\bigr|
 \le C_f e^{4+\sigma},\qquad
 \kappa_4^{\mu_\xi}(f)\ge\tfrac12e^4b(f)>0.
\tag{7}
```

In particular, $`\mu_\xi`$ is non-Gaussian. The full-measure component set is asserted for each fixed parent law, charge and probe.

Here $`\kappa_4^\lambda(f)`$ is the fourth cumulant of $`F(f)`$ under a law $`\lambda`$. For the Gaussian-dominated laws considered here, $`F(f)`$ has mean zero, so $`\kappa_4^\lambda(f)=S_4^\lambda(f^{\otimes4}) -3S_2^\lambda(f^{\otimes2})^2`$. The charge threshold may depend on the fixed probe. The factorization in (E4) is a conclusion for the translation-ergodic components.

The tensor action in (E1) is essential to (E2). For reflection in $`x_1=0`$, the components $`F_{12}`$ and $`F_{13}`$ change sign, while $`F_{23}`$ does not. Replacing this action by scalar reflection changes the positivity assertion. The growth condition is stated on all tensor tests, including tests meeting the diagonals; bounds on products of separately smeared fields alone do not state (E0′).


## Navigation

The published PDFs retain their mathematical text. Links to published outlines use their repository locations; links to withheld manuscripts open the corresponding README. Citations to material outside this assembly remain visible without a download link.
