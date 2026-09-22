<h1 id="11f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $v_I,v_J,v_K$ be the vertices opposite the corresponding sides, and let $\lambda_I,\lambda_J,\lambda_K$ be their barycentric coordinates. We prove the equivalence by negating each assertion.

Suppose the closed covering sets have empty triple intersection. For $x\in T$ put $d_I(x)=\operatorname{dist}(x,A)$, and define $d_J,d_K$ similarly. At least one distance is positive, since $x$ cannot belong to all three sets, and at least one is zero, since they cover $T$. Consequently

$$
f(x)=\frac{d_I(x)v_I+d_J(x)v_J+d_K(x)v_K}{d_I(x)+d_J(x)+d_K(x)}
$$

is continuous and lies in the boundary: one barycentric coordinate vanishes. On $I$ its first coefficient is zero because $I\subseteq A$, so $f(I)\subseteq I$, and likewise for the other sides. This contradicts assertion (1), proving (1) implies (2).

Conversely, suppose such a boundary-valued map exists. Define closed subsets of $\mathbb R^2$ by

$$
A=\{x\in T:\lambda_I(f(x))=0\},\quad B=\{x\in T:\lambda_J(f(x))=0\},\quad C=\{x\in T:\lambda_K(f(x))=0\}.
$$

They are closed because $T$ is [compact](../../../../../../compact-space.md) and the coordinate functions are continuous. They cover $T$ because $f$ is boundary-valued; the side-preserving condition gives $I\subseteq A$, $J\subseteq B$, $K\subseteq C$. Their triple intersection is empty because barycentric coordinates sum to one. Thus failure of (1) implies failure of (2), completing the equivalence.

In fact both assertions hold. If the map in (1) existed, let $R$ rotate the equilateral triangle through $120^\circ$. [Brouwer fixed-point theorem](../../../../../../brouwer-fixed-point-theorem.md) applied to $R\circ f:T\to T$ gives a [fixed point](../../../../../../fixed-point.md) $x$ on the boundary. On any side $I$ containing $x$, side preservation puts $x$ also on $R(I)$, so it is their common vertex. A side-preserving map fixes every vertex because that vertex lies on two sides. Therefore $x=Rf(x)=Rx$, impossible for a noncentral vertex. This also proves the covering-intersection assertion through the established equivalence.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
