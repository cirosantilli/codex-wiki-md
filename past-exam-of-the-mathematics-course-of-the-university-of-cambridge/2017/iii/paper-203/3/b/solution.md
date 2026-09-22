<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the [domains](../../../../../../domain-mathematical-analysis.md) are proper, so $d$ and $\widetilde d$ are finite and positive, and interpret the [conformal transformation](../../../../../../conformal-map.md) as a bijection. Apply the [Koebe quarter theorem](../../../../../../koebe-quarter-theorem.md) to

$$
F(w)=\frac{f(z+dw)-f(z)}{d f'(z)},\qquad |w|<1.
$$

The [open ball](../../../../../../open-ball.md) $B(z,d)$ lies in $D$, so $F$ is a normalized [univalent function](../../../../../../univalent-function.md). Its image inclusion shows that $B(\widetilde z,d|f'(z)|/4)\subseteq\widetilde D$. Therefore $d|f'(z)|/4\leq\widetilde d$, or $|f'(z)|\leq4\widetilde d/d$.

Apply the same argument to the inverse [conformal map](../../../../../../conformal-map.md), whose [derivative](../../../../../../derivative.md) at $\widetilde z$ is $1/f'(z)$. It gives $\widetilde d/(4|f'(z)|)\leq d$. Thus the [boundary-distance derivative bound for a conformal bijection](../../../../../../boundary-distance-derivative-bound-for-a-conformal-bijection.md) is

$$
\boxed{\frac{\widetilde d}{4d}\leq|f'(z)|\leq\frac{4\widetilde d}{d}.}
$$

The full [domains](../../../../../../domain-mathematical-analysis.md) need not be [simply connected domains](../../../../../../simply-connected-domain.md): only the two [interior](../../../../../../interior-topology.md) discs are used. If the whole plane is allowed as a [domain](../../../../../../domain-mathematical-analysis.md), a [conformal bijection](../../../../../../biholomorphism.md) onto another plane [domain](../../../../../../domain-mathematical-analysis.md) is affine and both [domains](../../../../../../domain-mathematical-analysis.md) are the whole plane. For example, $D=\widetilde D=\mathbb C$ and $f(z)=z$ make both [boundary](../../../../../../boundary-of-a-set.md) distances infinite and the printed ratios $\infty/\infty$ undefined. This is a necessary proper-domain convention. Bijectivity also matters: the injective [conformal map](../../../../../../conformal-map.md) $f(w)=w/8$ from the [unit disc](../../../../../../unit-disc.md) into itself has $d=\widetilde d=1$ at zero but $|f'(0)|=1/8<1/4$. Thus an interpretation allowing a map into, rather than onto, the second [domain](../../../../../../domain-mathematical-analysis.md) makes the lower bound false.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
