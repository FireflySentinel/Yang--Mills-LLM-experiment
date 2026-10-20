# Continuum existence (CE1)

**Disclaimer:** these documents are largely LLM-created. Their correctness has not been satisfactorily verified.

Project codename: **CE1**.

- **CEO1** — [Continuum limits from second-moment bounds](CEO1.pdf).
- **CEM1** — *Gaussian domination and structural properties of continuum limits* (manuscript to be added).

## Role in the QEM1 assembly

Gaussian/correlation stability, compactness, structural inheritance and prescribed-parent recovery.

QEO1 contracts: [B3](../QEO1.pdf#page=18), [A1](../QEO1.pdf#page=20).

CEO1 covers compactness only. Current compact-link IVM1 is not the real-curvature input. The selected common bare sequence is required in the QED3 application.

Related inputs: [LPM1](../Infinite-lattice%20reflection%20positivity%20%28LP1%29/README.md), [CVM1](../Cover%20agreement%20and%20common%20tuning%20%28CV1%29/README.md). Read their hypotheses at the cited results.

## Main statements

The setting and principal theorems below are reproduced from **CEM1**. Notation and numbered references follow that manuscript; references to other documents use their codenames.

Let $`\mathcal S=\mathcal S(\mathbb{R}^d;\mathbb{R}^r)`$ be the real Schwartz space
and $`\mathcal S'`$ its continuous dual. Write $`e_\alpha`$ for the
standard basis of $`\mathbb{R}^r`$. For the normalized real Hermite functions
$`h_k`$, $`k\in\mathbb{N}_0^d`$, set

```math
(1-\Delta+|y|^2)h_k=\lambda_k h_k,\qquad
 \lambda_k=2|k|_1+d+1,\qquad |k|_1=k_1+\cdots+k_d.
```

For $`t>0`$ we use the separable Hilbert space

```math
H_{-t}=\{F\in\mathcal S':\|F\|_{-t}<\infty\},\qquad
 \|F\|_{-t}^2=
 \sum_{\alpha=1}^r\sum_{k\in\mathbb{N}_0^d}
       \lambda_k^{-2t}|F(h_ke_\alpha)|^2.
```

All weak convergence of probability laws on this space refers to
its norm topology.

Extend each real distribution complex linearly to
$`\mathcal S_{\mathbb C}=\mathcal S(\mathbb{R}^d;\mathbb C^r)`$.
For a law $`P`$, its smeared $`n`$-point correlation is
$`S_n^P(f_1,\ldots,f_n)=\mathbb{E}_P\prod_{j=1}^n F(f_j)`$ whenever
this expectation exists.

**Theorem A (Gaussian domination and convergence of correlations).**

Fix integers $`d,r\ge1`$ and a real number $`t>0`$. Let $`P_j`$ and $`P`$ be Borel probability
laws on $`H_{-t}`$ such that $`P_j\Longrightarrow P`$. Suppose

```math
\mathbb{E}_{P_j}e^{F(f)}\le e^{\|f\|_2^2/2}
 \qquad(j\ge1,\ f\in\mathcal S).
```

Then

```math
\mathbb{E}_P e^{F(f)}\le e^{\|f\|_2^2/2}
 \qquad(f\in\mathcal S).
```

For every finite family $`f_1,\ldots,f_m\in\mathcal S_{\mathbb C}`$,
the functions

```math
Z_j(z)=\mathbb{E}_{P_j}\exp\left(\sum_{a=1}^m z_aF(f_a)\right),
 \qquad
 Z(z)=\mathbb{E}_P\exp\left(\sum_{a=1}^m z_aF(f_a)\right)
```

are entire on $`\mathbb C^m`$. They satisfy $`Z_j\to Z`$ locally
uniformly, with every complex derivative. In particular, for
every $`n\ge1`$ and $`f_1,\ldots,f_n\in\mathcal S_{\mathbb C}`$,

```math
S_n^{P_j}(f_1,\ldots,f_n)\longrightarrow
 S_n^P(f_1,\ldots,f_n).
```

On the common domain

```math
D_f=\left\{z\in\mathbb C^m:
                 \sum_{a=1}^m|z_a|\|f_a\|_2<2/5\right\},
```

all $`Z_j`$ and $`Z`$ satisfy $`|Z_j-1|<1/2`$ and $`|Z-1|<1/2`$.
Their principal logarithms converge locally uniformly on $`D_f`$,
with every derivative. Thus all joint cumulants converge, where

```math
\kappa_n^P(f_1,\ldots,f_n)
 =\left.\partial_{z_1}\cdots\partial_{z_n}
       \log\mathbb{E}_P\exp\left(\sum_{a=1}^n z_aF(f_a)\right)
   \right|_{z=0},
```

and $`\kappa_n^{P_j}`$ is defined in the same way.

**Theorem B (Continuum limits of lattice fields).**

Fix integers $`d,r\ge1`$, offsets $`t_1,\ldots,t_r\in[0,1]^d`$,
and a set $`I\subset(0,1]`$ with $`0`$ in its closure. For each
$`a\in I`$, let $`\nu_a`$ be a Borel probability law on
$`\mathbb{R}^{\mathbb{Z}^d\times\{1,\ldots,r\}}`$ with the coordinate product
topology. Suppose there is a constant $`0\le C<\infty`$ such that

```math
\mathbb{E}_{\nu_a}\left|\sum_{\alpha,x}b_\alpha(x)u_\alpha(x)\right|^2
 \le C\sum_{\alpha,x}|b_\alpha(x)|^2
```

for every $`a\in I`$ and every finitely supported real coefficient
array $`b`$. Define

```math
(F_a)_\alpha(y)=a^{-d/2}u_\alpha(x)
 \quad\text{for }y\in Q_{a,\alpha,x}
 :=a\bigl(x+t_\alpha+[-1/2,1/2)^d\bigr).
```

Then $`F_a`$ is almost surely a real tempered distribution, and

```math
\mathbb{E}_{\nu_a}|F_a(f)|^2\le C\|f\|_{L^2(\mathbb{R}^d;\mathbb{R}^r)}^2
 \qquad(f\in\mathcal S).
```

For every fixed $`t>d/2`$, these fields have Borel realizations in
$`H_{-t}`$ whose laws are uniformly tight. Consequently, for every
sequence $`a_j\in I`$ tending to zero there are a subsequence
$`a_{j_\ell}`$ and a Borel probability measure $`\mu`$ on $`H_{-t}`$
such that

```math
\mathcal L(F_{a_{j_\ell}})\ \Longrightarrow\ \mu.
```

Along this subsequence the pairings with every finite family of
Schwartz tests converge jointly in distribution to their pairings
under $`\mu`$.

For the structural assertion, identify the component space $`\mathbb{R}^r`$ with a real inner-product space $`V`$, and let $`W`$ be another
finite-dimensional real inner-product space.
Fix an orthogonal representation $`\rho:O(d)\to O(V)`$.
For $`g(x)=Qx+b`$, use the actions

```math
(g\cdot f)(x)=\rho(Q)f(Q^{-1}(x-b)),\qquad
 (g\cdot F)(f)=F(g^{-1}\cdot f).
```

Invariance concerns the law as a random tempered distribution,
with the sigma-algebra generated by evaluations.
For an open set $`O`$, write $`\Sigma_O`$ for the sigma-algebra
generated by $`F(f)`$, $`f\in C_c^\infty(O;V)`$ real.
For an open half-space $`H^+`$ and an $`r`$-invariant law $`P`$,
where $`r`$ reflects in its
boundary, reflection positivity means

```math
\mathbb{E}_P[\overline{B(r\cdot F)}B(F)]\ge0
 \qquad\bigl(B\in L^2(\Sigma_{H^+},P)\bigr).
```

**Theorem C (Identities, symmetries and reflection positivity).**

Let $`P_j\Rightarrow P`$ weakly on $`H_{-t}`$, and suppose

```math
\mathbb{E}_{P_j}e^{F(f)}\le e^{\|f\|_2^2/2}
 \qquad(j\ge1,\ f\in\mathcal S\text{ real}).
```

Let $`D^*:C_c^\infty(\mathbb{R}^d;W)\to\mathcal S`$ be continuous and
linear. Let $`\mathcal G`$ be a group of Euclidean isometries
containing all translations and a finite set $`\mathcal R`$ of
reflections through the origin. Choose an open side $`H_r^+`$ for
each $`r\in\mathcal R`$. Assume:

**(i)**
For each $`\xi\in C_c^\infty(\mathbb{R}^d;W)`$ there are real
$`v_j(\xi)\in\mathcal S`$ such that $`F(v_j(\xi))=0`$,
$`P_j`$-almost surely, and
$`\|v_j(\xi)-D^*\xi\|_2\to0`$.

**(ii)**
For each $`g\in\mathcal G`$ there are real linear maps
$`T_{j,g}:\mathcal S\to\mathcal S`$ satisfying

```math
\mathbb{E}_{P_j}e^{iF(T_{j,g}f)}=\mathbb{E}_{P_j}e^{iF(f)},\qquad
 \|T_{j,g}f-g\cdot f\|_2\longrightarrow0
 \quad(f\in\mathcal S).
```

**(iii)**
For every $`r\in\mathcal R`$, every finite family of real
$`f_a\in C_c^\infty(H_r^+;V)`$, and every $`z_a\in\mathbb{C}`$,

```math
\sum_{a,b}\overline z_a z_b
 \mathbb{E}_{P_j}e^{iF(f_b-r\cdot f_a)}\ge0
```

for all sufficiently large $`j`$, depending on the family.

Then $`P`$ satisfies $`\mathbb{E}_Pe^{F(f)}\le e^{\|f\|_2^2/2}`$
for every real $`f\in\mathcal S`$, is
$`\mathcal G`$-invariant, and almost every $`F`$ satisfies
$`F(D^*\xi)=0`$ simultaneously for all $`\xi`$.
The law is reflection invariant and reflection positive at every
translate of every plane in $`\mathcal R`$.
Along the same sequence, all joint moments and cumulants of every
fixed finite family of Schwartz evaluations converge to those of $`P`$.


## Navigation

[QEM1 assembly index](../README.md). The published PDFs retain their mathematical text. Links to published outlines use their repository locations; links to withheld manuscripts open the corresponding README. Citations to material outside this assembly remain visible without a download link.
