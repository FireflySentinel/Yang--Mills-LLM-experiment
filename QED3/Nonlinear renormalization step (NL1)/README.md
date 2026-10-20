# Nonlinear renormalization step (NL1)

**Disclaimer:** these documents are largely LLM-created. Their correctness has not been satisfactorily verified.

Project codename: **NL1**.

- **NLO1** — [The exact nonlinear renormalization step](NLO1.pdf).
- **AI-written manuscript:** **NLM1** — *The exact nonlinear renormalization step for lattice QED in three dimensions* (manuscript to be added).
- **Human-written manuscript:** to be added.

## Role in the QEM1 assembly

Exact conditional nonlinear step and connected logarithm.

QEO1 contracts: [S12](../QEO1.pdf#page=97), [S13](../QEO1.pdf#page=99), [S14](../QEO1.pdf#page=101), [S15](../QEO1.pdf#page=27).

Related inputs: [MBM1](../Maxwell%20block%20analysis%20%28MB1%29/README.md), [FBM1](../Chamber%20fermion%20block%20analysis%20%28FB1%29/README.md), [RNM1](../Relevant%20extraction%20and%20normalized%20contraction%20%28RN1%29/README.md). Read their hypotheses at the cited results.

## Main statements

The setting and principal theorem below are reproduced from **NLM1**. Notation and numbered references follow that manuscript; references to other documents use their codenames. The referenced activity spaces, maps and imported hypotheses remain part of the statement.

We consider one block transformation of noncompact lattice QED with
four-component chamber fermions. The photon field is periodic on
$`\eta\mathbb{Z}^3/\ell\mathbb{Z}^3`$, and spinors are antiperiodic in every coordinate.
Each photon site carries $`48`$ chamber labels. The chamber measure is
$`\eta^3/48`$; barred and unbarred Grassmann generators are independent.
The Dirac stencil, block averages and weighted transposes are those of
FBM1 (Section 1).

Fix $`0<\rho<1`$, odd $`L\ge4^8`$, an integer power $`M`$ of $`L`$ with $`M\ge L^2`$ and $`M>4L`$,
and $`k\in\mathbb{Z}_{\ge0}`$. Put $`\eta=L^{-k}`$, $`e=e_k\in(0,1)`$,
$`e_{k+1}=\sqrt L e_k`$, and $`0<\mu\le1/L`$; the scaled reference
mass is $`L\mu`$. Both charges are at most the common ceiling $`e_{\mathrm{prim}}`$ of the
photon and fermion estimates specified in the theorem below. Require
$`\ell/(LM)`$ and $`\ell/(L^2M)`$ to be odd integers at least $`13`$.
Fix an integer $`r\ge2`$. For $`v=-\log e`$, put

```math
r_k=\min\{L^i:i\ge0\text{ an integer},\ L^i\ge v^r\},
 \qquad \ell\ge Mr_k .
```

An activity in $`K_k^{x,\mathbb{C}}`$ is a balanced family of Grassmann
polynomials in ordinary and ordered-pair generators, holomorphic on
$`\widetilde R_k\times\mathfrak X_k`$, local in its polymer and its
connection bonds, and covariant under the lattice, independent local
real-gauge and charge-conjugation actions. The real space $`K_k^x`$
also satisfies the antilinear reality identity. We use exactly the
domains, pair support and actions of RNM1 (Section 2),
recalled in Section 2. In particular, $`\widetilde R_k`$
permits independent local real gauges; it imposes no bound on a real
harmonic part. With $`d_M(X)`$ the connected-net length divided by $`M`$,
the weights and norm are

```math
h_k=(e_k^{-1/4},e_k^{-1/4+\varepsilon}),\qquad
 \|\mathscr E\|_k^x=\sup_X\exp(\kappa d_M(X))
       \sup_{\widetilde R_k\times\mathfrak X_k}\|\mathscr E(X)\|_{h_k}.
```

The coefficient norm is the sum of absolute ordered coefficients
times their generator weights. Set

```math
w_k^{\mathrm m}=e_k^{3/4-8\varepsilon},\quad
 w_k^{\mathrm E}=e_k^{1/4-7\varepsilon},\quad
 \mathrm{Ball}_k^x(c)=
 \{(m,\mathscr E):|m|\le cw_k^{\mathrm m},\ {}
                 \|\mathscr E\|_k^x\le cw_k^{\mathrm E}\}.
```

At $`k=0`$ the activity is required to be zero. The interaction mass
$`m`$ is distinct from the positive reference mass $`\mu`$. Put
$`n_k=\ell^3`$, $`n_{k+1}=(\ell/L)^3`$, and $`q=e_k`$ at $`k=0`$.
The real photon domain is
$`\mathrm{Dom}_j=\{A:H_j^{\mathrm{ph}}A\in\frac14\widetilde R_j\}`$.
The density $`\mathscr F_j^x`$ and normalized block operator $`\mathbf T_k^x`$
are defined by (38) and
(39); the latter integrates over
$`\mathrm{Box}_k=\{\sup_\Upsilon|\zeta(\Upsilon)|\le p_{0,k}\}`$.

The quantitative constants are

```math
\begin{gathered}
 \bar\varepsilon=1/200,\qquad
 0<\varepsilon\le\bar\varepsilon,\qquad 1-\varepsilon<\alpha<1,\\[0pt]
 c_X=54,\quad \kappa_0=54\log72,\quad K_0=\exp(\kappa_0)/36,\quad
 c_{\rm rb}=c_XK_0,\quad c_{\rm fl}=61c_{\rm rb},\\[0pt]
 c_C=3L^{9/2},\quad b=1,\quad b_L=b/L,\quad b_-=1-L^{-1},\\[0pt]
 C_T=2\exp(3/2)
       [1+b_-^{-1}(54L\exp(6)+12\exp(1)+1)],\\[0pt]
 c_S=10^5c_X^5K_0^5\exp(6\kappa),\qquad
 \kappa_w=\kappa+\kappa_0+3 .
 \end{gathered}
```

The primitive constants $`C_w,\gamma_w,\alpha_0>0`$, the photon
local-gauge constant $`C_B`$, and the two exponential-sum bounds
$`c_\gamma`$ are those of the photon and fermion families in hypothesis (i) below; $`C_w,c_\gamma\ge1`$.

**Theorem A (The exact nonlinear step).**

In the setting above, assume the following simultaneous hypotheses.

**(i)**  Use a single system of photon and fermion primitives on this
torus. Assume the full hypotheses and conclusions of
MBM1 (Theorems A–B and Proposition 5.1)
and
FBM1 (Theorem A, Propositions 4.1,
4.2,
4.3,
6.1 and
6.2).
Use common constants $`(\alpha_0,\gamma_w,\kappa_w;C_w)`$ for their
analytic kernel and short Hölder bounds on
$`|s_a|\le M^{\alpha_0}`$. This assumption includes component
restriction, row vanishing, local read bonds, the exact operators at
$`s=1`$, and their lattice, gauge, transpose and reality identities.
At $`k=0`$ retain the stated diagonal families and chamber covariance.
Use the weighted integration conventions of
FBM1 (Theorem B and Proposition 5.1)
and the extraction, reconstruction and geometry of
RNM1 (Theorems A–B and Appendix B).
The fine inverses required for reconstruction exist at both signs
of every total connection in $`\widetilde G_k`$ by the fermion hypothesis.

**(ii)**  The extraction and scaling parameters satisfy

```math
\begin{gathered}
 L^{1/8-3\bar\varepsilon/2}\ge2400,\qquad e^\varepsilon\le\tfrac14,\qquad
 160L^{1+3\varepsilon/2}Me^\varepsilon\le1,\\[0pt]
 9ML^\varepsilon e^{2\varepsilon}\le1,\qquad
 90c_XLMe^\varepsilon\le1,\\[0pt]
 \kappa\ge7\kappa_0+7,\qquad
 L(\kappa-6\kappa_0-4)-1\ge\kappa .
 \end{gathered}
```

**(iii)**  The weakening radius and constants satisfy

```math
C_w\ge4\exp(2\gamma_w)M^{27\alpha_0},\qquad
 M^{\alpha_0}-1\ge\exp\big((2L+1)^3\kappa+\log(6c_X)\big).
```

For the localizations, connected expansion, scaling and determinant
reblocking, assume

```math
\begin{aligned}
&p_{0,k}\le e^{-\varepsilon/4},\qquad
       12\exp(-p_{0,k}^2/2)\le e^7,\qquad
       2e^{5\varepsilon/2}\le1,\qquad
       c_{\mathrm{fl}}e^\varepsilon\le1,\qquad3Me^\varepsilon\le1,
                                                        \\[0pt]
 &2c_CC_w^2c_\gamma^2e^{\varepsilon/4}\le1,\qquad
       16c_Xc_\gamma C_wC_T^2M^3e^{\varepsilon/2}\le1,\qquad
       96M^3e^{1/4}\le1,                                \\[0pt]
 &32C_wC_Te^{3\varepsilon/2}\le1,\qquad
       88M^3e^{1/4-6\varepsilon}\le1,\qquad
       112C_w^2c_\gamma e^{2\varepsilon}\le3,             \\[0pt]
 &c_Se^{1/4-5\varepsilon}\le1,\qquad
       c_SL^3e^\varepsilon\le1,\qquad e^\varepsilon\le\tfrac14,\qquad
       8c_{\mathrm{rb}}L^3C_dM^3e^{2\varepsilon}\le1.
\end{aligned}
```

Here $`C_d`$ is the local determinant constant in hypothesis (i).

**(iv)**  For fixed positive exponents $`p_0,p`$, put
$`p_{0,k}=v^{p_0}`$, $`p_k=v^p`$. The photon box and domain bounds
and the determinant gain require

```math
\begin{gathered}
 p_{0,k}\le e^{-\varepsilon/4},\qquad
 12\exp(-p_{0,k}^2/2)\le e^7,\qquad
 8C_Bp_k\le e^{-3/4+3\varepsilon},\\[0pt]
 8e^{3/4-7\varepsilon/2}\le1,\qquad L^{3/4}\ge8/3,\qquad
 v\ge9,\qquad 8M(v/4+4)e^\varepsilon\le1,\\[0pt]
 e^{1/4}+e^\varepsilon<1,\qquad
 4e^{1/4+2\varepsilon}+2e^{3\varepsilon}\le1 .
 \end{gathered}
```

There is a local connected logarithm $`E_k^\#(m,\mathscr E)`$ on
$`\widetilde R_k^-\times\mathfrak X_k`$ for every complex datum in
$`\mathrm{Ball}_k^x(4)`$. It has the lattice symmetry with
$`LM`$ translations, independent local real-gauge covariance and
charge conjugation. Each monomial is balanced; real data give the
reality identity. Its scaled sum

```math
E_k^*(m,\mathscr E)(Y;A,C)
   =\sum_{\bar X^L=LY}S_LE_k^\#(m,\mathscr E)(X;A_L,C_L)
```

belongs to $`K_{k+1}^{x,\mathbb{C}}`$ and has norm at most
$`e_k^{1/4-6\varepsilon}`$. Here $`A_L(b)=L^{-1/2}A(b/L)`$;
$`S_L`$ scales ordinary legs by $`L^{-1}`$ and pair legs by
$`L^{-1-\alpha}`$, and $`\bar X^L`$ is the union of $`LM`$-cubes
containing $`X`$. The correction is norm continuous on each affine
complex line's closed allowed set and norm analytic in its interior.
For two data in $`\mathrm{Ball}_k^x(1)`$,

```math
\|E_k^*(m_1,\mathscr E_1)-E_k^*(m_2,\mathscr E_2)\|_{k+1}^x
 \le e_k^{1/4-6\varepsilon}
 \left(\frac{|m_1-m_2|}{w_k^{\mathrm m}}+
       \frac{\|\mathscr E_1-\mathscr E_2\|_k^x}{w_k^{\mathrm E}}\right).
```

The second quotient is omitted at $`k=0`$.

For the local determinant terms of
Proposition 6.1 of FBM1, put

```math
\delta E_k^{\mathrm{det}}(X;\mathscr A,\mathscr C)
       =E_k^d(X,\mathscr A+\mathscr C)-E_k^d(X,\mathscr C),
 \qquad
 E_k^{\mathrm{det}}(X,\mathscr C)
       =E_k^d(X,\mathscr C)-E_k^d(X,0).
```

These are scalar activities. We use reblocking
$`\mathcal L`$ from (34) of RNM1.
The maps $`R`$, $`(\cdot)^{\mathrm{nat}}`$, $`m(\cdot)`$ and
$`\varepsilon_{\mathrm v}(\cdot)`$ are the subtraction, adjustment and
extraction maps of RNM1 (Theorem A).
The outgoing maps are

```math
\begin{aligned}
\mathscr E^+&=\mathcal L(R\mathscr E)^{\mathrm{nat}}
                        +\mathcal L\delta E_k^{\mathrm{det}}
                        +E_k^*(m,\mathscr E), \\[0pt]
 m^+&=L(m+m(\mathscr E)),\\[0pt]
 \varepsilon^{\mathrm v,+}
       &=L^3(\varepsilon^{\mathrm v}
                  +\varepsilon_{\mathrm v}(\mathscr E)
                                      +\delta\varepsilon_k^0),\\[0pt]
 \mathfrak P_{k+1}(Y,\mathscr C')
       &=\sum_{\bar X^L=LY}
           \big(\mathfrak P_k(X,\mathscr C'_L)
                          +E_k^{\mathrm{det}}(X,\mathscr C'_L)\big).
\end{aligned}
```

Here $`\mathfrak P_k`$ is any given family of scalar
functions of the external slot.

Let $`\varepsilon^{\mathrm v},m`$ be real,
$`\mathscr E\in K_k^x`$, and
$`(m,\mathscr E)\in\mathrm{Ball}_k^x(1)`$, with
$`\mathscr E=0`$ at $`k=0`$. For $`A'\in\mathrm{Dom}_{k+1}`$
with arbitrary harmonic part and
$`\mathscr C'\in\mathfrak X_{k+1}`$, the exact density satisfies

```math
\mathbf T_k^x\mathscr F_k^x[\varepsilon^{\mathrm v},m,\mathscr E]
   =\mathscr F_{k+1}^x
            [\varepsilon^{\mathrm v,+},m^+,\mathscr E^+],
```

with external scalar families $`\mathfrak P_k`$ and
$`\mathfrak P_{k+1}`$ on the respective sides.
Its integral satisfies

```math
y_{k+1}^x(A';\mathscr C')
  =\int_{\mathrm{Box}_k}\mathrm{d}\mu_I(\zeta)\,
        y_k^x(A_k^{\min}(A')+\mathrm{Sq}_k\zeta;\mathscr C'_L),
```

where $`y_j^x=\int\mathrm D\Psi\,\mathscr F_j^x`$ with the
data and scalar family of that level. The photon integral uses the
unnormalized Gaussian restriction to the box.
Moreover $`\mathscr E^+\in K_{k+1}^x`$ and

```math
\begin{aligned}
\|\mathscr E^+\|_{k+1}^x
 &\le c_{\mathrm{fl}}L^{-1/4+2\varepsilon}\|\mathscr E\|_k^x
           +e_{k+1}^{1/4-2\varepsilon}+e_k^{1/4-6\varepsilon},
                                      \\[0pt]
 |m^+-Lm|
 &\le Lc_{\mathrm{fl}}e_k^{1/2}\|\mathscr E\|_k^x,
                                      \\[0pt]
 |\varepsilon^{\mathrm v,+}-L^3\varepsilon^{\mathrm v}|
 &\le L^3(c_{\mathrm{fl}}\|\mathscr E\|_k^x+e_k^7).
\end{aligned}
```

At level zero this formula integrates all $`192n_0`$
incoming pairs of generators, with chamber measure $`1/48`$,
and leaves $`4n_1`$ outgoing pairs. Its data are

```math
\mathscr E^+=\mathcal L\delta E_0^{\mathrm{det}}+E_0^*(m,0),
 \quad m^+=Lm,\quad
 \varepsilon^{\mathrm v,+}
                         =L^3(\varepsilon^{\mathrm v}+\delta\varepsilon_0^0).
```

In particular
$`0\le\varepsilon^{\mathrm v,+}-L^3\varepsilon^{\mathrm v} \le L^3q^7`$.
All maps commute with setting the external connection to zero.
The estimates are independent of the side and harmonic part, for
one primitive system satisfying the stated hypotheses. The theorem
asserts one step on the two admitted sides; it makes no assertion
that the outgoing datum lies in the next unit ball.


## Navigation

[QEM1 assembly index](../README.md). The published PDFs retain their mathematical text. Links to published outlines use their repository locations; links to withheld manuscripts open the corresponding README. Citations to material outside this assembly remain visible without a download link.
