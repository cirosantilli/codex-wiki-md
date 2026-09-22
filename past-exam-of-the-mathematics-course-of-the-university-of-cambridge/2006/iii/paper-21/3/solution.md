<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\xi$ have real rank $r$, choose a bundle metric, and write $D(\xi),S(\xi)$ for its disk and sphere bundles. In a [multiplicative generalized cohomology theory](../../../../../multiplicative-generalized-cohomology-theory.md), a [Thom class in a generalized cohomology theory](../../../../../thom-class-in-a-generalized-cohomology-theory.md) is a class

$$
u_h(\xi)\in h^r(D(\xi),S(\xi))
$$

whose restriction to each fiber pair $(D^r,S^{r-1})$ is the suspension of the coefficient unit $1\in h^0(\mathrm{pt})$ under the chosen oriented identification. Equivalently, it is a fiberwise generator over the coefficient ring compatible with the $h$-orientation. [Cup product](../../../../../cup-product.md) with this class gives the [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md)

$$
h^k(X)\longrightarrow h^{k+r}(D(\xi),S(\xi)),\qquad
a\longmapsto\pi^*a\smile u_h(\xi),
$$

where $X$ is the base.

Let $z:X\to D(\xi)$ be the [zero section](../../../../../zero-section-of-a-vector-bundle.md) and let $\jmath:h^r(D(\xi),S(\xi))\to h^r(D(\xi))$ forget relative supports. The [Euler class in a generalized cohomology theory](../../../../../euler-class-in-a-generalized-cohomology-theory.md) is

$$
\boxed{e_h(\xi)=z^*\jmath(u_h(\xi))\in h^r(X).}
$$

Equivalently, identify relative cohomology with [reduced cohomology](../../../../../reduced-cohomology.md) of the [Thom space](../../../../../thom-space.md) and pull its [Thom class](../../../../../thom-class.md) back along the [zero section](../../../../../zero-section-of-a-vector-bundle.md) followed by the quotient map.

Suppose $s$ is a nowhere-zero section. Normalize it to $\widehat s(x)=s(x)/\|s(x)\|\in S(\xi)_x$. The maps

$$
H_t(x)=t\widehat s(x),\qquad 0\leq t\leq1,
$$

give a [homotopy](../../../../../homotopy.md) within $D(\xi)$ from $z$ to the sphere-valued section $\widehat s$. The image $\jmath(u_h(\xi))$ restricts to zero on $S(\xi)$, by the exact sequence of the pair. [Homotopy](../../../../../homotopy.md) invariance therefore yields

$$
z^*\jmath(u_h(\xi))
=\widehat s^{\,*}\jmath(u_h(\xi))=0.
$$

Thus [a nowhere-zero section annihilates generalized Euler classes](../../../../../a-nowhere-zero-section-annihilates-generalized-euler-classes.md):

$$
\boxed{e_h(\xi)=0.}
$$

The argument uses the actual nowhere-zero section and is valid for any chosen Thom orientation in the multiplicative theory.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
