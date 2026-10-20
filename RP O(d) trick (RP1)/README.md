# RP O(d) trick (RP1)

**Disclaimer:** these documents are largely LLM-created. Their correctness has not been satisfactorily verified.

Project codename: **RP1**.

- **RP1O1** — [Reflection positivity to rotations: expanded proof outline](RP1O1.pdf).
- **RP1M1** — *Rotation invariance from lattice symmetry and reflection positivity* (manuscript to be added).

## Main theorem

The statement below is taken from Theorem A of **RP1M1**, with its notation from the manuscript. The TeX formatting and macros have been adapted for GitHub.

Fix a number $`d\geq 2`$, and consider $`d`$-dimensional Euclidean spacetime $`\mathbb{R}^d`$.

Here $`\mathcal{T}`$ is a finite-dimensional real orthogonal representation of $`\mathrm{O}(d)`$ whose planar rotation weights lie in $`\{-2,-1,0,1,2\}`$.

The space $`\mathcal{S}=\mathcal{S}(\mathbb{R}^d;\mathcal{T})`$ is the Fréchet space of real
Schwartz tests, and $`\mathcal{S}'`$ is its continuous dual with the weak-$`*`$
topology. The Euclidean inner product on $`\mathcal{T}`$ fixes the pointwise norm
and hence the $`L^1`$ and $`L^2`$ norms.

By a “random distribution” is meant a Borel probability measure

```math
\mu:\mathrm{Borel}(\mathcal{S}')\to [0,1]
```

on $`\mathcal{S}'`$, which we assume possesses well-defined moments $`S_N: \mathcal{S}^N\to \mathbb{R}`$. Let $`\Phi:\mathcal{S}\to \mathbb{C}`$ denote the characteristic function

```math
\Phi(\chi) = \int_{\mathcal{S}'} e^{iF(\chi)} \,\mathrm{d} \mu(F)
```

of the measure.

Let $`\mathcal{S}_N \subset \mathcal{S}^N`$ denote the set of tuples $`\chi=(\chi_1,\dots,\chi_N)`$ such that the test functions $`\chi_\bullet`$'s have pairwise disjoint supports.

Let $`\mathcal{N}`$ denote the set of all hyperplanes $`\subset \mathbb{R}^d`$ of the form

```math
\{x_j=0\}\quad(0\leq j\leq d-1),\qquad \{x_j+x_k=0\},\quad \{x_j-x_k=0\}
```

for $`0\leq j<k\leq d-1`$ in the latter two families.

For an isometry $`T(\mathbf{x})=g\mathbf{x}+\mathbf{a}`$, our pullback convention is

```math
(T^*\chi)(\mathbf{x})=\rho(g)\chi(T\mathbf{x}),\qquad
 (T_1T_2)^*=T_2^*T_1^*.
```

Here $`\rho(g)`$ is the pullback action on the tensor indices; thus
$`\rho(g_1g_2)=\rho(g_2)\rho(g_1)`$. It is an isometry for real $`g`$.

**Theorem A.**

Suppose that:

**(i)**  There exists a constant $`C>0`$ such that

```math
\int_{\mathcal{S}'} e^{F(\chi)} \,\mathrm{d} \mu(F) \leq e^{C(\lVert\chi\rVert_{L^1}+\lVert\chi\rVert_{L^2}^2)}
```

for every real $`\chi\in\mathcal{S}`$.

**(ii)**
The measure is invariant under spacetime translations. That is, for any $`T:\mathbb{R}^d\to \mathbb{R}^d`$ of the form $`T(\mathbf{x})=\mathbf{x}+\mathbf{a}`$ for $`\mathbf{a}\in \mathbb{R}^d`$,

```math
\Phi(T^* \chi) = \Phi(\chi).
```

**(iii)** The measure is reflection positive across each of the hyperplanes $`H\in \mathcal{N}`$: for any finite sequence $`\chi_0,\chi_1,\dots \in \mathcal{S}`$ of test functions supported on one side of $`\mathbb{R}^d\backslash H`$, and for any $`z_\bullet\in \mathbb{C}`$,

```math
\sum_{a,b} \bar{z}_a z_b \Phi(\chi_a - \Theta^* \chi_b ) \geq 0,
```

where $`\Theta:\mathbb{R}^d\to\mathbb{R}^d`$ denotes reflection across the hyperplane $`H`$.

Then the measure is rotationally-invariant in the sense of Osterwalder--Schrader, meaning $`S_N(R^* \chi) = S_N(\chi)`$ for all $`R\in \mathrm{O}(d)`$ and $`\chi\in \mathcal{S}_N`$.

Here, $`R^* \chi=(R^* \chi_1,\dots,R^* \chi_N)`$.
