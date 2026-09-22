<h1 id="s1/1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the positive orientation shown in the source: the upper bank runs outwards and the lower bank returns towards one. On those banks the [logarithm branch](../../../../../branch-of-the-complex-logarithm.md) has values $\ell-i\pi$ and $\ell+i\pi$, respectively, with $\ell=\log(x-1)$. Their squared difference is $-4i\pi\ell$. The [residue theorem](../../../../../residue-theorem.md) therefore gives

$$
2\pi i=\lim\oint_\Gamma\frac{L(z)^2}{z^3}\,dz=-4\pi i\int_1^\infty\frac{\log(x-1)}{x^3}\,dx,
$$

and hence

$$
\boxed{\int_1^\infty\frac{\log(x-1)}{x^3}\,dx=-\frac12.}
$$

The large-circle contribution is $O(R^{-2}\log^2R)$ and the small circle about one contributes $O(\varepsilon|\log\varepsilon|^2)$, both tending to zero. These estimates justify replacing the closed [contour integral](../../../../../contour-integral.md) by its two cut-bank [integrals](../../../../../integral-split.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [1](../../1.md)
3. [S1](../../../s1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
