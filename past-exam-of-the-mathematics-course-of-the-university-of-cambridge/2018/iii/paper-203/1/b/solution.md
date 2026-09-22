<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There is a small closure issue in the printed set: the [unit disc](../../../../../../unit-disc.md) is open, so its half-disc is not relatively closed in $\mathbb H$. As written, the set is not a [compact H-hull](../../../../../../compact-h-hull.md). We compute the intended [half-plane capacity](../../../../../../half-plane-capacity.md) after taking its relative closure in $\mathbb H$.

First remove the closed unit half-disc $K$. Its [mapping-out function of a compact H-hull](../../../../../../mapping-out-function-of-a-compact-h-hull.md) is the [Joukowski map](../../../../../../joukowski-map.md)

$$
g_K(z)=z+\frac1z,\qquad\operatorname{hcap}(K)=1.
$$

For $z=iy$ on the remaining portion of the vertical slit, $1<y\leq2$,

$$
g_K(iy)=i\left(y-\frac1y\right).
$$

Thus the image of the remaining slit is $(0,3i/2]$. By the [half-plane capacity of a vertical slit](../../../../../../half-plane-capacity-of-a-vertical-slit.md), its capacity is $(3/2)^2/2=9/8$. The [half-plane-capacity composition rule](../../../../../../half-plane-capacity-composition-rule.md) gives

$$
\boxed{\operatorname{hcap}(\overline A\cap\mathbb H)=1+\frac98=\frac{17}{8}.}
$$

As a direct check, composing with the slit map gives $g_A(z)=\sqrt{(z+z^{-1})^2+9/4}$, with the branch asymptotic to $z$. Its $z^{-1}$ coefficient is $17/8$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
