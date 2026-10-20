# Chamber fermion block analysis (FB1)

**Disclaimer:** these documents are largely LLM-created. Their correctness has not been satisfactorily verified.

Project codename: **FB1**.

- **FBO1** — [Chamber fermion locality and local integration](FBO1.pdf).
- **AI-written manuscript:** **FBM1** — *Chamber fermion locality and local integration* (manuscript to be added).
- **Human-written manuscript:** to be added.

## Role in the QEM1 assembly

Chamber inverses, locality, determinant gains and local integration.

QEO1 contracts: [S01](../QEO1.pdf#page=77), [S02](../QEO1.pdf#page=79), [S05](../QEO1.pdf#page=85), [S06](../QEO1.pdf#page=87), [S07](../QEO1.pdf#page=89), [S08](../QEO1.pdf#page=90).

Related inputs: [MBM1](../Maxwell%20block%20analysis%20%28MB1%29/README.md). Read their hypotheses at the cited results.

## Main statements

The setting and principal theorem below are reproduced from **FBM1**. Notation and numbered references follow that manuscript; references to other documents use their codenames.

Fix $`0<\rho<1`$, an odd integer $`L\ge5`$, $`0<\alpha<1`$, and
$`\varepsilon>0`$. At level $`k\ge0`$, put $`\eta=\eta_k=L^{-k}`$.
A photon site is $`c\in\eta\mathbb{Z}^3/\ell\mathbb{Z}^3`$; a chamber site is
$`x=(c,g)`$, where $`g\in O_{\mathrm{cub}}`$ is a signed permutation
matrix. There are $`48`$ labels $`g`$ and four spin components at
each photon site. Connections are periodic complex oriented bond
functions, with $`A(c',c)=-A(c,c')`$; spinors are antiperiodic in
each coordinate. The chamber measure is $`\eta^3/48`$, while the
photon-site spinor measure is $`\eta^3`$.
Operator kernels use the chamber measure in their column variable;
the identity kernel is $`48\eta^{-3}\mathbf1[x=x']1_4`$.
The cluster injection and mean are

```math
(J\xi)(c,g)=\xi(c),\qquad J^*f(c)=48^{-1}\sum_g f(c,g).
```

Adjoints use these Hermitian pairings. Transposes use the corresponding
bilinear pairings, without complex conjugation.

Use the Pauli and Dirac matrices

```math
\sigma_1=\begin{pmatrix}0&1\\1&0\end{pmatrix},\quad
 \sigma_2=\begin{pmatrix}0&-i\\i&0\end{pmatrix},\quad
 \sigma_3=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad
 \gamma_j=\sigma_3\otimes\sigma_j,\quad
 \gamma_5=\sigma_1\otimes1_2.
```

Let $`s_0`$ reverse the third coordinate, $`s_1`$ interchange
coordinates $`2,3`$, and $`s_2`$ interchange $`1,2`$; let $`r_{e_1}`$
reverse the first coordinate. The four neighbours, inward normals,
and weights are

```math
\begin{gathered}
 x^{(i)}=(c,gs_i)\quad(0\le i\le2),\qquad
 x^{(3)}=(c+\eta ge_1,gr_{e_1}),\\[0pt]
 (n_0,n_1,n_2,n_3)
   =(e_3,(e_2-e_3)/\sqrt2,(e_1-e_2)/\sqrt2,-e_1),\\[0pt]
 (w_0,w_1,w_2,w_3)=(6,6\sqrt2,6\sqrt2,6).
 \end{gathered}
```

For a charge $`e_k>0`$, the chamber operator is

```math
(D_Af)(x)=-\eta^{-1}\sum_{i=0}^3
       \frac{w_i}{2}(\rho+\gamma\cdot gn_i)
       \bigl(U_A(x,x^{(i)})f(x^{(i)})-f(x)\bigr),
```

where internal transports are one and the external transport is
$`\exp(ie_k\eta A(c,c+\eta ge_1))`$.

The unit blocks are
$`\Delta_z=\{c:|c-z|_\infty<1/2\}`$, $`z\in\mathbb{Z}^3/\ell\mathbb{Z}^3`$.
For $`c\in\Delta_z`$, let $`c=c_0,c_1,\ldots,c_k=z`$ be the
centres of its nested blocks of sides $`L^j\eta`$.
Write $`\tau A(u,v)`$ for the arithmetic mean of the oriented
fine-bond sums along the six coordinate-order paths from $`u`$ to $`v`$.
Set

```math
\begin{aligned}
 \varphi_A(z,c)&=\exp\!\left(ie_k\eta
                    \sum_{j<k}\tau A(c_{j+1},c_j)\right),&
 (Q_k(A)\xi)(z)&=\eta^3\sum_{c\in\Delta_z}\varphi_A(z,c)\xi(c),\\[0pt]
 (Q_k^T(-A)v)(c)&=\varphi_A(z,c)^{-1}v(z).&&
 \end{aligned}
```

For $`z'\in L\mathbb{Z}^3/\ell\mathbb{Z}^3`$, put $`B(z')=\{z:|z-z'|_\infty<L/2\}`$.
The next average and its algebraic reverse are

```math
\begin{aligned}
 U_A(z',z)&=\exp(ie_k\eta\tau A(z',z)),\\[0pt]
 (Q(A)v)(z')&=L^{-3}\sum_{z\in B(z')}U_A(z',z)v(z),&
 (Q^T(-A)v')(z)&=U_A(z',z)^{-1}v'(z').
 \end{aligned}
```

The target pairing has measure $`L^3`$. These maps act componentwise
in spin. For $`k\ge1`$, define

```math
\Pi_1(A)=JQ_k^T(-A)Q_k(A)J^*,\qquad
 \Pi_L(A)=JQ_k^T(-A)Q^T(-A)Q(A)Q_k(A)J^*.
```

At $`k=0`$ use only $`\Pi_L(A)=JQ^T(-A)Q(A)J^*`$.
Let $`b=1`$, $`b_L=L^{-1}`$, $`b_-=1-L^{-1}`$, and

```math
b_k=\frac{1-L^{-1}}{1-L^{-k}}\quad(k\ge1),\qquad
 \alpha_y=\frac{b_ki\gamma_5y}{b_k+i\gamma_5y},\qquad
 \beta_y=\frac{b_k^2b_L}{(b_k+b_L+i\gamma_5y)(b_k+i\gamma_5y)}.
```

At $`y=\infty`$, put $`\alpha_\infty=b_k`$, $`\beta_\infty=0`$.
For $`0<\mu\le1`$, the penalized operators are

```math
F_y(A)=
 \begin{cases}
 D_A+\mu+\alpha_y\Pi_1(A)+\beta_y\Pi_L(A),
      & k\ge1,\ y\in\mathbb{R}\cup\{\infty\},\\[0pt]
 D_A+\mu+b_L\Pi_L(A)+i\gamma_5y,
      & k=0,\ y\in\mathbb{R}.
 \end{cases}
```

The data $`k,\mu,\ell,e_k`$ are independent.

Let $`M\ge L^2`$ be a power of $`L`$, with partition $`M`$-cubes
centred in $`M\mathbb{Z}^3/\ell\mathbb{Z}^3`$, and assume $`\ell/(LM)`$ is odd
and at least $`13`$. A connection belongs to
$`\widetilde{\mathcal G}_k`$ if $`A=A_0+A_1`$, $`A_0`$ is real,
$`\|A_1\|_\infty<e_k^{-1+\varepsilon}`$, and on every concentric
$`11M`$ enlargement of a partition cube,

```math
A_0=B_0+d\lambda,\qquad B_0,\lambda\ \hbox{real},\qquad
 \|B_0\|_\infty<e_k^{-1+\varepsilon},\qquad
 d\lambda(c,c')=\eta^{-1}(\lambda(c')-\lambda(c)).
```

The local gauges may be chosen independently.

Distances are periodic sup distances. For distinct chamber sites set
$`d_X(x,x')=\max(d(c,c'),\eta)`$, and, on pairs with $`0<d_X<1`$, put

```math
U_A(x,x')=\exp(ie_k\eta\tau A(c,c')),\qquad
 (\delta_{\alpha,A}v)(x,x')
 =\frac{U_A(x,x')v(x')-v(x)}
        {d_X(x,x')^\alpha}.
```

Thus distinct labels over one photon site are included when $`k\ge1`$.
For an operator $`T`$, define

```math
N_\gamma(T)=\sup_z\sum_{z'}e^{\gamma d(z,z')}
       \|\mathbf1_{\Delta_z}T\mathbf1_{\Delta_{z'}}\|_{\infty\to\infty}.
```

The sup norm uses Euclidean spinor norms; for pair outputs the left
indicator restricts the first point. At level zero,
$`N_\gamma^{\mathrm{ker}}`$ replaces the localized operator norm by
the supremum of the normalized chamber kernel on the two clusters.

**Theorem A.**

There are $`a'>0`$ and $`0<\gamma\le(6L)^{-1}`$, depending only on
$`\rho,L,\alpha`$, with the following property. Set
$`C_V=2\exp(1)(42+6b)`$ and
$`q(p)=54\pi C_Va'p/M`$. Assume

```math
M>4L,\qquad q(1)\le\tfrac12,\qquad
 0<e_k\le e_0,\qquad
 6Le_0^\varepsilon\le1,\qquad 4C_Va'e_0^\varepsilon\le1.
```

For every $`A\in\widetilde{\mathcal G}_k`$, all the operators
(2) are invertible. Their inverses
$`S_y(A)`$ are analytic in the connection and satisfy

```math
N_\gamma(S_y(A))\le32a'w_k(y),\qquad
 N_\gamma(\delta_{\alpha,A}S_y(A))\le304a',\qquad
 w_k(y)=
 \begin{cases}1,&k\ge1,\\(1+|y|)^{-1},&k=0.\end{cases}
```

At level zero the first bound also holds in
$`N_\gamma^{\mathrm{ker}}`$; there are no short pairs at that level.
The constants are independent of the level, mesh, volume,
permitted connection, reference mass $`\mu\in(0,1]`$, and resolvent
parameter in its stated range.

Theorem B of FBM1 (Section 5, “Weighted Grassmann block integration”) gives the block-integration identity and determinant localization under Theorem A and the additional weakened-walk hypotheses stated there.


## Navigation

[QEM1 assembly index](../README.md). The published PDFs retain their mathematical text. Links to published outlines use their repository locations; links to withheld manuscripts open the corresponding README. Citations to material outside this assembly remain visible without a download link.
