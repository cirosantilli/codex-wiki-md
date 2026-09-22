<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $0<\alpha<1$, an [averaged operator](../../../../../../averaged-operator.md) has the form

$$
\boxed{T=(1-\alpha)I+\alpha R}
$$

for some [nonexpansive mapping](../../../../../../nonexpansive-mapping.md) $R$, meaning $\|Rz-Rw\|_2\leq\|z-w\|_2$ for all $z,w$. The word averaging refers to a [convex combination](../../../../../../convex-combination.md) with the identity. It does not mean averaging function values over a neighborhood.

An equivalent and useful [averaged-operator inequality](../../../../../../averaged-operator-inequality.md) is

$$
\boxed{\|Tz-Tw\|_2^2\leq\|z-w\|_2^2-\frac{1-\alpha}{\alpha}\|(I-T)z-(I-T)w\|_2^2}.
$$

To see it, put $d=z-w$ and $r=Rz-Rw$ and expand

$$
\|(1-\alpha)d+\alpha r\|_2^2
=(1-\alpha)\|d\|_2^2+\alpha\|r\|_2^2-\alpha(1-\alpha)\|d-r\|_2^2.
$$

Use $\|r\|_2\leq\|d\|_2$ and $(I-T)z-(I-T)w=\alpha(d-r)$. Conversely, substituting $R=[T-(1-\alpha)I]/\alpha$ into the same expansion proves its [nonexpansiveness](../../../../../../nonexpansive-mapping.md) from the displayed inequality. The strict range $0<\alpha<1$ matters for convergence of unrelaxed iterations: a general [nonexpansive mapping](../../../../../../nonexpansive-mapping.md) such as $T=-I$ can have nonconvergent alternating iterates.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
