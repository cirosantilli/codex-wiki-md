<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Here [subvariety](../../../../closed-subvariety.md) means a closed affine [subvariety](../../../../closed-subvariety.md). Suppose first that $F^\#$ is onto, and write $X\subseteq\mathbb A^n$, $Y\subseteq\mathbb A^m$. Put $J=\ker F^\#$ and $Z=V_Y(J)$. Choose $g_i\in A(Y)$ with $F^\#g_i=x_i|_X$ and let $G:Z\to\mathbb A^n$ have components $g_i|_Z$.

If $h\in I(X)$, then $F^\#(h(g_1,\ldots,g_n))=h|_X=0$, so $h(g_1,\ldots,g_n)\in J$. It vanishes on $Z$, proving $G(Z)\subseteq X$. The chosen lifts give $G\circ F=\operatorname{id}_X$, and $F(X)\subseteq Z$ by the definition of $J$.

Let the components of $F$ be [polynomial functions](../../../../polynomial-function.md) $f_1,\ldots,f_m$ on $X$. For each target coordinate $y_j$, the element $y_j-f_j(g_1,\ldots,g_n)$ has zero [pullback](../../../../pullback-category-theory.md), hence belongs to $J$. It vanishes on $Z$, giving $F\circ G=\operatorname{id}_Z$. Both maps have [polynomial](../../../../polynomial-split.md) components, so $F$ is an [isomorphism](../../../../isomorphism.md) onto the [closed subvariety](../../../../closed-subvariety.md) $Z$.

Conversely, if $F:X\to Z\subseteq Y$ is an [isomorphism](../../../../isomorphism.md) onto a [closed subvariety](../../../../closed-subvariety.md), [restriction](../../../../restriction-mathematics.md) $A(Y)\to A(Z)$ is [surjective](../../../../surjective-function.md), and the [pullback](../../../../pullback-category-theory.md) $A(Z)\to A(X)$ of that [isomorphism](../../../../isomorphism.md) is an [isomorphism](../../../../isomorphism.md). Their composition is $F^\#$, proving

$$
\boxed{F^\#\text{ onto}\iff F\text{ is a closed embedding}.}
$$

The word closed matters: an [isomorphism](../../../../isomorphism.md) onto a merely locally [closed subset](../../../../closed-set.md) need not induce a [surjective](../../../../surjective-function.md) coordinate-ring map. For example $\mathbb G_m\hookrightarrow\mathbb A^1$ induces $k[t]\hookrightarrow k[t,t^{-1}]$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebraic Geometry course of the University of Oxford](../../../split.md)
5. [Algebraic Geometry course of the University of Oxford](../../../../algebraic-geometry-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
