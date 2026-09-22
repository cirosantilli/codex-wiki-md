<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Cameron-Martin space of a Gaussian random variable in a Banach space](../../../../../cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space.md) is most conveniently defined using the [first Gaussian chaos](../../../../../first-gaussian-chaos.md). Work over the real [separable Banach space](../../../../../separable-banach-space.md) $B$, with continuous [dual space](../../../../../dual-space.md) $B^*$. For a centered [Gaussian random variable in a Banach space](../../../../../gaussian-random-variable-in-a-banach-space.md), define

$$
\mathcal G=\overline{\{\ell(X):\ell\in B^*\}}^{L^2(\Omega)},\qquad Sg=\mathbb E[Xg]\quad(g\in\mathcal G).
$$

The set inside the closure is already a [linear subspace](../../../../../vector-subspace.md). Every $g\in\mathcal G$ is a centered [Gaussian random variable](../../../../../gaussian-random-variable.md). The [Bochner integral](../../../../../bochner-integral.md) defining $S$ exists: [Fernique's theorem](../../../../../fernique-s-theorem.md) states that for some $a>0$, $\mathbb E e^{a\|X\|_B^2}<\infty$, and then [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $\mathbb E\|Xg\|_B<\infty$.

The map $S$ is injective. Indeed, $Sg=0$ implies $\mathbb E[g\ell(X)]=\ell(Sg)=0$ for all $\ell\in B^*$. Density of these observations in $\mathcal G$ then implies $\mathbb Eg^2=0$. Define the [Reproducing kernel Hilbert space](../../../../../reproducing-kernel-hilbert-space.md) by

$$
H=S\mathcal G\subset B,\qquad \langle Sg,Sv\rangle_H=\mathbb E[gv],\qquad \|Sg\|_H=\|g\|_2.
$$

The injectivity makes the [inner product](../../../../../inner-product.md) unambiguous, and the completeness of $\mathcal G$ makes $H$ a [Hilbert space](../../../../../hilbert-space-split.md). The embedding into $B$ is continuous since

$$
\|Sg\|_B\leq(\mathbb E\|X\|_B^2)^{1/2}\|g\|_2.
$$

For $\ell\in B^*$ put $Q\ell=S(\ell(X))$. The [reproducing property](../../../../../reproducing-property.md) is

$$
\langle h,Q\ell\rangle_H=\ell(h),\qquad \langle Q\ell,Qm\rangle_H=\mathbb E[\ell(X)m(X)].
$$

This defines the [Banach-space Gaussian RKHS](../../../../../cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space.md) even for a degenerate [Gaussian measure](../../../../../gaussian-measure.md).

For $h=Sg\in H$, write $\widehat h(X)=g$. There is a measurable coordinate $\widehat h$ on $B$, obtained as a limit in [L2 space](../../../../../l2-space-is-a-hilbert-space.md) of continuous linear observations, and $\widehat h(X)$ has [normal distribution](../../../../../normal-distribution.md) $\mathcal N(0,\|h\|_H^2)$. The [Cameron-Martin theorem for a Gaussian measure](../../../../../cameron-martin-theorem-for-a-gaussian-measure.md), in its real [separable Banach space](../../../../../separable-banach-space.md) form, states that if $\mu$ is the [probability law](../../../../../probability-distribution.md) of $X$, then the [probability law](../../../../../probability-distribution.md) $\mu_h$ of $X+h$ is an [equivalent probability measure](../../../../../equivalent-probability-measure.md) to $\mu$ precisely when $h\in H$. For such a shift,

$$
\frac{d\mu_h}{d\mu}(x)=\exp\!\left(\widehat h(x)-\frac12\|h\|_H^2\right)\quad\text{for }\mu\text{-almost every }x.
$$

For $h\notin H$ the two laws are [mutually singular measures](../../../../../mutually-singular-measures.md). The coordinate $\widehat h$ need not be a continuous functional on $B$, and the sample $X$ need not belong to $H$.

Apply this theorem to the shift $-h$. With $a=\|h\|_H^2/2$, it gives

$$
\mathbb P(X-h\in C)=e^{-a}\mathbb E[\mathbf1_C(X)e^{-\widehat h(X)}].
$$

Choose the measurable coordinate so that $\widehat h(-x)=-\widehat h(x)$ on a symmetric set of full $\mu$-measure. This is possible by taking an almost-surely convergent subsequence of the approximating linear observations and intersecting its convergence set with its negative. Alternatively the joint law of $(X,\widehat h(X))$ is invariant under simultaneous negation, directly from those observations and their [mean-square convergence](../../../../../convergence-in-l2.md). Since $C=-C$ and the centered [Gaussian measure](../../../../../gaussian-measure.md) is symmetric, the two exponential integrals with signs $+$ and $-$ agree. Consequently

$$
\mathbb P(X-h\in C)=e^{-a}\mathbb E[\mathbf1_C(X)\cosh\widehat h(X)]\geq e^{-a}\mathbb P(X\in C),
$$

because $\cosh v\geq1$. The [symmetric Gaussian translation lower bound](../../../../../symmetric-gaussian-translation-lower-bound.md) is therefore

$$
\boxed{\mathbb P(X-h\in C)\geq e^{-\|h\|_H^2/2}\mathbb P(X\in C).}
$$

Only symmetry and Borel measurability of $C$ are required; [convexity](../../../../../convex-function.md) is not needed.

There is one degenerate flaw in the last printed claim. The [separable Banach space](../../../../../separable-banach-space.md) $B=\{0\}$ with $X=0$ has $H=\{0\}$ dense in $B$, and all positive-radius balls have [probability](../../../../../probability.md) one. Nevertheless $\Phi(t)=1$ for every $t>0$. Thus the statement needs the additional hypothesis **$B\ne\{0\}$**. If the course convention excludes the zero space, this hypothesis is already implicit.

Under this necessary hypothesis, density of $H$ implies that $H$ contains a nonzero vector. Given $0<a<b$, scale that vector to obtain $h\in H$ with $\|h\|_B=(a+b)/2$, and choose $0<\delta<(b-a)/2$. The [triangle inequality](../../../../../triangle-inequality.md) gives

$$
\|x-h\|_B\leq\delta\quad\Longrightarrow\quad a<\|x\|_B<b.
$$

The centered closed ball $C_\delta=\{x:\|x\|_B\leq\delta\}$ is a symmetric [Borel set](../../../../../borel-set.md). Apply the [symmetric Gaussian translation lower bound](../../../../../symmetric-gaussian-translation-lower-bound.md) to get

$$
\begin{aligned}
\Phi(b)-\Phi(a)&=\mathbb P(a<\|X\|_B\leq b)\\
&\geq\mathbb P(\|X-h\|_B\leq\delta)\\
&\geq e^{-\|h\|_H^2/2}\Phi(\delta)>0.
\end{aligned}
$$

Hence **the Gaussian norm distribution is strictly increasing when $B$ is nonzero**. This proves the [strict increase of a Gaussian norm distribution](../../../../../strict-increase-of-a-gaussian-norm-distribution.md) without assuming that its distribution has a density or that spheres have zero [probability](../../../../../probability.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 217](../../paper-217-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
