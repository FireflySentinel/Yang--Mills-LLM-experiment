# Reference response (RR1)

**Disclaimer:** these documents are largely LLM-created. Their correctness has not been satisfactorily verified.

Project codename: **RR1**.

- **RRO1** — [Exact sources and normalized reference response](RRO1.pdf).
- **RRM1** — *Exact source identities and normalized reference response for lattice QED in three dimensions* (manuscript to be added).

## Role in the QEM1 assembly

Early source identities and later normalized reference response.

QEO1 contracts: [T05](../QEO1.pdf#page=110), [T06](../QEO1.pdf#page=111), [T07](../QEO1.pdf#page=112), [Q4R](../QEO1.pdf#page=36), [T12](../QEO1.pdf#page=116), [T13](../QEO1.pdf#page=118), [T14](../QEO1.pdf#page=120), [T15](../QEO1.pdf#page=121).

Early zero-flux/Wick identities feed TPM1; later response results import terminal bounds. These are separate result ports, not a whole-paper cycle.

Related inputs: [CVM1](../Cover%20agreement%20and%20common%20tuning%20%28CV1%29/README.md), [TPM1](../Terminal%20measure%20and%20pressure%20%28TP1%29/README.md). Read their hypotheses at the cited results.

## Principal statements

Notation and numbered references below follow **RRM1**. The imported construction and estimates are part of the hypotheses.

### Setting

We use the chamber regulator with weights $`(6,6\sqrt2,6\sqrt2,6)`$ and Wilson parameter $`0<\rho<1`$. The operator $`D^{\rm ch}[B]`$ acts on four-component spinors with $`48`$ chamber labels per site, antiperiodic in every coordinate; its argument $`B`$ is the bond phase. The stencil is recalled in Section 1.1.

Fix the block construction of (**QEM1**, Proposition 4.1 and Section 4.1–4.4), with its positive charge ceilings $`e_1\le e_0<1`$ and the common-pair theorem (**CVM1**, Theorem D). Thus $`L\ge13`$ is odd, $`M=L^m`$ with $`m\in\mathbb{Z}_{\ge2}`$, $`0<\alpha<1`$, $`1-\alpha<\varepsilon\le1/200`$, and the localization and cutoff powers are $`r_{\rm loc}=2`$, $`p_0=9`$, $`p=19`$. The fixed ceilings denoted by $`e_0,e_1`$ here are the $`\bar e_0,\bar e_1`$ of (**QEM1**); they are distinct from the running charge $`e_j`$ at $`j=0`$. These fixed constants include the photon and fermion inverse bounds, the exact block step and the terminal conditions. The parameter input is Proposition 4.1 of (**QEM1**), which supplies the construction and charge ceilings before any probe-dependent restriction. The response estimates are proved here.

For $`0<\bar m\le1`$ put

```math
h=L^{\lfloor\log_L\bar m^{-1}\rfloor},\qquad
 \eta=L^{-N},\qquad q=e\sqrt\eta,\qquad K=N+\log_Lh.
```

Let $`r_K`$ be the least nonnegative integer power of $`L`$ at least $`[-\log(e\sqrt h)]^2`$, and set

```math
R_{\rm top}=hMr_K,\qquad R^*=R_{\rm top}/L,\qquad
 n_*=R^*/\eta,\qquad \ell_c=R^*/(2L),\qquad N_*=8L^3.
```

The finite threshold $`N_{\rm ref}(e)`$ and stopping level on $`R^*`$ are those of (**CVM1**, Proposition 6.1 and (53)). For $`N\ge N_{\rm ref}(e)`$ use the real pair $`P_N(e)=(m_{0,N},\varepsilon_{0,N}^{\rm v})`$ selected on $`R_{\rm top}`$ by (**CVM1**, Theorem D), and write $`\boldsymbol\mu_N=\bar m\eta+m_{0,N}`$. This same pair is used for every source and every twist. Its vacuum factor cancels from the normalized response below.

Fix a real nonzero $`\beta\in C_c^\infty(\mathbb{R}^3;\Lambda^2)`$, put $`f=dd^*\beta`$, and let $`D_\beta`$ be the side of a least coordinate cube containing $`\mathrm{supp}\beta`$. Enlarge that cube by two in each direction to obtain $`Q_\beta`$ of side $`D_\beta^{\rm buf}=D_\beta+4`$ and center $`z_\beta`$. With $`J_\eta`$ denoting cube averaging and $`\delta_{\eta,\mu}`$ the centered difference, define the covering bond cochain

```math
\widehat a^o_\nu(x)=
 -\eta^{1/2}\sum_{\mu\ne\nu}
 (\delta_{\eta,\mu}J_\eta\beta_{\mu\nu})
                         (\eta x+\eta e_\nu/2).
\tag{1}
```

A placement $`v\in\eta\mathbb{Z}^3`$ is admitted when $`v+Q_\beta\subset[\ell_c/8,7\ell_c/8]^3`$. Translate the probe by $`v`$, reflect it into the cells indexed by $`\mathcal C_*=(\mathbb{Z}/2L\mathbb{Z})^3`$, and periodize on $`C(n_*)`$. The resulting cochains are $`\widehat a_c`$; the reflection maps and their orientation action are specified in Section 2. They have mutually orthogonal curvatures, all of squared norm $`v_\eta=\|d\widehat a^o\|_{\ell^2}^2`$.

Write $`C(n_*)=\mathbb{Z}^3/n_*\mathbb{Z}^3`$ with its oriented cubical cells. Let $`\gamma_{n_*}`$ be the standard Gaussian on its exact real two-cochains, with counting inner product. For such a curvature $`u`$, let $`A(u)`$ be its mean-zero transverse potential. Set $`H_{\theta,\nu}=\theta_\nu/(qn_*)`$ and $`a(t)=e^{-1}\sum_ct_c\widehat a_c`$. Define

```math
\mathring\Phi(t)=
 \frac{\displaystyle\int_{[-\pi,\pi]^3}\frac{\mathrm{d}\theta}{(2\pi)^3}
       \int\det\bigl(D^{\rm ch}[q(A(u)+H_\theta+a(t))]
                         +\boldsymbol\mu_N\bigr)\,\mathrm{d}\gamma_{n_*}(u)}
      {\displaystyle\int_{[-\pi,\pi]^3}\frac{\mathrm{d}\theta}{(2\pi)^3}
       \int\det\bigl(D^{\rm ch}[q(A(u)+H_\theta)]
                         +\boldsymbol\mu_N\bigr)\,\mathrm{d}\gamma_{n_*}(u)}.
\tag{2}
```

The denominator is positive, including when the tuned total mass has either sign. The free one-cell ratio uses the positive reference mass:

```math
N_0(t)=\frac{\det\bigl(D^{\rm ch}[q(t/e)\widehat a_0]
                                      +\bar m\eta\bigr)}
                   {\det\bigl(D^{\rm ch}[0]+\bar m\eta\bigr)},
 \qquad c_m=N_0^{(m)}(0),\quad m=2,4.
\tag{3}
```

These are ordinary derivatives of the ratio. Put

```math
\Theta_m^{(0)}=
 \left|\left[\prod_{c\in\mathcal C_*}
           (\partial_{t_c}^m-c_m)\right]\mathring\Phi(0)
                                      \right|^{1/N_*},\qquad
 \mathfrak e=\tfrac12(1/4-9\varepsilon)-12\varepsilon>0.
```

### Regulator and elementary conventions

Let $`\sigma_\mu`$ be the Pauli matrices and $`\gamma_\mu=\sigma_3\otimes\sigma_\mu`$. The labels $`g\in O_{\rm cub}=O(3)\cap\mathrm{GL}(3,\mathbb{Z})`$ are the signed permutation matrices. Let $`s_0`$ reverse coordinate three, $`s_1,s_2`$ exchange $`(2,3)`$ and $`(1,2)`$, and let $`r_{e_1}`$ reverse coordinate one. Put

```math
n_0=e_3,\quad n_1=(e_2-e_3)/\sqrt2,\quad
 n_2=(e_1-e_2)/\sqrt2,\quad n_3=-e_1,\qquad
 M_i(g)=\tfrac12w_i(\rho+\gamma\cdot gn_i).
```

On a unit torus the chamber operator is

```math
\begin{split}
 (D^{\rm ch}[B]\psi)(c,g)={}&
 \sum_{i=0}^2M_i(g)\bigl(\psi(c,g)-\psi(c,gs_i)\bigr)\\[0pt]
 &+M_3(g)\bigl(\psi(c,g)
       -\mathrm e^{iB(c,c+ge_1)}\psi(c+ge_1,gr_{e_1})\bigr).
 \end{split}
\tag{6}
```

Reversed bonds carry the negative cochain value. We write $`D_A=D^{\rm ch}[qA]`$ in the unit-lattice source identities. At mesh $`\eta_j`$, the external hop and the bond phase have the corresponding factors $`\eta_j^{-1}`$ and $`e_j\eta_j`$. The spinor pairing has weight $`1/48`$ per chamber label; its constant weight does not change a finite-dimensional determinant.

For smooth functions,

```math
J_\eta v(y)=\eta^{-3}\int_{[-\eta/2,\eta/2]^3}v(y+z)\,\mathrm{d} z,
 \qquad
 \delta_{\eta,\mu}v(y)=
 \frac{v(y+\eta e_\mu/2)-v(y-\eta e_\mu/2)}{\eta}.
```

We use $`\tau_vf(x)=f(x-v)`$ and the seminorm $`|\beta|_{C^j}=\max_{\mu<\nu,|\alpha|\le j} \|\partial^\alpha\beta_{\mu\nu}\|_\infty`$. Counting cochain pairings are bilinear after complexification. Distances are periodic sup distances. The symbol $`e`$ is the physical charge; numerical exponentials are written $`\exp(\cdot)`$ or $`\mathrm e`$.

### Cell geometry and probe constants

Put

```math
\begin{aligned}
 a'_{\eta,\nu}&=-\sum_{\mu\ne\nu}\delta_{\eta,\mu}\beta_{\mu\nu},\\[0pt]
 f^\eta_{\mu\nu}&=\delta_{\eta,\mu}a'_{\eta,\nu}
                         -\delta_{\eta,\nu}a'_{\eta,\mu}.
\end{aligned}
\tag{7}
```

On the physical lattice $`\eta\mathbb{Z}^3`$ set

```math
 b_{\eta,\mu\nu}(c)
       =(J_\eta\beta_{\mu\nu})
                       (c+\eta(e_\mu+e_\nu)/2),\qquad
 a_\eta^o=d_\eta^*b_\eta.
```

Here $`d_\eta`$ is the mesh-normalized forward cochain differential and $`d_\eta^*`$ its adjoint for the pairing $`\eta^3\sum`$. The adjoint formula gives

```math
 a_{\eta,\nu}^o(c)=(J_\eta a'_{\eta,\nu})(c+\eta e_\nu/2).
\tag{8}
```

Transport to the unit lattice and define

```math
 \hat{\mathfrak a}_\eta^o(x,x+e_\nu)
                    =\eta^{1/2}a_{\eta,\nu}^o(\eta x).
```

Its coboundary uses unscaled unit-lattice differences.

Form $`\widehat{\mathfrak a}`$ with $`\tau_v\beta`$ as in (8), and periodize it on $`C(n_*)`$, $`n_*=R^*/\eta`$. For $`c\in\mathcal C_*=\{0,\ldots,2L-1\}^3`$, write $`\widehat{\mathfrak a}_c`$ for its cell copy; thus $`\widehat{\mathfrak a}_c=\widehat a_c`$ in the introduction. In physical coordinates the wall map carrying the first cell to cell $`c`$ acts in coordinate $`\mu`$ by translation through $`2i\ell_c`$ if $`c_\mu=2i`$, and by reflection $`y_\mu\mapsto(2i+2)\ell_c-y_\mu`$ if $`c_\mu=2i+1`$.

For a level-$`j`$ bond function $`A`$, $`\partial A`$ uses forward differences divided by $`\eta_j`$, and

```math
|\delta_\alpha\partial A|_\infty
  =\sup_{\mu,\nu}\sup_{0<d(x,x')\le1}
     \frac{|\partial_\nu A_\mu(x')-\partial_\nu A_\mu(x)|}
          {d(x,x')^\alpha}.
```

We define the uniform probe constants over both possible stop scales. For $`\eta'=L^{-N'}`$ put

```math
g_\nu^{\eta'}[\beta']
      =-\sum_{\mu\ne\nu}\delta_{\eta',\mu}J_{\eta'}\beta'_{\mu\nu}.
```

This is the smooth vector field $`J_{\eta'}a'_{\eta'}`$ in the midpoint formula. Let $`\mathcal I_\beta`$ consist of triples $`(N',a_{\rm s},r')`$ with $`N'\ge0`$, $`a_{\rm s}\in\{h/L,h/L^2\}`$, $`N'+\log_La_{\rm s}\ge1`$, and $`r'\in\{\pm1\}^3`$. $`r'`$ is identified with its diagonal orthogonal matrix, and $`U_{r'}\beta(x)=(\wedge^2r')\beta(r'^{-1}x)`$. At such a triple set $`\eta''=\eta'/a_{\rm s}`$, $`g^0=g^{\eta'}[U_{r'}\beta]`$, and

```math
G_\nu(c)=\sqrt{a_{\rm s}}\,
                  g_\nu^0(a_{\rm s}c+\eta'e_\nu/2)
                       \quad(c\in\eta''\mathbb{Z}^3),\qquad
 W_\nu(x)=\sqrt{\eta'}\,g_\nu^0(\eta'x+\eta'e_\nu/2)
                       \quad(x\in\mathbb{Z}^3).
```

The three norms of $`G`$ are taken at mesh $`\eta''`$. Set

```math
C_\beta=\sup_{\mathcal I_\beta}
              (|G|_\infty+|\partial G|_\infty+
                                    |\delta_\alpha\partial G|_\infty),
 \qquad
 \mathbf D=\sup_{\mathcal I_\beta}\|dW\|_{\ell^2(\text{plaquettes})}^2.
\tag{58}
```

These suprema depend on $`\bar m,L,\alpha,\beta`$, and contain no charge, torus, or placement. They have the finite bounds

```math
C_\beta\le2\sqrt h(1+h+3h^2)|\beta|_{C^3},
 \qquad
 \mathbf D\le48|\beta|_{C^2}^2(D_\beta^{\rm buf}+3)^3 .
\tag{59}
```

**Theorem A (Normalized reference response).**

For the fixed construction, mass $`0<\bar m\le1`$, and probe $`\beta`$ above, there is $`e_{\rm RR}>0`$ such that for every $`0<e\le e_{\rm RR}`$ and every integer $`N\ge N_{\rm ref}(e)`$, the function (2) is entire and

```math
\Theta_4^{(0)}\le C e^{\mathfrak e},\qquad
 (1+|c_2|)\Theta_2^{(0)}\le C e^{\mathfrak e}.
\tag{4}
```

The constants are independent of $`N`$ and of the admitted placement. Every centered placement, $`|v+z_\beta-(\ell_c/2)(1,1,1)|_\infty\le\eta/2`$, is admitted in this range. One may take $`C=3\cdot10^5(1+\sqrt h\,C_\beta)^4h^{1/8}`$, where the finite, charge-independent $`C_\beta`$ is defined in (58).

Let $`\mathbb E^{(0)}`$ denote the normalized zero-flux curvature law on this same reference torus and at the same tuned mass. Equivalently it is the probability law of $`F^{\rm u}=u`$ obtained by weighting $`\gamma_{n_*}`$ with the zero-source twist-averaged determinant in (2). For $`X_c=\langle d\widehat a_c,F^{\rm u}\rangle`$ and $`H_2(y)=y^2-v_\eta`$, $`H_4(y)=y^4-6v_\eta y^2+3v_\eta^2`$,

```math
\mathbb E^{(0)}\prod_{c\in\mathcal C_*}
             (e^{-m}H_m(X_c)-c_m)
       =\left[\prod_{c\in\mathcal C_*}
           (\partial_{t_c}^m-c_m)\right]\mathring\Phi(0),
 \qquad m=2,4.
\tag{5}
```

All expectations are finite. The response estimate concerns the full fixed family of $`N_*=8L^3`$ cells and the harmonic-averaged zero-flux law.

RRM1 also contains **Theorem B in Section 10**, the quantitative terminal reference-error estimate under the factor, mass, one-cell, tree and jet conditions. **Proposition 11.1** admits those conditions on a positive charge interval.


## Navigation

[QEM1 assembly index](../README.md). The published PDFs retain their mathematical text. Links to published outlines use their repository locations; links to withheld manuscripts open the corresponding README. Citations to material outside this assembly remain visible without a download link.
