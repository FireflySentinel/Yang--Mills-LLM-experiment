# Maxwell block analysis (MB1)

**Disclaimer:** these documents are largely LLM-created. Their correctness has not been satisfactorily verified.

Project codename: **MB1**.

- **MBO1** — [Maxwell block minimization and Gaussian fluctuations](MBO1.pdf).
- **MBM1** — *Maxwell block minimization and Gaussian fluctuations* (manuscript to be added).

## Role in the QEM1 assembly

Photon minimization and constrained Gaussian primitives.

QEO1 contracts: [S03](../QEO1.pdf#page=81), [S04](../QEO1.pdf#page=83), [S05](../QEO1.pdf#page=85).

## Main statements

The setting and principal theorem below are reproduced from **MBM1**. Notation and numbered references follow that manuscript; references to other documents use their codenames.

Fix an odd integer $`L\ge5`$, a power $`M=L^m\ge L^2`$, and
$`0<\alpha<1`$. At level $`k\ge0`$, set
$`\eta=L^{-k}`$ and $`N=\eta^{-1}`$.
We use real periodic cochains on
$`T_{\eta,\ell}=\eta\mathbb{Z}^3/\ell\mathbb{Z}^3`$, with pairing
$`\eta^3\sum`$ on each component. Differences are normalized by
the mesh:

```math
\partial_\mu f(x)=\eta^{-1}(f(x+\eta e_\mu)-f(x)),\qquad
 (d\lambda)_\mu=\partial_\mu\lambda,\qquad
 (d\mathscr A)_{\mu\nu}
   =\partial_\mu\mathscr A_\nu-\partial_\nu\mathscr A_\mu.
```

Write $`\delta=d^T`$ and $`\Delta_{\mathrm{sc}}=\delta d`$
on scalars. Distances between sites are periodic sup distances.
For bonds use their initial sites, and for coordinate supports use
the minimum distance between their points.
The local regularity norms $`\|B\|_{i,W}`$, $`i=1,2,3`$, mean
the supremum, first-difference supremum, and $`\alpha`$-Hölder
first-difference supremum on $`W`$, respectively. Only contained
bonds and difference cells enter these local norms.
Elsewhere $`\|B\|_2`$ denotes the quadratic norm; the domain
section explicitly uses $`\|B\|_i`$ for the three global
regularity norms.
Hölder differences compare parallel output bonds at distance
in $`(0,1]`$, with the input column and derivative direction fixed.

For $`z\in\mathbb{Z}^3/\ell\mathbb{Z}^3`$, put
$`\Delta_z=\{c:|c-z|_\infty<1/2\}`$.
The partition $`M`$-cubes have side $`M`$ and centers in
$`M\mathbb{Z}^3/\ell\mathbb{Z}^3`$.
The scalar, bond, and plaquette averages to the unit lattice are

```math
\begin{aligned}
(\mathbf Q_k\lambda)(z)
   &=\eta^3\sum_{c\in\Delta_z}\lambda(c),\\[0pt]
 (\mathbf Q_k\mathscr A)_\mu(z)
   &=\eta^3\sum_{c\in\Delta_z}\sum_{j=0}^{N-1}
          \eta\mathscr A_\mu(c+j\eta e_\mu),\\[0pt]
 (\mathbf Q_k^{(2)}F)_{\mu\nu}(z)
   &=\eta^3\sum_{c\in\Delta_z}\sum_{i,j=0}^{N-1}
          \eta^2F_{\mu\nu}(c+i\eta e_\mu+j\eta e_\nu).
\end{aligned}
```

All sums are taken on the periodic covering lattice.
Let $`\mathcal R_k`$ be the orthogonal projection onto
$`\Delta_{\mathrm{sc}}(\ker\mathbf Q_k)`$ in scalar cochains.
The Landau representative $`H_k^{\mathrm{ph}}A`$ minimizes
$`\|d\mathscr A\|_2^2`$ under

```math
\mathbf Q_k\mathscr A=A,\qquad \mathcal R_k\delta\mathscr A=0.
```

Set

```math
\Delta_k=(dH_k^{\mathrm{ph}})^TdH_k^{\mathrm{ph}}.
```

For one block step on the unit lattice, let
$`B(y)=\{z:|z-y|_\infty<L/2\}`$, $`y\in L\mathbb{Z}^3/\ell\mathbb{Z}^3`$.
The scalar average is
$`\mathbf Q\lambda(y)=L^{-3}\sum_{z\in B(y)}\lambda(z)`$.
On bonds put

```math
(\mathbf QA)(y,y+Le_\mu)
   =L^{-4}\sum_{z\in B(y)}A(\Gamma_{z,z+Le_\mu}),\qquad
 (\tau A)(y,z)=\tfrac16\sum_\pi A(\Gamma^\pi(y,z)).
```

Here $`A(\Gamma)`$ is the oriented bond sum; the first paths are
straight, while the latter change coordinates in each of the six
orders. Write $`\mathcal Z=\{Z:\mathbf QZ=0,\ \tau Z=0\}`$.
For a coarse field $`A'`$ on side $`\ell/L`$, set
$`A'_L(b)=L^{-1/2}A'(b/L)`$.

**Theorem A.**

Assume that $`\ell/(LM)`$ is an odd integer at least $`13`$.
There are constants $`C_P^{\mathrm{ph}}>0`$ and
$`0<\gamma_P\le1`$, depending only on $`L,\alpha`$, for which
the following assertions hold uniformly in $`k,\ell`$.

The minimizer $`H_k^{\mathrm{ph}}`$ exists uniquely, is real
linear, and satisfies $`\mathbf Q_kH_k^{\mathrm{ph}}=1`$.
It preserves constants and closed fields, and $`H_0^{\mathrm{ph}}=1`$.
Each of its kernel, first-difference kernel, and short Hölder
first-difference kernel is bounded by
$`C_P^{\mathrm{ph}}e^{-\gamma_Pd(b,b')}`$.
Also

```math
|\Delta_k(b,b')|\le C_P^{\mathrm{ph}}e^{-\gamma_Pd(b,b')}.
```

There is a real coordinate space $`V_k`$ with an orthonormal
basis $`\{\Upsilon\}`$, each vector supported in an $`L`$-block
or on a noncentral face bond, and a bijection $`C:V_k\to\mathcal Z`$.
The basis choices are translates of one fixed block basis, and

```math
\dim V_k=(2-2L^{-3})\ell^3,\qquad
 \|z\|_2\le\|Cz\|_2\le\sqrt{5L^3}\|z\|_2.
```

The form $`\widetilde\Delta_k=C^T\Delta_kC`$ is strictly positive,
with upper and lower bounds depending only on $`L`$, and

```math
\big|\widetilde\Delta_k^{-1/2}(\Upsilon,\Upsilon')\big|
 \le C_P^{\mathrm{ph}}e^{-\gamma_Pd(\Upsilon,\Upsilon')}.
```

Here the distance on the right is between basis supports.

For every real $`A'`$, the minimum $`A_k^{\min}(A')`$ of
$`\langle A,\Delta_kA\rangle`$ under
$`\mathbf QA=A'_L,\ \tau A=0`$ exists uniquely. With
$`\mathrm{Sq}_k=C\widetilde\Delta_k^{-1/2}`$,

```math
\begin{aligned}
 &\langle A_k^{\min}(A')+\mathrm{Sq}_k\zeta,\,
   \Delta_k(A_k^{\min}(A')+\mathrm{Sq}_k\zeta)\rangle\\[0pt]
 &\hspace{35mm}=\|dH_{k+1}^{\mathrm{ph}}A'\|_2^2+\|\zeta\|_2^2.
 \end{aligned}
```

The operator at level $`k+1`$ on the right is formed on side
$`\ell/L`$ and mesh $`\eta/L`$. The harmonic part of $`A'`$
is arbitrary. The probability law on the affine constraint space
with density proportional to
$`\exp(-\langle A,\Delta_kA\rangle/2)`$, relative to its Euclidean
volume, is the image of the standard product Gaussian $`\mu_I`$
under $`A=A_k^{\min}(A')+\mathrm{Sq}_k\zeta`$.
For every $`q\ge1`$,

```math
\mu_I\{\sup_\Upsilon|\zeta(\Upsilon)|\le q\}
   =e^{-\ell^3\delta\varepsilon^0(q)},\qquad
 0\le\delta\varepsilon^0(q)\le12e^{-q^2/2}.
```

If $`\square`$ is a partition $`M`$-cube and
$`\square^\dagger`$ its concentric enlargement of side
$`(2L+1)M`$, then for every real $`A`$ there is an independent
real gauge $`\nu`$ on this nonwrapping enlargement such that

```math
\|H_k^{\mathrm{ph}}A-d\nu\|_{i,\square^\dagger}
       \le C_B\|dA\|_\infty,\qquad i=1,2,3,
```

where $`C_B`$ depends only on $`L,M,\alpha`$; the subscripts
$`i`$ denote the three regularity norms.

Finally, let $`\ell_2=J\ell_1`$, with $`J`$ odd and both sides
as above, and use the same translated block basis. Periodic
pullback intertwines $`H_k^{\mathrm{ph}},\Delta_k,C, \widetilde\Delta_k,(\widetilde\Delta_k+xI)^{-1}`$ for $`x\ge0`$,
$`\widetilde\Delta_k^{-1/2},\mathrm{Sq}_k`$, and
$`A_k^{\min}`$ on the two tori.

Theorem B of MBM1 (Section 6, “Domains for block integration”) gives additional domain estimates under the geometry, weakening and small-charge hypotheses stated there.


## Navigation

[QEM1 assembly index](../README.md). The published PDFs retain their mathematical text. Links to published outlines use their repository locations; links to withheld manuscripts open the corresponding README. Citations to material outside this assembly remain visible without a download link.
