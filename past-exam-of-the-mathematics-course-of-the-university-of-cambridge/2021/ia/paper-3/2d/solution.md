<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

Elements $g,h\in G$ are conjugate when

$$
h=xgx^{-1}
$$

for some $x\in G$. Then

$$
h^n=xg^nx^{-1}
$$

for every integer $n$, so $h^n=e$ exactly when $g^n=e$. They therefore have the same [order](../../../../../order-of-a-group-element.md).

The Möbius group consists of the [Möbius transformations](../../../../../mobius-transformation.md)

$$
z\longmapsto\frac{az+b}{cz+d},
\qquad ad-bc\ne0,
$$

of the Riemann sphere, under composition. If $h=xgx^{-1}$, then

$$
h(x(p))=x(g(p)).
$$

Thus $p$ is fixed by $g$ exactly when $x(p)$ is fixed by $h$. Conjugation gives a bijection between their fixed-point sets, so conjugate elements have the same number of fixed points.

A nonidentity Möbius transformation has at most two fixed points because its fixed-point equation is quadratic on the Riemann sphere. If it has only one repeated fixed point, conjugate that point to infinity; the transformation becomes a nontrivial translation $z\mapsto z+c$, which has infinite order. Consequently every nontrivial finite-order element has two distinct fixed points:

$$
\boxed{|\operatorname{Fix}(g)|=2}.
$$

This is [fixed points of a finite-order Möbius transformation](../../../../../fixed-points-of-a-finite-order-mobius-transformation.md).

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
