<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

Use [Minkowski spacetime](../../../../../minkowski-spacetime.md) coordinates $x^\mu=(ct,x,y,z)$ and the [Minkowski metric](../../../../../minkowski-metric.md) of signature $(+,-,-,-)$. For a massive particle with three-velocity $\mathbf v=d\mathbf x/dt$ and $|\mathbf v|<c$, [proper time](../../../../../proper-time.md) satisfies

$$
c^2\,d\tau^2=c^2\,dt^2-|d\mathbf x|^2,\qquad
\frac{dt}{d\tau}=\gamma=\left(1-\frac{|\mathbf v|^2}{c^2}\right)^{-1/2}.
$$

Thus the [four-velocity](../../../../../four-velocity.md) components are

$$
\boxed{U^\mu=(\gamma c,\gamma v_x,\gamma v_y,\gamma v_z)}.
$$

Here upper indices indicate components in the chosen coordinates; lowering with the [Minkowski metric](../../../../../minkowski-metric.md) changes the signs of the spatial components. Its invariant product defined by the [Minkowski metric](../../../../../minkowski-metric.md) is

$$
U\cdot U=(U^0)^2-\sum_{j=1}^3(U^j)^2
=\gamma^2(c^2-|\mathbf v|^2)=c^2.
$$

The [four-momentum](../../../../../four-momentum.md) is $p^\mu=(E/c,\mathbf p)=mU^\mu$, so $E=\gamma mc^2$ and $\mathbf p=\gamma m\mathbf v$. The [Taylor expansion](../../../../../taylor-expansion.md) of the [Lorentz factor](../../../../../lorentz-factor.md) at small $|\mathbf v|/c$ is

$$
\gamma=1+\frac{|\mathbf v|^2}{2c^2}+O(|\mathbf v|^4/c^4).
$$

Consequently $\mathbf p=m\mathbf v+O(m|\mathbf v|^3/c^2)$, recovering ordinary [momentum](../../../../../momentum.md). At rest the [four-momentum](../../../../../four-momentum.md) has energy $E_0=mc^2$, so subtracting this [rest energy](../../../../../rest-energy.md) gives the [kinetic energy](../../../../../kinetic-energy.md)

$$
\boxed{K=E-E_0=(\gamma-1)mc^2
=\frac12m|\mathbf v|^2+O(m|\mathbf v|^4/c^2)}.
$$

Thus the nonrelativistic limit preserves the rest-energy offset as well as the usual [kinetic energy](../../../../../kinetic-energy.md).

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
