<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

With $s=0$, the [equilibria](../../../../../equilibrium-of-an-autonomous-differential-equation.md) satisfy

$$
g\left(\frac{kg}{1+g^2}-1\right)=0.
$$

Besides $g=0$, the two positive equilibria are

$$
g_\pm=\frac{k\pm\sqrt{k^2-4}}2,
\qquad
g_-<1<g_+,
$$

where $g_-g_+=1$. Since

$$
\partial_gf(g,0)=\frac{2kg}{(1+g^2)^2}-1,
$$

the nonzero equilibrium relation $k=(1+g^2)/g$ gives

$$
\partial_gf(g,0)=\frac{1-g^2}{1+g^2}.
$$

The [fixed point stability for an autonomous differential equation](../../../../../fixed-point-stability-for-an-autonomous-differential-equation.md) therefore shows that $g=0$ and $g_+$ are stable, while $g_-$ is unstable. The graph of $f(g,0)$ starts at zero with negative slope, crosses upward at $g_-$, crosses downward at $g_+$, and tends to $-\infty$ as $g\to\infty$.

For a constant input $s$, write the equilibrium equation as

$$
s=h(g),
\qquad
h(g)=g-\frac{kg^2}{1+g^2}.
$$

The low stable equilibrium and the intervening unstable equilibrium coalesce in a [saddle-node bifurcation](../../../../../saddle-node-bifurcation.md). More precisely, let $g_c$ be the first positive solution of

$$
h'(g_c)=1-\frac{2kg_c}{(1+g_c^2)^2}=0
$$

and define

$$
\boxed{s_c(k)=h(g_c)
=g_c-\frac{kg_c^2}{1+g_c^2}.}
$$

Equivalently, $f(g_c,s_c)=0$ and $\partial_gf(g_c,s_c)=0$, with $g_c$ on the low-concentration branch. If $s_1>s_c(k)$, that branch no longer exists. Holding the input long enough carries the trajectory into the [basin of attraction](../../../../../basin-of-attraction.md) of the high state. When the input returns to zero, the concentration converges to

$$
\boxed{g^*=g_+=\frac{k+\sqrt{k^2-4}}2.}
$$

This is the [saturating autocatalytic switch](../../../../../saturating-autocatalytic-switch.md).

For $k\gg1$, the threshold occurs at $g=O(k^{-1})$, so

$$
f(g,s)=s+kg^2-g+O(kg^4).
$$

The approximate double-root conditions are

$$
s+kg^2-g=0,
\qquad
2kg-1=0.
$$

Thus $g_c\simeq1/(2k)$ and

$$
\boxed{s_c(k)\simeq\frac1{4k}.}
$$

Hence the constant in $s_c(k)\simeq Ck^{-1}$ is $\boxed{C=1/4}$, as recorded by the [strong-autocatalysis switching threshold](../../../../../strong-autocatalysis-switching-threshold.md).

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
