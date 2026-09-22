<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The exponential series is absolutely norm-convergent, since $\sum_{n\ge1}\|x^n\|/n!\le e^{\|x\|}-1$. [Completeness](../../../../../completeness.md) defines the [Banach algebra exponential](../../../../../banach-algebra-exponential.md) $e^x\in A$. If $xy=yx$, absolute convergence permits rearrangement of the product series, and the binomial identity gives

$$
e^xe^y=\sum_{n=0}^\infty\sum_{j=0}^n\frac{x^jy^{n-j}}{j!(n-j)!}=\sum_{n=0}^\infty\frac{(x+y)^n}{n!}=e^{x+y}.
$$

Taking $y=-x$ yields **$(e^x)^{-1}=e^{-x}$**.

For the spectral hypothesis, put $K=\sigma_A(u)$. Its complement has an [open](../../../../../open-set.md), hence [path-connected](../../../../../path-connected-space.md), unbounded component containing $0$. Join $0$ to an exterior point by a simple polygonal arc in that component, and continue it to infinity, avoiding $K$. Removing this polygonal slit gives a [simply connected](../../../../../simply-connected-space.md) [open](../../../../../open-set.md) neighborhood $\Omega$ of $K$ on which $z$ has a [branch of the complex logarithm](../../../../../branch-of-the-complex-logarithm.md) $L(z)$. The [holomorphic functional calculus](../../../../../holomorphic-functional-calculus.md) therefore defines $x=L(u)$ and its composition rule gives

$$
\boxed{e^x=(e^L)(u)=u}.
$$

The relevant slit is chosen through the resolvent, not assumed to be a fixed negative-real-axis cut. This is the [logarithm from a spectral slit in a Banach algebra](../../../../../logarithm-from-a-spectral-slit-in-a-banach-algebra.md).

Let $H$ be the [subgroup](../../../../../subgroup.md) of finite products of exponentials. It is a [subgroup](../../../../../subgroup.md) because $e^ae^{-a}=1$ and reversing a product gives its inverse. Each product is joined to $1$ by $t\mapsto e^{ta_1}\cdots e^{ta_m}$, so $H\subseteq G_0$. Conversely, if $\|v-1\|<1$, the convergent logarithm series

$$
\log v=\sum_{n=1}^\infty\frac{(-1)^{n+1}(v-1)^n}{n}
$$

satisfies $e^{\log v}=v$, by the scalar analytic identity and functional calculus. Thus $H$ contains a neighborhood of $1$. Its translates make $H$ [open](../../../../../open-set.md), and all other cosets are [open](../../../../../open-set.md) too, making $H$ [closed](../../../../../closed-set.md). [Connectedness](../../../../../connected-space.md) forces $G_0\subseteq H$. Finally $ge^ag^{-1}=e^{gag^{-1}}$, so $H$ is normal. Therefore

$$
\boxed{G_0=H=\{e^{a_1}\cdots e^{a_m}:m\ge0,\ a_j\in A\}},
$$

an open-and-closed [normal subgroup](../../../../../normal-subgroup.md). This is the [identity component of Banach-algebra invertibles](../../../../../identity-component-of-banach-algebra-invertibles.md); finite products are essential and are not asserted to be single exponentials.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
