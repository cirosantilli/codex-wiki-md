<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [Fredholm index](../../../../../fredholm-index.md) measures the finite-dimensional obstruction to inverting an operator. For a [bounded operator](../../../../../continuous-linear-operator.md) $T:H_1\to H_2$ between [Hilbert spaces](../../../../../hilbert-space-split.md), the [Fredholm](../../../../../fredholm-operator.md) conditions are that its [range of a bounded linear operator](../../../../../range-of-a-bounded-linear-operator.md) is closed and its [kernel](../../../../../kernel-of-a-linear-map.md) and [cokernel](../../../../../cokernel.md) are finite-dimensional. The [orthogonal complement](../../../../../orthogonal-complement.md) of the range is $\ker T^*$, so

$$
\boxed{\operatorname{ind}T=\dim\ker T-\dim\ker T^*.}
$$

An [invertible linear map](../../../../../invertible-linear-map.md) has [Fredholm index](../../../../../fredholm-index.md) zero; the converse needs an additional finite-dimensional correction, since an operator can have equally large [kernel](../../../../../kernel-of-a-linear-map.md) and [cokernel](../../../../../cokernel.md).

First construct an inverse up to [finite-rank operators](../../../../../finite-rank-operator.md). On $(\ker T)^\perp$, the restriction of $T$ is a bounded bijection onto its closed range, with bounded inverse by the [bounded inverse theorem](../../../../../bounded-inverse-theorem.md). Extend that inverse by zero on $(\operatorname{ran}T)^\perp$, obtaining $S:H_2\to H_1$. Then

$$
ST=I-P_{\ker T},\qquad TS=I-P_{\ker T^*}.
$$

Conversely, suppose $ST-I$ and $TS-I$ are [compact operators](../../../../../compact-operator-split.md). On $\ker T$, the first identity expresses the identity as a [compact operator](../../../../../compact-operator-split.md), so this [kernel](../../../../../kernel-of-a-linear-map.md) is finite-dimensional. If $T$ were not bounded below on $(\ker T)^\perp$, there would be unit [vectors](../../../../../vector.md) $x_j$ in that complement with $Tx_j\to0$. Write $ST=I+K$. [Compactness](../../../../../compact-space.md) of $K$ gives a subsequence for which $Kx_j$ converges, hence $x_j=STx_j-Kx_j$ converges to a unit [vector](../../../../../vector.md) $x$ in $(\ker T)^\perp$ with $Tx=0$, a contradiction. This lower bound makes the range closed. Applying the analogous argument to $T^*$, using $S^*T^*=I+K'^*$, proves that its [kernel](../../../../../kernel-of-a-linear-map.md) is finite-dimensional. This proves the [Atkinson theorem](../../../../../atkinson-theorem.md): a [bounded operator](../../../../../continuous-linear-operator.md) is [Fredholm](../../../../../fredholm-operator.md) exactly when it has an inverse modulo [compact operators](../../../../../compact-operator-split.md). For operators on one [Hilbert space](../../../../../hilbert-space-split.md) this says that its image in the [Calkin algebra](../../../../../calkin-algebra.md) is invertible.

The [Fredholm index](../../../../../fredholm-index.md) is stable. Decompose the domain as $N\oplus N^\perp$, where $N=\ker T$, and the target as $C\oplus R$, where $C=\ker T^*$ and $R=\operatorname{ran}T$. A sufficiently small [norm](../../../../../norm.md) perturbation has block [matrix](../../../../../matrix.md)

$$
T+E=\begin{pmatrix}a&b\\c&D\end{pmatrix},\qquad D:N^\perp\longrightarrow R\text{ invertible}.
$$

Multiplying by invertible triangular block [matrices](../../../../../matrix.md) reduces this [matrix](../../../../../matrix.md) to the [direct sum](../../../../../direct-sum.md) of $D$ and the [Schur complement](../../../../../schur-complement.md) $a-bD^{-1}c:N\to C$. The latter's [kernel](../../../../../kernel-of-a-linear-map.md) [dimension](../../../../../dimension-vector-space.md) minus [cokernel](../../../../../cokernel.md) [dimension](../../../../../dimension-vector-space.md) is $\dim N-\dim C$, whatever its [rank](../../../../../rank-one-quadratic-form.md). Therefore the Fredholm set is open and the index is locally constant. If $K$ is compact, the same parametrix works modulo [compact operators](../../../../../compact-operator-split.md) for every $T+tK$, $0\leq t\leq1$. Local constancy along this path gives

$$
\operatorname{ind}(T+K)=\operatorname{ind}T.
$$

For [Fredholm operators](../../../../../fredholm-operator.md) $A:H_1\to H_2$ and $B:H_2\to H_3$, multiplication of parametrices shows that $BA$ is Fredholm. Its index is additive. Here is a direct proof, rather than an assertion of additivity. There is an [exact sequence](../../../../../exact-sequence.md) of finite-dimensional spaces

$$
0\longrightarrow\ker A\longrightarrow\ker BA
\xrightarrow{A}\ker B\longrightarrow\operatorname{coker}A
\xrightarrow{B}\operatorname{coker}BA
\longrightarrow\operatorname{coker}B\longrightarrow0.
$$

The map from $\ker B$ takes a [vector](../../../../../vector.md) to its class modulo $\operatorname{ran}A$; the next takes the class of $y$ to that of $By$; the last is the quotient map. For example, a class $y+\operatorname{ran}A$ lies in the [kernel](../../../../../kernel-of-a-linear-map.md) of the middle map exactly when $By=BAx$ for some $x$, so $y-Ax\in\ker B$. This verifies the only less immediate exactness assertion; the others follow directly from their definitions. Alternating the [dimensions](../../../../../dimension-vector-space.md) gives

$$
\operatorname{ind}(BA)=\operatorname{ind}B+\operatorname{ind}A.
$$

Also $\operatorname{ind}T^*=-\operatorname{ind}T$, and indices add under [direct sums](../../../../../direct-sum.md). For $I+K$ with $K$ compact, the index is zero, so [injectivity](../../../../../injective-function.md) is equivalent to [surjectivity](../../../../../surjective-function.md). More generally $Tx=f$ is solvable exactly when $f$ is orthogonal to $\ker T^*$: these are the finitely many compatibility conditions in the [Fredholm alternative](../../../../../fredholm-alternative.md).

[Toeplitz operators](../../../../../toeplitz-operator.md) exhibit how this analytic index detects a topological winding. Let $H^2\subset L^2(S^1)$ be the [Hardy space of the circle](../../../../../hardy-space-of-the-circle.md), spanned by $1,z,z^2,\ldots$, and let $P$ be its [orthogonal projection](../../../../../orthogonal-projection.md). For a continuous symbol $g$, define $T_g=P M_g|_{H^2}$, where $M_g$ is multiplication by $g$. Then $\|T_g\|\leq\|g\|_\infty$. The product defect is

$$
T_fT_g-T_{fg}=-P M_f(I-P)M_g|_{H^2}.
$$

For [trigonometric polynomials](../../../../../trigonometric-polynomial.md) the crossing of negative and nonnegative [Fourier modes](../../../../../fourier-mode.md) has finite [rank](../../../../../rank-one-quadratic-form.md). Uniform approximation of continuous symbols by [trigonometric polynomials](../../../../../trigonometric-polynomial.md), together with the displayed [norm](../../../../../norm.md) estimate, therefore makes this defect a [compact operator](../../../../../compact-operator-split.md) for all continuous $f,g$. If $g$ is nowhere zero, $1/g$ is continuous and $T_{1/g}$ is a two-sided parametrix modulo [compact operators](../../../../../compact-operator-split.md). Thus $T_g$ is Fredholm.

The converse is instructive. If $g(\zeta)=0$ at $\zeta\in S^1$, consider the normalized Hardy [kernels](../../../../../kernel-of-a-linear-map.md)

$$
k_{r,\zeta}(z)=\frac{\sqrt{1-r^2}}{1-r\overline\zeta z},\qquad 0<r<1.
$$

Their [norms](../../../../../norm.md) are one, their individual [Fourier coefficients](../../../../../fourier-coefficient.md) tend to zero as $r\uparrow1$, and hence they converge weakly to zero. Their squared moduli are the [Poisson kernel](../../../../../poisson-kernel-for-the-upper-half-plane.md), so continuity of $g$ gives

$$
\|T_g k_{r,\zeta}\|_2^2\leq\|gk_{r,\zeta}\|_2^2
=\int_{S^1}|g(z)|^2|k_{r,\zeta}(z)|^2\,\frac{|dz|}{2\pi}\longrightarrow0.
$$

A [Fredholm operator](../../../../../fredholm-operator.md) is bounded below off its finite-dimensional [kernel](../../../../../kernel-of-a-linear-map.md). The projection of these weakly vanishing [vectors](../../../../../vector.md) onto that [kernel](../../../../../kernel-of-a-linear-map.md) tends to zero, contradicting this lower bound. Thus **a continuous-symbol [Toeplitz operator](../../../../../toeplitz-operator.md) is Fredholm exactly when its symbol never vanishes**. Applying the same argument to $g-\lambda$ gives its [essential spectrum](../../../../../essential-spectrum-of-a-closed-operator.md) as $g(S^1)$, with essential [spectrum](../../../../../spectrum-functional-analysis.md) defined by failure of the Fredholm property.

For nonvanishing $g$, let $m=\operatorname{wind}(g,0)$. Lifting a continuous argument of $g(e^{it})$ on $0\leq t\leq2\pi$ gives an argument change $2\pi m$. After division by $z^m$, its argument has matching endpoints, so there is a [continuous function](../../../../../continuous-function.md) $h:S^1\to\mathbb C$ with $g(z)=z^m e^{h(z)}$. The nonvanishing-symbol homotopy $g_t=z^m e^{th}$ reduces the index to that of $T_{z^m}$. For $m\geq0$ this is the $m$th power of the [unilateral shift operator](../../../../../unilateral-shift-operator.md), whose [kernel](../../../../../kernel-of-a-linear-map.md) is zero and whose range has codimension $m$. For $m<0$ it is the $(-m)$th power of the adjoint shift, whose [kernel](../../../../../kernel-of-a-linear-map.md) has [dimension](../../../../../dimension-vector-space.md) $-m$ and whose range is all of $H^2$. Consequently

$$
\boxed{\operatorname{ind}T_g=-\operatorname{wind}(g,0).}
$$

The minus sign comes from counting missing nonnegative [Fourier modes](../../../../../fourier-mode.md). This is a concrete bridge between the [Fredholm index](../../../../../fredholm-index.md), stability under compact perturbations, and the [winding number](../../../../../winding-number.md) of a loop.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
