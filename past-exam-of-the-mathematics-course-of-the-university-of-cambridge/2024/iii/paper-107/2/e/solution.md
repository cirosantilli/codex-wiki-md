<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $h=\log X$. The first equation becomes

$$
\Delta h=\frac{\Delta X}{X}-\frac{|\nabla X|^2}{X^2}
=-\frac{|\nabla Y|^2}{X^2},
$$

while the second remains

$$
\operatorname{div}(X^{-2}\nabla Y)=0.
$$

The assumed $C^{0,\alpha}$ regularity and the bounds away from zero make $X^{-2}$ a $C^{0,\alpha}$ uniformly elliptic coefficient. The divergence-form $C^{1,\alpha}$ estimate from part (d) first gives $Y\in C^{1,\alpha}_{\mathrm{loc}}$. Hence the right side of the equation for $h$ is $C^{0,\alpha}$, and the [interior Schauder estimate](../../../../../../interior-schauder-estimate.md) gives $h$, and therefore $X$, in $C^{2,\alpha}_{\mathrm{loc}}$.

Expanding the $Y$ equation gives

$$
\Delta Y-2\nabla h\cdot\nabla Y=0.
$$

The higher-order Schauder estimates now alternate between the equations for $h$ and $Y$, gaining derivatives at each step. Induction yields $(X,Y)\in C^\infty(\Omega';H)$ for every $\Omega'\Subset\Omega$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
