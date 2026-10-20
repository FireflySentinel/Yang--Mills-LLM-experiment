# Terminal measure and pressure (TP1)

**Disclaimer:** these documents are largely LLM-created. Their correctness has not been satisfactorily verified.

Project codename: **TP1**.

- **TPO1** — [The terminal measure and pressure estimates](TPO1.pdf).
- **AI-written manuscript:** **TPM1** — *The terminal measure and pressure estimates for lattice QED in three dimensions* (manuscript to be added).
- **Human-written manuscript:** to be added.

## Role in the QEM1 assembly

Terminal measure, pressure and two-torus comparison.

QEO1 contracts: [T08](../QEO1.pdf#page=113), [T09](../QEO1.pdf#page=32), [T10](../QEO1.pdf#page=115), [T11](../QEO1.pdf#page=34).

Only early RRM1 source identities are imported here; later RRM1 response uses TPM1.

Related inputs: [CVM1](../Cover%20agreement%20and%20common%20tuning%20%28CV1%29/README.md), [RRM1](../Reference%20response%20%28RR1%29/README.md). Read their hypotheses at the cited results.

## Principal statements

Notation and numbered references below follow **TPM1**. The imported construction and estimates are part of the hypotheses.

### Setting

We use the chamber regulator with weights $`(6,6\sqrt2,6\sqrt2,6)`$ and Wilson parameter $`0<\rho<1`$. On the unit cubic torus $`C_n`$ with $`n`$ sites per side, let $`\mathcal F_n=dC^1(C_n;\mathbb{R})`$ be the space of exact real two-cochains, with counting inner product and standard Gaussian measure $`\gamma_n`$. Write $`A(u)`$ for the mean-zero coclosed potential of $`u\in\mathcal F_n`$. For $`q>0`$ and a real lattice mass $`\boldsymbol\mu`$, define the matter factor

```math
z_{r,n}(q,\boldsymbol\mu)=
 \int_{[-\pi,\pi]^3}\frac{\mathrm{d}\theta}{(2\pi)^3}
 \int_{\mathcal F_n}
 \det\bigl(D^{\rm ch}[q(A(u)+H_\theta)]+\boldsymbol\mu\bigr)
 \,\mathrm{d}\gamma_n(u),\qquad
 H_{\theta,\nu}=\frac{\theta_\nu}{qn}.
\tag{1}
```

Here $`D^{\rm ch}[qB]`$ is the unit-mesh, four-spin-component chamber Dirac operator of (**LPM1**, Section 2), with $`48`$ chamber labels per site and antiperiodic spinors. Its argument $`qB`$ is the bond phase; the subscript $`r`$ in $`z_{r,n}`$ denotes the regulator. The harmonic average in (1) is the zero-flux matter factor of (**RRM1**, (37)–(40)).

Fix once and for all a choice of the block construction constants satisfying (**QEM1**, Proposition 4.1), through its charge ceilings $`e_1\le e_0<1`$ and terminal scalar conditions. Thus $`L`$ is odd, $`M`$ is a power of $`L`$, $`M\ge L^2`$, $`0<\varepsilon\le1/200`$, and the exponents are $`r=2`$, $`p_0=9`$, $`p=19`$. The fixed ceilings denoted by $`e_0,e_1`$ here are the $`\bar e_0,\bar e_1`$ of (**QEM1**); they are distinct from the running charge $`e_j`$ at $`j=0`$. This choice includes the photon and fermion primitive bounds, the exact normalized block step, and its field domains. For $`0<\bar m\le1`$ and $`N\in\mathbb{Z}_{\ge0}`$ put

```math
h=L^{\lfloor\log_L\bar m^{-1}\rfloor},\qquad
 \eta=L^{-N},\qquad K=N+\log_Lh,\qquad
 a_j=L^{j-N},\quad e_j=e\sqrt{a_j},\quad \mu_j=\bar m a_j.
```

We distinguish the initial charge $`q=e\sqrt\eta`$ from the fixed ceiling $`e_0`$. Set $`v_j=-\log e_j`$, $`p_j=v_j^{19}`$, $`p_{0,j}=v_j^9`$, and let $`r_j`$ be the least nonnegative integer power of $`L`$ which is at least $`v_j^2`$. Define

```math
R_{\rm top}=hMr_K,\qquad R_*=R_{\rm top}/L,\qquad
 \mathcal T(e)=\{hL^t:t\in\mathbb{Z}_{\ge0},\ hL^t\le R_{\rm top}\}.
```

For $`R\in\mathcal T(e)`$, the threshold $`N_{\min}(R,e)`$ and first stopping level $`k_*(R)\ge1`$ are those of (**CVM1**, Proposition 6.1 and (52)): the stop is the first level with $`\ell_j=Mr_j`$, where $`\ell_j=R/a_j`$. At cutoffs $`N\ge N_{\min}(R,e)`$, write $`a_*=a_{k_*}`$, $`e_*=e_{k_*}`$, $`\mu_*=\mu_{k_*}`$ and $`\ell_*=\ell_{k_*}`$. These physical quantities are independent of $`N`$, and

```math
Mv_*^2\le\ell_*<LMv_*^2,\qquad
 \mu_*^{-1}<L\ell_*,\qquad 0<e_*\le e_K=e\sqrt h,\qquad
 0<\mu_*\le1.
\tag{2}
```

The threshold is finite and nonincreasing in $`R`$. The numerical consequences of the fixed scheme used below are listed and verified in Section 5.

Use the real pair $`P_N(e)=(m_{0,N}(e),\varepsilon_{0,N}^{\rm v}(e))`$ of (**CVM1**, Theorem D): it is selected on $`R_{\rm top}`$ with zero initial activity and zero terminal mass shift and vacuum term there. The same pair gives a controlled trajectory on every $`R\in\mathcal T(e)`$ above its stated threshold. In particular, $`|m_{0,N}(e)|\le\frac18 q^{3/4-8\varepsilon}`$. Set $`\boldsymbol\mu_N=\bar m\eta+m_{0,N}(e)`$ and abbreviate $`z_{r,n}=z_{r,n}(q,\boldsymbol\mu_N)`$, $`n=R/\eta`$. The total mass $`\boldsymbol\mu_N`$ may have either sign. Its free comparison uses the positive reference mass:

```math
z_{r,n}^{\rm free}
   =\int_{[-\pi,\pi]^3}
        \det(D^{\rm ch}[qH_\theta]+\bar m\eta)
                      \frac{\mathrm{d}\theta}{(2\pi)^3}.
```

Let $`\mathcal D_m(p)`$ denote the $`192\times192`$ chamber Fourier symbol at mass $`m>0`$, and set

```math
p_{\rm ch}^0(m)=\int_{[-\pi,\pi]^3}
                   \log\det\mathcal D_m(p)\frac{\mathrm{d} p}{(2\pi)^3},
 \qquad
 p_F=p_{\rm ch}^0(\bar m\eta)+\varepsilon_{0,N}^{\rm v}(e).
\tag{3}
```

The positive constants $`C_6,\kappa_{(0)}`$, depending only on $`\rho`$ and the fixed weights, are given in Proposition 4.1. Write $`\varepsilon_5(x)=C_6\log(1-e^{-\kappa_{(0)}x})^{-1}`$ and $`N_{\rm ref}(e)=N_{\min}(R_*,e)`$.

**Theorem A (Common pressure and the two-torus comparison).**

Fix the construction and the common pair specified above, and assume $`0<e\sqrt h\le e_1`$. For every $`R\in\mathcal T(e)`$ and $`N\ge N_{\min}(R,e)`$, the matter factors $`z_{r,n}`$ and $`z_{r,n}^{\rm free}`$ are positive, and

```math
\begin{aligned}
\left|\log z_{r,n}-\log z_{r,n}^{\rm free}
                      -\varepsilon_{0,N}^{\rm v}(e)n^3\right|
          &\le3e_*^{1/4-9\varepsilon},\\[0pt]
 \left|\log z_{r,n}-p_Fn^3\right|
          &\le\varepsilon_P(R)
             :=\varepsilon_5(\bar mR)+3e_*^{1/4-9\varepsilon}
          \le\varepsilon_5(1/L)+3e_K^{1/4-9\varepsilon}.
\end{aligned}
\tag{4}
```

In particular let $`R_*=R_{\mathrm{top}}/L`$, $`n_*=R_*/\eta`$, and $`N\ge N_{\rm ref}(e)`$. The two tori $`R_*`$ and $`LR_*`$ use the same mass and the same pressure. Their matter comparison satisfies

```math
\begin{aligned}
|D_{\rm mat}|
 &:=\left|L^3\log z_{r,n_*}-\log z_{r,Ln_*}\right|
       \le L^3\varepsilon_P(R_*)+\varepsilon_P(LR_*)
       \\[0pt]
 &\le (L^3+1)
          \left[\varepsilon_5(\bar mR_*)
                                      +3e_K^{1/4-9\varepsilon}\right]
       \le C_{\rm mat},\\[0pt]
 C_{\rm mat}&=(L^3+1)\bigl(\varepsilon_5(1/L)+1\bigr).
\end{aligned}
\tag{5}
```

The same $`p_F=p_F(N,e,\bar m)`$ is used for every asserted side. The displayed error bounds are uniform in $`N`$; $`C_{\rm mat}`$ depends only on $`L,\rho`$ and the fixed chamber weights.

### Free pressure and harmonic twists

The partition comparison requires an error in the free pressure which depends on the physical size, rather than on the number of lattice sites. It also requires a twist estimate for the operator with a block penalty. The latter penalty removes the small-mass singularity before the fine mesh is taken to zero.

For $`0<m\le1`$ let $`\mathfrak d_m(p)=\det\mathcal D_m(p)`$, where $`\mathcal D_m`$ is the $`192`$-dimensional chamber symbol in (**FBM1**, Section 2.2), and set

```math
p_{\rm ch}^0(m)=
       \int_{[-\pi,\pi]^3}\log\mathfrak d_m(p)
                                      \frac{\mathrm{d} p}{(2\pi)^3}.
\tag{25}
```

The spin-block identity and positive real part imply $`\mathfrak d_m(p)>0`$ for real $`p`$. In this subsection $`|z|=|z|_\infty`$ for $`z\in\mathbb{Z}^3`$. Write $`\kappa_{(0)}=\kappa_{\mathrm{strip}}`$ from (**FBM1**, Proposition 2.2).

**Proposition 4.1.**

There is a finite $`C_6`$, depending only on $`\rho`$, such that, with

```math
\varepsilon_5(x)=
 C_6\log\frac1{1-e^{-\kappa_{(0)}x}}\qquad(x>0),
\tag{26}
```

the free twisted determinant on a unit torus of side $`n\ge1`$ satisfies

```math
\left|\log\det(D^{\rm ch}[qH_\theta]+m)
                     -n^3p_{\rm ch}^0(m)\right|
                                 \le\varepsilon_5(mn).
\tag{27}
```

Here $`H_{\theta,\mu}=\theta_\mu/(qn)`$ and $`\theta\in\mathbb{R}^3`$. For $`m=\bar m\eta`$ and $`n=R/\eta`$ define

```math
z_{r,n}^{\rm free}
       =\int_{[-\pi,\pi]^3}
            \det(D^{\rm ch}[qH_\theta]+\bar m\eta)
                                         \frac{\mathrm{d}\theta}{(2\pi)^3}.
```

Then $`z_{r,n}^{\rm free}>0`$ and

```math
\left|\log z_{r,n}^{\rm free}
                 -n^3p_{\rm ch}^0(\bar m\eta)\right|
                              \le\varepsilon_5(\bar mR).
\tag{28}
```

TPM1 also contains **Theorem B in Section 3.2**, the exact terminal-density identity for bounded Borel observables, under the photon-coordinate, box, domain and external-connection conventions of Section 3.


## Navigation

[QEM1 assembly index](../README.md). The published PDFs retain their mathematical text. Links to published outlines use their repository locations; links to withheld manuscripts open the corresponding README. Citations to material outside this assembly remain visible without a download link.
