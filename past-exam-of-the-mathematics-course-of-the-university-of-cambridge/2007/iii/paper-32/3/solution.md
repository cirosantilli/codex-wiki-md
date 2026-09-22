<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Fix $T<\infty$ and a standard $d$-dimensional [Brownian motion](../../../../../brownian-motion-split.md) $B$ starting at zero. Let $D_n$ be deterministic nested finite partitions of $[0,T]$ with mesh tending to zero; dyadic partitions are the basic example. Let $B^n$ be the polygonal interpolation through the partition values and put $\mathbf B^n=S_2(B^n)$. The limit is [enhanced Brownian motion](../../../../../enhanced-brownian-motion.md), with increments

$$
\mathbf B_{s,t}=(1,B_{s,t},\mathbb B_{s,t}),\qquad
\mathbb B^{ij}_{s,t}=\int_s^t(B^i_r-B^i_s)\circ dB^j_r.
$$

Here the integral is a [Stratonovich integral](../../../../../stratonovich-integral.md). In terms of [Itô integrals](../../../../../ito-integral.md),

$$
\mathbb B^{ij}_{s,t}=\int_s^t(B^i_r-B^i_s)\,dB^j_r+\tfrac12\delta_{ij}(t-s).
$$

Its symmetric part is $\tfrac12 B_{s,t}^{\otimes2}$, while its antisymmetric part is [Lévy area](../../../../../levy-area.md),

$$
A^{ij}_{s,t}=\tfrac12(\mathbb B^{ij}_{s,t}-\mathbb B^{ji}_{s,t}).
$$

These identities and splitting the integral at an intermediate time give the [Chen identity](../../../../../chen-identity.md), so $\mathbf B$ has values in $G^2(\mathbb R^d)$.

A precise [nested polygonal approximation of Brownian rough paths](../../../../../nested-polygonal-approximation-of-brownian-rough-paths.md) statement is: for every $0<\alpha<1/2$,

$$
\boxed{\rho_\alpha(\mathbf B^n,\mathbf B)\longrightarrow0\quad\text{almost surely},}
$$

where the [rough path metric](../../../../../rough-path-metric.md) used here is

$$
\rho_\alpha(\mathbf X,\mathbf Y)=
\sup_{s<t}\frac{|X_{s,t}-Y_{s,t}|}{|t-s|^\alpha}
+\sup_{s<t}\frac{|\mathbb X_{s,t}-\mathbb Y_{s,t}|}{|t-s|^{2\alpha}}.
$$

In particular, for each $2<p<3$, choosing $1/p<\alpha<1/2$ gives convergence in the inhomogeneous $p$-variation [rough path metric](../../../../../rough-path-metric.md). The limiting signed area is the [Lévy area](../../../../../levy-area.md), and the limiting full second level is Stratonovich, not Itô. This distinction is necessary: a polygonal lift has the prescribed symmetric second level, whereas an Itô lift would lack half the quadratic-variation correction.

Here is a proof sketch emphasizing the nested [martingale](../../../../../martingale-split.md) structure. Set

$$
\mathcal G_n=\sigma(B_t:t\in D_n).
$$

A [Brownian bridge](../../../../../brownian-bridge.md) between two prescribed endpoints has the affine interpolation as conditional mean. Consequently

$$
B^n_t=\mathbb E[B_t\mid\mathcal G_n].
$$

For $i\ne j$ the coordinate processes remain independent when their respective partition values are conditioned on. Approximating the [Itô integral](../../../../../ito-integral.md) by its left sums, conditioning each product, and then taking its $L^2$ limit gives

$$
\mathbb E[\mathbb B^{ij}_{s,t}\mid\mathcal G_n]
=\int_s^t(B^{n,i}_r-B^{n,i}_s)\,dB^{n,j}_r
=\mathbb B^{n,ij}_{s,t}.
$$

Indeed each conditioned factor is its polygonal interpolation, and their sums converge to the ordinary integral of those piecewise linear functions. For a fixed pair $s,t$, the right side is therefore a [martingale](../../../../../martingale-split.md) in the refinement index $n$. It is not being asserted to be a [martingale](../../../../../martingale-split.md) in physical time; polygonal interpolation uses the right endpoint of its current cell.

The union of the partitions is dense. Continuity of $B$ implies that $\mathcal G_\infty=\sigma(\bigcup_n\mathcal G_n)$ contains the full Brownian path and its [stochastic integrals](../../../../../stochastic-integral.md), up to completion. The [martingale convergence theorem](../../../../../martingale-convergence-theorem.md) for [conditional expectations](../../../../../conditional-expectation.md) therefore yields convergence of $B^n_t$ and all off-diagonal $\mathbb B^{n,ij}_{s,t}$ at every fixed pair, almost surely and in $L^q$ for finite $q$. Simultaneously it holds for a countable dense collection of pairs. The diagonal terms must be handled separately:

$$
\mathbb B^{n,ii}_{s,t}=\tfrac12(B^{n,i}_{s,t})^2
\longrightarrow\tfrac12(B^i_{s,t})^2=\mathbb B^{ii}_{s,t}.
$$

They are not [conditional expectations](../../../../../conditional-expectation.md) of the diagonal Brownian second level: the latter would also contain a conditional variance.

Pointwise convergence alone is insufficient for the [rough path metric](../../../../../rough-path-metric.md). The [Burkholder-Davis-Gundy inequalities](../../../../../burkholder-davis-gundy-inequalities.md), [Brownian scaling](../../../../../brownian-scaling.md) and Gaussian increment moments give, for arbitrarily large $q$,

$$
\mathbb E|B_{s,t}|^q\le C_q|t-s|^{q/2},\qquad
\mathbb E|\mathbb B_{s,t}|^q\le C_q|t-s|^q.
$$

Equivalently, using the homogeneous norm on $G^2$, the $q$-th moment of the [Carnot-Carathéodory distance](../../../../../carnot-caratheodory-distance.md) of an increment is bounded by $C_q|t-s|^{q/2}$. The metric form of the [Kolmogorov continuity theorem](../../../../../kolmogorov-continuity-theorem.md), with $q$ chosen large, gives for every $\beta<1/2$ a random $K_\beta$ having all finite moments such that

$$
|B_{s,t}|\le K_\beta|t-s|^\beta,\qquad
|\mathbb B_{s,t}|\le K_\beta^2|t-s|^{2\beta}.
$$

Conditioning these bounds gives

$$
|B^n_{s,t}|\le\mathbb E[K_\beta\mid\mathcal G_n]|t-s|^\beta,
\qquad
|\mathbb B^{n,ij}_{s,t}|\le\mathbb E[K_\beta^2\mid\mathcal G_n]|t-s|^{2\beta}\quad(i\ne j).
$$

The diagonal bounds follow by squaring the first bound. The two conditional-expectation processes are nonnegative [martingales](../../../../../martingale-split.md); the [Doob Lp maximal inequality](../../../../../doob-lp-maximal-inequality.md) makes their suprema over $n$ finite almost surely, with all needed moments. Thus all the polygonal lifts have a common random bound at exponent $\beta$.

These bounds and the [Chen identity](../../../../../chen-identity.md) give joint equicontinuity of the increments as functions of $(s,t)$. Convergence on the dense collection of pairs consequently gives [uniform convergence](../../../../../uniform-convergence.md) of both levels on the time triangle. Take $\alpha<\beta<1/2$. For either level $k=1,2$, with $M$ a common bound and $\varepsilon_n$ its uniform difference, interpolation gives

$$
\sup_{s<t}\frac{|X^{n,(k)}_{s,t}-X^{(k)}_{s,t}|}{|t-s|^{k\alpha}}
\le (2M)^{\alpha/\beta}\varepsilon_n^{\,1-\alpha/\beta}\longrightarrow0.
$$

This proves the stated Hölder [rough path metric](../../../../../rough-path-metric.md) convergence. Finally, for a partition $D$, the $k$-th level difference satisfies

$$
\sum_{[u,v]\in D}|X^{n,(k)}_{u,v}-X^{(k)}_{u,v}|^{p/k}
\le\rho_\alpha(\mathbf B^n,\mathbf B)^{p/k}
\sum_{[u,v]\in D}|v-u|^{\alpha p}
\le\rho_\alpha(\mathbf B^n,\mathbf B)^{p/k}T^{\alpha p},
$$

because $\alpha p>1$. Taking the appropriate powers and suprema proves $p$-variation convergence too. Nesting is what permits the conditional-expectation [martingale](../../../../../martingale-split.md) proof; without nesting one instead needs direct approximation estimates.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
