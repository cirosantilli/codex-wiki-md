<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

First extract the [polynomial content](../../../polynomial-content.md) from $f$:

$$
\boxed{f(X)=2\bigl(X^4-2X^3+4X^2-2X+2\bigr).}
$$

The primitive quartic is [Eisenstein](../../../eisenstein-criterion.md) at the prime $2$: every nonleading coefficient is divisible by $2$, while the constant term is not divisible by $4$. [Eisenstein's criterion](../../../eisenstein-criterion.md) makes it irreducible over $\mathbb Q$, and [Gauss's lemma](../../../gauss-s-lemma-riemannian-geometry.md) makes it irreducible in $\mathbb Z[X]$. The constant factor $2$ is itself irreducible in $\mathbb Z[X]$.

The polynomial $g$ is already irreducible over $\mathbb Q$: it is [Eisenstein](../../../eisenstein-criterion.md) at $3$. Its nonleading coefficients, including the missing zero coefficients, are divisible by $3$, and $-21$ is not divisible by $9$. Thus **$g$ is its own sole nonconstant irreducible factor** over $\mathbb Q$.

Over the field $\mathbb Z_3$, grouping terms gives

$$
\boxed{h(X)=X(X+2)(X^2+1).}
$$

The first two factors are linear and therefore irreducible. The quadratic takes the values $1,2,2$ at $0,1,2$ respectively, so it has no root in $\mathbb Z_3$. A degree-two polynomial over a field is reducible exactly when it has a root, proving its irreducibility.

All three factorizations are **unique up to order and multiplication by units**. The ring $\mathbb Z$ is a [unique factorization domain](../../../unique-factorization-domain.md), hence so is $\mathbb Z[X]$ by [Gauss's lemma](../../../gauss-s-lemma-riemannian-geometry.md). A polynomial ring over a field is a [Euclidean domain](../../../euclidean-domain.md), so both $\mathbb Q[X]$ and $\mathbb Z_3[X]$ have unique factorization. The units are $\pm1$ in the first ring, nonzero rational constants in the second, and $1,2$ in the third.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2010](../../2010-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
