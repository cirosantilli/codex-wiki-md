<h1 id="13c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the same indented upper-semicircle contour and [branch of the complex logarithm](../../../../../../branch-of-the-complex-logarithm.md), now for $F(z)=z^{1/2}\operatorname{Log}z/(1+z^2)$. Write $J=\int_0^\infty x^{1/2}\log x/(1+x^2)\,dx$. On the negative axis, $z^{1/2}=i|z|^{1/2}$ and $\operatorname{Log}z=\log|z|+i\pi$. Consequently the two straight contributions tend to

$$
(1+i)J-\pi I(1/2).
$$

The outer arc is $O(R^{-1/2}\log R)$ and the small arc is $O(\varepsilon^{3/2}(|\log\varepsilon|+1))$, so neither contributes in the limit. At the enclosed [pole](../../../../../../pole.md) $i$,

$$
\operatorname{Res}_{z=i}F=\frac{e^{i\pi/4}(i\pi/2)}{2i}=\frac\pi4e^{i\pi/4}.
$$

The [residue theorem](../../../../../../residue-theorem.md) gives $(1+i)J-\pi I(1/2)=i\pi^2e^{i\pi/4}/2$. Part (a) gives $I(1/2)=\pi/\sqrt2$. Substituting and using $e^{i\pi/4}=(1+i)/\sqrt2$, the right side after moving the $I$ term is $\pi^2(1+i)/(2\sqrt2)$. Hence

$$
\boxed{J=\frac{\pi^2}{2\sqrt2}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [13C](../../13c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
