<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

By transitivity, choose $h\in G$ with $hy=x$. If $gy=y$, then

$$
(hgh^{-1})x=hgy=hy=x.
$$

Thus $hgh^{-1}\in B$. This proves the conjugation assertion directly from the [transitive group action](../../../../../transitive-group-action.md).

For the [complex special linear group in dimension two](../../../../../complex-special-linear-group-in-dimension-two.md), the [Möbius transformation](../../../../../mobius-transformation.md) of a matrix $g$ acts by $z\mapsto(az+b)/(cz+d)$, with $ad-bc=1$. It fixes infinity exactly when $c=0$, so its [stabilizer subgroup](../../../../../stabilizer-subgroup.md) is

$$
\boxed{B=\left\{\begin{pmatrix}a&b\\0&a^{-1}\end{pmatrix}:a\in\mathbb C^\times,\ b\in\mathbb C\right\}.}
$$

We distinguish the cases to avoid dividing by a vanishing coefficient.

If $c\ne0$, infinity is not fixed, and the finite fixed points solve

$$
cz^2+(d-a)z-b=0.
$$

Neither root is the pole $-d/c$: substituting that value gives $(ad-bc)/c=1/c\ne0$. The fixed-point set is therefore

$$
\boxed{\left\{\frac{a-d+\sqrt{(a+d)^2-4}}{2c},\ \frac{a-d-\sqrt{(a+d)^2-4}}{2c}\right\},}
$$

with the two entries coinciding when the discriminant is zero. The discriminant identity uses $(a-d)^2+4bc=(a+d)^2-4$.

If $c=0$ and $a\ne d$, the fixed points are $\{\infty,b/(d-a)\}$. If $c=0$, $a=d$ and $b\ne0$, only infinity is fixed. If $c=0$, $a=d$ and $b=0$, the determinant condition gives $g=\pm I$ and every point is fixed. Both central matrices induce the identity Möbius transformation.

Every case has a fixed point, because a quadratic over the complex numbers has a root. The action is transitive: any finite $z_0$ is sent to infinity by

$$
h=\begin{pmatrix}0&-1\\1&-z_0\end{pmatrix}\in SL_2(\mathbb C),
$$

and infinity already needs no change. Applying the first argument to a fixed point proves **every element of $SL_2(\mathbb C)$ is conjugate to an element of $B$**.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
