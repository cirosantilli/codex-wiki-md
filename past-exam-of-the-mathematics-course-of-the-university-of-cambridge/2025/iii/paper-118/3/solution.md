<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Choose holomorphic coordinates centered at $p$. Locally, the [blowup of a complex manifold at a point](../../../../../blowup-of-a-complex-manifold-at-a-point.md) is

$$
\widetilde{\mathbb C^n}=\{(z,[\ell])\in\mathbb C^n\times\mathbb{CP}^{n-1}:z\in\ell\},
$$

with $\sigma(z,[\ell])=z$; away from $p$ this is an isomorphism, so it glues to $X\setminus\{p\}$. The [exceptional divisor](../../../../../exceptional-divisor.md) is $E=\sigma^{-1}(p)\cong\mathbb{CP}^{n-1}$.

The [proper transform](../../../../../strict-transform.md) is the closure of $\sigma^{-1}(Y\setminus\{p\})$. If $p\notin Y$, it is isomorphic to $Y$. If $p\in Y$, the holomorphic [implicit function theorem](../../../../../implicit-function-theorem.md) supplies coordinates in which $Y=\{z_1=0\}$. In the blowup chart with $z_i=t$ and $z_j=tu_j$ for $j\ne i$, every chart with $i\ne1$ describes the proper transform by $u_1=0$, while the chart $i=1$ does not meet it. These are smooth coordinate hypersurfaces, so $\widetilde Y$ is smooth.

For a divisor $D$, the [line bundle associated to a divisor](../../../../../line-bundle-associated-to-a-divisor.md) $\mathcal O(D)$ consists locally of [meromorphic functions](../../../../../meromorphic-function.md) $f$ such that $(f)+D\geq0$. Pulling back a local defining function for $Y$ shows that its divisor is

$$
\sigma^*Y=\widetilde Y+mE,
$$

where $m$ is the [order of vanishing](../../../../../order-of-vanishing.md) at $p$ of a local defining function for $Y$. Therefore

$$
\sigma^*\mathcal O(Y)\cong\mathcal O(\widetilde Y+mE).
$$

Because $Y$ is smooth, $m=1$ when $p\in Y$ and $m=0$ when $p\notin Y$.

Applying the definition with $D=E$ gives directly

$$
H^0(\widetilde X,\mathcal O(E))\cong\{f\text{ meromorphic on }\widetilde X:(f)+E\geq0\}.
$$

The map sends a section to its local meromorphic coefficient relative to the canonical meromorphic section of $\mathcal O(E)$; the divisor inequality is exactly the condition that these coefficients define a holomorphic section, and the inverse construction is local multiplication by that canonical section.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 118](../../paper-118-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
