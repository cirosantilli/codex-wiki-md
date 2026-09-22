<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat\varphi(\xi)=\int e^{-ix\cdot\xi}\varphi(x)\,dx$ and $D_j=-i\partial_j$, so $\widehat{P(D)u}=P(\xi)\widehat u$. All [distribution](../../../../../distribution-mathematical-analysis.md) pairings use complex [bilinearity](../../../../../bilinearity.md), and the [formal transpose](../../../../../formal-transpose-of-a-differential-operator.md) is $P(-D)$, without [complex conjugation](../../../../../complex-conjugation.md) of the coefficients. If $D_j$ instead denotes $\partial_j$, the Fourier multiplier is $P(i\xi)$; the argument below is unchanged after this substitution.

For a nonempty [compact convex set](../../../../../compact-convex-set.md) $K\subset\mathbb R^n$, let $H_K(\eta)=\sup_{x\in K}x\cdot\eta$ be its [support function](../../../../../support-function.md). The [Paley–Wiener–Schwartz theorem](../../../../../paley-wiener-schwartz-theorem.md) says that the [Fourier transform](../../../../../fourier-transform.md) is a bijection between [distributions](../../../../../distribution-mathematical-analysis.md) supported in $K$ and [entire functions](../../../../../entire-function.md) $F$ on $\mathbb C^n$ for which

$$
\boxed{|F(\zeta)|\leq C(1+|\zeta|)^N e^{H_K(\operatorname{Im}\zeta)}}
$$

for some $C>0$ and nonnegative integer $N$. In particular, support in $\overline B_R$ is equivalent to the bound with $e^{R|\operatorname{Im}\zeta|}$. Convexity is essential in the precise support formulation: the [support function](../../../../../support-function.md) of a set equals that of its [convex hull](../../../../../convex-hull.md).

Suppose first that $u$ is a [compactly supported distribution](../../../../../compactly-supported-distribution.md) with support in $K$. Define $F(\zeta)=\langle u,e^{-ix\cdot\zeta}\rangle$, inserting any [cutoff function](../../../../../cutoff-function.md) equal to one near $K$ when viewing $u$ on [test functions](../../../../../test-function.md). A fixed cutoff and the finite [order of a distribution](../../../../../order-of-a-distribution.md) estimate permit differentiation of the pairing in each complex variable, giving $\partial_\zeta^\alpha F=\langle u,(-ix)^\alpha e^{-ix\cdot\zeta}\rangle$. The [exponential function](../../../../../exponential-function.md)'s [power series](../../../../../power-series.md) converges with every required derivative on a fixed compact set; hence $F$ is an [entire function](../../../../../entire-function.md). On real frequencies it agrees with the [Fourier transform of a compactly supported distribution](../../../../../fourier-transform-of-a-compactly-supported-distribution.md).

The exact exponential indicator needs a shrinking [cutoff function](../../../../../cutoff-function.md), rather than one fixed outside $K$. Choose $\chi_\varepsilon=1$ near $K$, with support in $K+B_{2\varepsilon}$ and $\|\partial^\alpha\chi_\varepsilon\|_\infty\leq C_\alpha\varepsilon^{-|\alpha|}$ for $0<\varepsilon\leq1$. Such a cutoff is obtained by convolving the indicator of $K+B_\varepsilon$ with a [mollifier](../../../../../mollifier.md) supported in $B_{\varepsilon/2}$. On one fixed ball containing all these supports, the finite [order of a distribution](../../../../../order-of-a-distribution.md) bound is

$$
|\langle u,\theta\rangle|\leq C_0\max_{|\alpha|\leq m}\|\partial^\alpha\theta\|_\infty.
$$

The [Leibniz rule](../../../../../leibniz-rule.md) applied to $\theta=\chi_\varepsilon e^{-ix\cdot\zeta}$ therefore gives

$$
|F(\zeta)|\leq C_1\varepsilon^{-m}(1+|\zeta|)^m
e^{H_K(\operatorname{Im}\zeta)+2\varepsilon|\operatorname{Im}\zeta|}.
$$

Taking $\varepsilon=(1+|\zeta|)^{-1}$ proves the required bound, with $N=2m$ and a fixed additional factor at most $e^2$.

Conversely, suppose $F$ is an [entire function](../../../../../entire-function.md) with the displayed bound. Its real restriction has [polynomial growth](../../../../../polynomial-growth.md), so its inverse [Fourier transform](../../../../../fourier-transform.md) defines a [tempered distribution](../../../../../tempered-distribution.md) by

$$
\langle u,\varphi\rangle=(2\pi)^{-n}\int_{\mathbb R^n}F(\xi)\widehat\varphi(-\xi)\,d\xi,
\qquad \varphi\in\mathcal S.
$$

Rapid decay of the [Schwartz function](../../../../../schwartz-function.md) $\widehat\varphi$ makes this integral absolutely convergent and continuous in the [Schwartz space](../../../../../schwartz-space.md) topology.

To determine the [support of a distribution](../../../../../support-of-a-distribution.md), take a [test function](../../../../../test-function.md) supported in a half-space $x\cdot\omega\geq H_K(\omega)+\delta$, where $|\omega|=1$ and $\delta>0$. The [contour-shift proof of the Paley–Wiener–Schwartz theorem](../../../../../contour-shift-proof-of-the-paley-wiener-schwartz-theorem.md) gives, for each $t\geq0$,

$$
\langle u,\varphi\rangle=(2\pi)^{-n}\int_{\mathbb R^n}
F(\xi+it\omega)\widehat\varphi(-\xi-it\omega)\,d\xi.
$$

Here is the estimate that justifies both the shift and its limiting use. Since $\widehat\varphi(-\xi-it\omega)=\int e^{ix\cdot\xi}e^{-t x\cdot\omega}\varphi(x)\,dx$, repeated [integration by parts](../../../../../integration-by-parts.md) with $1-\Delta_x$ yields

$$
|\widehat\varphi(-\xi-it\omega)|
\leq C_L(1+t)^{2L}e^{-t(H_K(\omega)+\delta)}(1+|\xi|^2)^{-L}.
$$

For fixed $t$, the same estimate is uniform over the imaginary strip from $0$ to $t\omega$. Rotate coordinates so $\omega$ is the first coordinate direction, apply the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) on truncated rectangles, and let their real edges tend to infinity. If $2L>N+n$, the boundary integrals vanish and the horizontal integrals converge absolutely; thus the claimed shift is valid. Using $H_K(t\omega)=tH_K(\omega)$ now bounds the pairing by

$$
C'(1+t)^{N+2L}e^{-\delta t}
\int_{\mathbb R^n}(1+|\xi|)^{N-2L}\,d\xi,
$$

which tends to zero. A [separating hyperplane](../../../../../separating-hyperplane.md) exists at every point outside the [compact convex set](../../../../../compact-convex-set.md) $K$. A finite [partition of unity](../../../../../partition-of-unity.md) on the support of any exterior [test function](../../../../../test-function.md) reduces it to such half-spaces, so $\operatorname{supp}u\subseteq K$. [Fourier inversion](../../../../../fourier-inversion-theorem.md) gives uniqueness; the entire transform of this $u$ agrees with $F$ on $\mathbb R^n$ and hence everywhere, by applying the one-variable [identity theorem](../../../../../identity-theorem.md) successively in each coordinate. This completes both directions.

Now apply this theorem to [compact support solvability for a constant-coefficient ordinary differential equation](../../../../../compact-support-solvability-for-a-constant-coefficient-ordinary-differential-equation.md). If $P$ is a nonzero constant, its kernel is zero and $u=v/P$ is the unique solution. Otherwise write

$$
P(\zeta)=a_m\prod_{j=1}^m(\zeta-\alpha_j),\qquad \alpha_j\ne\alpha_k\quad(j\ne k).
$$

The solution space of $P(-D)\varphi=0$ is

$$
\mathcal N=\operatorname{span}\{e^{-i\alpha_1x},\ldots,e^{-i\alpha_mx}\}.
$$

Indeed these exponentials solve the equation, their initial derivative vectors have a nonzero [Vandermonde determinant](../../../../../vandermonde-determinant.md), and uniqueness for the order-$m$ [ordinary differential equation](../../../../../ordinary-differential-equation.md) makes them a basis. Pairing $P(D)u=v$ with any such solution proves necessity:

$$
\langle v,\varphi\rangle=\langle u,P(-D)\varphi\rangle=0.
$$

For sufficiency, choose $R$ with $\operatorname{supp}v\subseteq[-R,R]$ and let $V(\zeta)=\langle v,e^{-ix\zeta}\rangle$. The assumed annihilation is precisely $V(\alpha_j)=0$ for every $j$. Since all [roots of a polynomial](../../../../../root-of-a-polynomial.md) are simple, $U=V/P$ has removable singularities at every root and is an [entire function](../../../../../entire-function.md). Outside one disk, $|P(\zeta)|\geq c(1+|\zeta|)^m$. Inside that disk, the extended $U$ is bounded. The [polynomial division preservation of exponential type](../../../../../polynomial-division-preservation-of-exponential-type.md) therefore gives

$$
|U(\zeta)|\leq C'(1+|\zeta|)^{N'}e^{R|\operatorname{Im}\zeta|}.
$$

The [Paley–Wiener–Schwartz theorem](../../../../../paley-wiener-schwartz-theorem.md) produces a [compactly supported distribution](../../../../../compactly-supported-distribution.md) $u$ with transform $U$, supported in the same interval. Then $\widehat{P(D)u}=PU=V$, so [Fourier inversion](../../../../../fourier-inversion-theorem.md) gives $P(D)u=v$. Thus

$$
\boxed{v\in P(D)\mathcal E'(\mathbb R)\ \Longleftrightarrow\
\langle v,\varphi\rangle=0\ \text{for every }\varphi\in\mathcal N.}
$$

The compactly supported solution is unique: $P\widehat u=0$ forces the entire transform to vanish off the finitely many roots and hence everywhere. With repeated roots, the corresponding condition would also require derivatives $V^{(k)}(\alpha)=0$, or pairing with $x^k e^{-i\alpha x}$, up to one less than each multiplicity.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 327](../../paper-327-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
