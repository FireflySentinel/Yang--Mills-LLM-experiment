# Volume transfer (VT1)

**Disclaimer:** these documents are largely LLM-created. Their correctness has not been satisfactorily verified.

Project codename: **VT1**.

- **VTO1** — [Volume transfer and non-Gaussian continuum components](VTO1.pdf).
- **VTM1** — *Volume transfer and component cumulants for lattice QED in three dimensions* (manuscript to be added).

## Role in the QEM1 assembly

All-volume products, prescribed-parent finite-periodic moments and component cumulants.

QEO1 contracts: [T17](../QEO1.pdf#page=37), [T18](../QEO1.pdf#page=122), [B5](../QEO1.pdf#page=39), [A3](../QEO1.pdf#page=43).

Retain the same selected mass/parent, component Gaussian hypothesis and numerical inputs.

Related inputs: [TPM1](../Terminal%20measure%20and%20pressure%20%28TP1%29/README.md), [RRM1](../Reference%20response%20%28RR1%29/README.md), [PRM1](../Positive%20probes%20and%20free%20response%20%28PR1%29/README.md), [LPM1](../Infinite-lattice%20reflection%20positivity%20%28LP1%29/README.md), [CEM1](../Continuum%20existence%20%28CE1%29/README.md), [ECM1](../Continuum%20components%20and%20clustering%20%28EC1%29/README.md). Read their hypotheses at the cited results.

## Principal statement

Notation and numbered references below follow **VTM1**. The imported construction and estimates are part of the hypotheses.

### Setting

Let $`\mathbb P_{n;q,\boldsymbol\mu}^{\rm af}`$ be the all-flux chamber QED law on $`C(n)=\mathbb{Z}^3/n\mathbb{Z}^3`$, with charge $`q>0`$, real lattice mass $`\boldsymbol\mu`$, Wilson parameter $`0<\rho<1`$, weights $`(6,6\sqrt2,6\sqrt2,6)`$ and antiperiodic fermions. Its real curvature is $`F^{\rm u}=dA+(2\pi/q)z`$, where $`z`$ is a closed integer two-cochain. Write $`Z_n`$ for its unnormalized partition function and $`F^\sharp`$ for the physical step field: on the cube of side $`\eta`$ centered at a plaquette, its corresponding component is $`\eta^{-3/2}F^{\rm u}`$. The measure and its normalization are recalled in Section 2.

Fix an odd integer $`L\ge13`$, $`M=L^k`$ with integer $`k\ge2`$, $`0<\varepsilon\le1/200`$ and $`0<\bar m\le1`$. Set

```math
h=L^{\lfloor\log_L(1/\bar m)\rfloor},\qquad
 \eta=L^{-N},\quad q=e\sqrt\eta,\qquad R=8hL^T,\quad n=R/\eta.
\tag{1}
```

At each $`e,N`$ let $`\boldsymbol\mu_N`$ be real and independent of the outer volume $`T`$. Every reference and outer law below uses this same mass. The cutoffs $`N,T`$ are nonnegative integers. For $`e\sqrt h<1`$, put

```math
v_K=-\log(e\sqrt h),\qquad
 r_K=\min\{L^i:i\in\mathbb{Z}_{\ge0},\ L^i\ge v_K^2\},
 \qquad R^*=\frac{hMr_K}{L}=hL^{T^*}.
```

The reference torus has side $`n_*=R^*/\eta`$ and $`N_*=8L^3`$ cells, each of physical width $`\ell_c=R^*/(2L)`$.

Fix real nonzero $`\beta\in C_c^\infty(\mathbb{R}^3;\Lambda^2)`$ and $`f=dd^*\beta`$. Let $`D_\beta`$ be the side of a least coordinate cube containing $`\mathrm{supp}\beta`$ and let $`Q_\beta`$, of side $`D_\beta^{\rm buf}=D_\beta+4`$ and center $`z_\beta`$, be that cube enlarged by two in each direction. Denote cube averaging by $`J_\eta`$ and centered differences by

```math
\delta_{\eta,\mu}g=
 \frac{g(\,\cdot+\eta e_\mu/2)-g(\,\cdot-\eta e_\mu/2)}{\eta}.
```

Define

```math
a'_{\eta,\nu}=-\sum_{\mu\ne\nu}\delta_{\eta,\mu}\beta_{\mu\nu},
 \qquad
 f^\eta_{\mu\nu}=\delta_{\eta,\mu}a'_{\eta,\nu}
                     -\delta_{\eta,\nu}a'_{\eta,\mu}.
\tag{2}
```

The covering bond source is $`\widehat a^o_\nu(x)=\eta^{1/2}(J_\eta a'_{\eta,\nu})(\eta x+\eta e_\nu/2)`$. Put $`v_\eta=\|d\widehat a^o\|_{\ell^2}^2`$. A centered placement $`v\in\eta\mathbb{Z}^3`$ satisfies $`|v+z_\beta-(\ell_c/2)(1,1,1)|_\infty\le\eta/2`$. Translate the probe by $`v`$, reflect its source into the $`N_*`$ cells, and periodize to obtain $`\widehat a_c`$. The reflected copies use the two-form orientation signs.

Let $`D^{\rm ch}[B]`$ be the chamber Dirac operator with bond phase $`B`$. Define the free one-cell ratio and its ordinary derivatives by

```math
N_0(t)=\frac{\det(D^{\rm ch}[q(t/e)\widehat a_0]+\bar m\eta)}
                    {\det(D^{\rm ch}[0]+\bar m\eta)},\qquad
 c_m=N_0^{(m)}(0),\quad m=2,4.
\tag{3}
```

The free mass is positive even when $`\boldsymbol\mu_N`$ is signed. Write $`\mathbb E^{(0)}_{n_*}`$ for the same-mass reference law conditioned on zero flux, and set

```math
H_2(x;v)=x^2-v,\qquad H_4(x;v)=x^4-6vx^2+3v^2,\qquad
 W_m(x;v,c)=e^{-m}H_m(x;v)-c.
\tag{4}
```

Here and below $`e`$ is the charge, so $`e^{-m}`$ is its inverse power. With $`X_c=\langle d\widehat a_c,F^{\rm u}\rangle`$, put

```math
\Theta_m^{(0)}
 =\left|\mathbb E_{n_*}^{(0)}
       \prod_{c\in\{0,\ldots,2L-1\}^3}W_m(X_c;v_\eta,c_m)
   \right|^{1/N_*}.
\tag{5}
```

Let $`z_{r,n}`$ be the positive zero-flux matter factor in (16). At continuum mass $`\bar m`$ define

```math
b(f)=-6\mathrm{tr}\left[
    \bigl((\bar m+\gamma\cdot\partial)^{-1}i\gamma\cdot d^*\beta
                 \bigr)^4\right],
```

where $`\gamma_\nu=\mathrm{diag}(\sigma_\nu,-\sigma_\nu)`$. The displayed fourth power is trace class and its trace is real by (**PRM1**, Theorem A).

### Finite-law and reference-cell conventions

The chamber operator is the finite-range operator of (**LPM1**, Section 2); its bond argument is a phase. It acts on four spin components and $`48`$ chamber labels per site. The fermions are antiperiodic in each coordinate. For a rectangular coordinate torus with $`V`$ sites and every side at least four, put $`r_q=2\pi/q`$. The unnormalized integral of a curvature observable $`O`$ is

```math
Z[O]=\sum_{\substack{z\in C^2(\mathbb{Z})\\dz=0}}
  \int_{[0,r_q)^{3V}}
 O(dA+r_qz)\exp\bigl(-\tfrac12\|dA+r_qz\|^2\bigr)
 \det(D^{\rm ch}[qA]+\boldsymbol\mu)\,\mathrm{d} A.
\tag{14}
```

Cochains and the integer sum are on this torus; norms and pairings count positively oriented cells. The identification $`(A,z)\sim(A+r_qk,z-dk)`$ makes the integral independent of the chosen fundamental domain. The law is $`Z[O]/Z[1]`$. The partition function is finite and positive for every real $`\boldsymbol\mu`$, and the determinant gives nonnegative weights; see (**LPM1**, Section 2–3). Flux is the three integer periods of $`z`$, ordered as $`(23,13,12)`$. We retain every flux sector in (14).

The coordinate-torus Gaussian bound (**LPM1**, Proposition 5.1) is

```math
\mathbb{E}^{\rm af}\exp\langle g,F^{\rm u}\rangle
       \le\exp(\|g\|^2/2)
\tag{15}
```

for every real torus two-cochain $`g`$. It holds for both odd and even coordinate sides. The law is invariant under lattice translations and $`F^{\rm u}\mapsto-F^{\rm u}`$. In particular all odd moments of a real linear observable vanish.

On $`C(n)`$, let $`\gamma_n`$ be the standard Gaussian measure on the exact real two-cochains, and let $`A(u)`$ be the mean-zero coclosed potential of $`u`$. For $`\theta\in[-\pi,\pi]^3`$ put $`H_{\theta,\nu}=\theta_\nu/(qn)`$. The matter factor is

```math
z_{r,n}=\int_{[-\pi,\pi]^3}\frac{\mathrm{d}\theta}{(2\pi)^3}
     \int\det(D^{\rm ch}[q(A(u)+H_\theta)]
                     +\boldsymbol\mu)\,\mathrm{d}\gamma_n(u)>0.
\tag{16}
```

The subscript $`r`$ denotes the regulator. The exact zero-flux factorization of (**RRM1**, Section 3.4) gives

```math
Z_n^{(0)}[1]=Z_n^{\rm ph}z_{r,n},
\tag{17}
```

```math
Z_n^{\rm ph}=r_q^{\,n^3+2}(2\pi)^{n^3-1}
                         \exp(-\mathcal L(n)/2).
\tag{18}
```

where $`\mathcal L(n)`$ is the scalar-Laplacian logarithmic determinant in Section 4. Thus the normalized zero-flux curvature law is the Gaussian law weighted by the twist-averaged determinant in (16). The factorization retains the gauge and harmonic volume factors; they will contribute to the partition defect.

Write $`p_{\rm cell}=n_*/L`$ and $`w=p_{\rm cell}/2`$. The reference side $`n_*`$ and $`p_{\rm cell}`$ are odd, so $`w`$ is half-integral. The number $`2L`$ of cells per side is even. In unit-lattice coordinates the open cells are $`Q_c^\circ=w(c+(0,1)^3)`$.

For a two-form $`g`$ let

```math
g_{[\eta]}(\sigma)=\eta^{-3/2}
        \int_{Q_\eta(\sigma)}g_{\mu\nu}(y)\,\mathrm{d} y,\qquad
 Q_\eta(\sigma)=\eta\bigl(x+(e_\mu+e_\nu)/2+[-1/2,1/2)^3\bigr),
```

when $`\sigma=(x;\mu\nu)`$. The source of the introduction obeys $`d\widehat a^o=(f^\eta)_{[\eta]}`$. After periodizing, this gives

```math
\langle d\widehat a,F^{\rm u}\rangle=F^\sharp(f^\eta).
```

All $`f^\eta`$ are supported in $`Q_\beta`$ for $`\eta\le1`$, and

```math
\|f^\eta-f\|_{H^s}\le\eta^2\|\beta\|_{H^{s+4}}
                       \quad(s\in\mathbb{R}).
\tag{19}
```

The variance converges with the quantitative estimate

```math
\left|\sqrt{v_\eta}-\|f\|_2\right|
 \le21\eta|\beta|_{C^3}(D_\beta^{\rm buf})^{3/2}
                       +\eta^2\|\beta\|_{H^4}.
\tag{20}
```

Here $`|\beta|_{C^3}`$ is the maximum component derivative norm through order three. These estimates follow from the centered difference symbols and the cell-average approximation.

For the placed probe, the coordinate map $`g_c`$ carrying the base cell to cell $`c`$ is, in coordinate $`\mu`$, $`x_\mu\mapsto x_\mu+2iw`$ if $`c_\mu=2i`$, and $`x_\mu\mapsto(2i+2)w-x_\mu`$ if $`c_\mu=2i+1`$. Transport oriented cochains by this map before periodizing. Denote the placed and reflected covering source by $`\widehat a_c^o`$; its periodization is $`\widehat a_c`$. On every carrying torus with $`p_{\rm cell}\mid n`$ and $`n\ge n_*`$,

```math
\langle d\widehat a_c,d\widehat a_{c'}\rangle_n
                         =v_\eta\mathbf1_{\{c=c'\}}.
\tag{21}
```

The placement condition (6) ensures that their support boxes are strictly inside the open cells and that the boxes enlarged by one embed in the torus. Each polynomial $`P(X_c)`$ is consequently read by the same local scalar integrand on every such torus.

### Limit topology

Let $`\mathsf A=1+|y|^2-\Delta`$ on $`\mathbb{R}^3`$, with real $`L^2`$-orthonormal Hermite two-forms $`h_\kappa`$ and eigenvalues $`\lambda_\kappa`$. Each scalar Hermite function occurs once for each of the three components. We use the Hilbert space

```math
H_{-4}=\left\{F:\sum_\kappa\lambda_\kappa^{-8}
                                  |F(h_\kappa)|^2<\infty\right\}.
```

It is continuously embedded in tempered two-form distributions, and each Schwartz evaluation is continuous there. The step-field realization, tightness and fixed-spacing limits in this space are proved in (**CEM1**).

**Theorem A (Volume transfer and component cumulants).**

Fix the data above and a charge interval $`0<e\le e_*\le1/3`$. For each charge let $`N_{\rm ref}(e)`$ be a finite nonnegative integer. Assume the following conditions for every charge in this interval and every $`N\ge N_{\rm ref}(e)`$.

**(i)** The scale and placement conditions are

```math
v_K\ge8,\qquad e\sqrt h\log h\le1,\qquad
 6N_*Mv_K^2\exp(-v_K)
          \bigl(v_K\exp(-v_K)+\tfrac12\bigr)\le\pi^2,
```

and

```math
D_\beta^{\rm buf}+3\eta\le\ell_c,\qquad
 v+Q_\beta\subset[\ell_c/8,7\ell_c/8]^3
\tag{6}
```

for each centered placement used.

**(ii)** There are finite nonnegative constants $`C_{\rm mat}`$ and $`C_{\rm ref}`$, independent of charge, mesh and placement, such that, at the same $`q,\boldsymbol\mu_N`$ on the two reference tori,

```math
\begin{aligned}
L^3\log z_{r,n_*}-\log z_{r,Ln_*}&\le C_{\rm mat},\\[0pt]
 \Theta_4^{(0)}&\le C_{\rm ref}e^{\mathfrak e},\qquad
 (1+|c_2|)\Theta_2^{(0)}\le C_{\rm ref}e^{\mathfrak e},
 \\[0pt]
 |c_2|+|c_4|^{1/2}&\le C_{\rm ref},\qquad
 |c_4-3c_2^2-b(f)|\le C_{\rm ref}(e+\eta^{1/4}),
\end{aligned}
\tag{7}
```

where

```math
\mathfrak e=\tfrac12(1/4-9\varepsilon)-12\varepsilon,\qquad
 a_L=\frac{L^3-1}{(L-1)^3},\qquad
 \sigma=\mathfrak e-\frac{2a_L}{N_*}>0.
```

There is $`C_U<\infty`$, depending only on these fixed data and constants, such that the following assertions hold uniformly in the stated charge interval.

For each $`N\ge N_{\rm ref}(e)`$ there are $`u_2,u_4\ge0`$, independent of the outer cutoff $`T`$, with

```math
u_4\le C_Ue^\sigma,\qquad
 (1+|c_2|)u_2\le C_Ue^\sigma,\qquad
 |c_4-3c_2^2-b(f)|\le C_U(e^\sigma+\eta^{1/4}).
\tag{8}
```

For every $`T\ge T^*(e)+1`$ and every finite $`Y\subset(R^*/L)\mathbb{Z}^3`$ whose points are incongruent modulo $`R\mathbb{Z}^3`$,

```math
\left|\mathbb{E}_{N,T}\prod_{y\in Y}
 W_m(F^\sharp(\tau_yf^\eta);v_\eta,c_m)\right|
              \le u_m^{|Y|},\qquad m=2,4.
\tag{9}
```

Here $`\tau_yf(x)=f(x-y)`$ and $`\mathbb{E}_{N,T}`$ is expectation under $`\mathbb P_{n;q,\boldsymbol\mu_N}^{\rm af}`$. Its smooth-test fourth cumulant satisfies

```math
|\kappa_4(F^\sharp(f))-e^4b(f)|
 \le(8C_U+3C_U^2)e^{4+\sigma}
                  +C_U(\eta^2+e^4\eta^{1/4}).
\tag{10}
```

Fix one charge. Let $`\mu`$ be any prescribed volume-first limit: for $`N_i\to\infty`$, choose fixed-spacing weak volume limits $`\mu_i`$ of these laws, with $`\mu_i\Rightarrow\mu`$. All weak convergence here is on the negative Hermite space $`H_{-4}`$ specified in Section 7. Assume that $`\mu`$ is translation invariant and that almost every component in its translation-ergodic decomposition $`\mu=\int\mu_\xi\,\mathrm{d}\nu(\xi)`$ satisfies

```math
\mathbb{E}_{\mu_\xi}\exp(F(g))\le\exp(\|g\|_2^2/2)
 \quad\text{for all real }g\in\mathcal S(\mathbb{R}^3;\Lambda^2).
\tag{11}
```

Then, on one $`\nu`$-full set,

```math
|\kappa_4^{\mu_\xi}(f)-e^4b(f)|
                    \le C_fe^{4+\sigma},\qquad C_f=8C_U+3C_U^2.
\tag{12}
```

If $`b(f)>0`$ and $`C_fe^\sigma\le b(f)/2`$, every component in this set has $`\kappa_4^{\mu_\xi}(f)\ge e^4b(f)/2>0`$. The full-measure set is for this fixed charge, probe and parent law.


## Navigation

[QEM1 assembly index](../README.md). The published PDFs retain their mathematical text. Links to published outlines use their repository locations; links to withheld manuscripts open the corresponding README. Citations to material outside this assembly remain visible without a download link.
