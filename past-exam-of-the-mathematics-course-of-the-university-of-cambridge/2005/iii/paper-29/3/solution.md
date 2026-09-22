<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $f(z)=\sum_{n\geq0}z^{l^n}$. The authoritative PDF has exponent $l^n$; the geometric-series exponent in the converted TeX is a transcription error. On the [unit disk](../../../../../unit-disk.md) this [Fredholm series](../../../../../fredholm-lacunary-series.md) satisfies

$$
\boxed{f(z^l)=f(z)-z.}
$$

First it is transcendental as a function. If $\zeta^{l^s}=1$, the terms with $n\geq s$ in $f(\rho\zeta)$ are the positive terms $\rho^{l^n}$ and their sum tends to infinity as $\rho\uparrow1$; the finite preceding sum stays bounded. Thus every [root of unity](../../../../../root-of-unity.md) of $l$-power order is a singularity. These roots are dense on the unit circle. An algebraic function has only finitely many possible branch points or poles, as seen from its defining [polynomial](../../../../../polynomial-split.md)'s leading coefficient and discriminant. Hence $f$ cannot be algebraic over $\mathbb C(z)$.

Suppose now that $\alpha$ is algebraic, $0<|\alpha|<1$, and $a=f(\alpha)$ is algebraic. For a positive [integer](../../../../../integer.md) $N$, a [polynomial](../../../../../polynomial-split.md) $P(X,Y)\in\mathbb Z[X,Y]$, nonzero and of degree at most $N$ in each variable, can be chosen so that

$$
G(z)=P(z,f(z))=O(z^T),\qquad T=(N+1)^2-1.
$$

Indeed the first $T$ Taylor coefficients impose $T$ homogeneous [integer](../../../../../integer.md) equations on $(N+1)^2$ coefficients. There is a nonzero rational solution, which can be cleared to an [integer](../../../../../integer.md) one. Functional transcendence ensures $G$ is not identically zero.

Iterating the [functional equation](../../../../../functional-equation.md) gives

$$
f(\alpha^{l^k})=a-\sum_{j=0}^{k-1}\alpha^{l^j}.
$$

Thus $\beta_k=G(\alpha^{l^k})$ belongs to the fixed field $K=\mathbb Q(\alpha,a)$ and is nonzero for all sufficiently large $k$, since a nonzero analytic $G$ has no sufficiently small nonzero zeros. Its analytic upper bound is

$$
|\beta_k|\leq C_P|\alpha|^{T l^k}.
$$

Choose an [integer](../../../../../integer.md) $q\geq1$ making $q\alpha,qa$ [algebraic integers](../../../../../algebraic-integer.md), let $d=[K:\mathbb Q]$, and choose $M\geq2$ bounding every conjugate of $\alpha$ and $a$. Then $q^{l^k}\alpha^{l^k}$ and $q^{l^{k-1}}f(\alpha^{l^k})$ are [algebraic integers](../../../../../algebraic-integer.md). Therefore

$$
D_k\beta_k\text{ is integral},\qquad D_k=q^{N(l^k+l^{k-1})}.
$$

For every embedding $\sigma$ of $K$, the coefficient sum $L(P)$ bounds the [polynomial](../../../../../polynomial-split.md) and gives

$$
|\sigma\beta_k|\leq L(P)(k+1)^N M^{N(l^k+l^{k-1})}.
$$

Taking the norm of the nonzero integral $D_k\beta_k$ yields a nonzero rational [integer](../../../../../integer.md), of absolute value at least one. Consequently

$$
\log|\beta_k|\geq-NC_0l^k-O_N(\log(k+1)),\qquad
C_0=(1+1/l)\big[d\log q+(d-1)\log M\big].
$$

On the other hand the upper bound is $\log|\beta_k|\leq-T\lambda l^k+O_P(1)$, where $\lambda=-\log|\alpha|>0$. Choose $N$ so large that $T\lambda>NC_0$, possible because $T=N^2+2N$. Letting $k\to\infty$ contradicts the two bounds. This proves, by the [Mahler method](../../../../../mahler-method.md), **$\boxed{f(\alpha)\text{ is transcendental for }0<|\alpha|<1}$** at every algebraic $\alpha$.

For the shorter rational-approximation argument at $1/2$, truncate after $n=m$ and write $s_m=p_m/q_m$ with $q_m=2^{l^m}$. The numerator is odd because its last summand is one and all previous summands are even, so this fraction is reduced. The tail satisfies

$$
0<f(1/2)-\frac{p_m}{q_m}<2\,q_m^{-l}.
$$

The value is irrational: if it were $P/Q$, the positive difference from a truncation would be at least $1/(Qq_m)$, contradicting the tail bound for large $m$. If it were algebraic irrational and $l\geq3$, choose $0<\epsilon<l-2$. Eventually the displayed upper bound is below $q_m^{-2-\epsilon}$ for infinitely many reduced fractions. The [Roth theorem](../../../../../roth-s-theorem.md) says that an algebraic irrational admits only finitely many such approximations. This contradiction proves transcendence directly. The argument does not cover $l=2$, because its exponent is not strictly larger than two; the Mahler proof does cover that case.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
