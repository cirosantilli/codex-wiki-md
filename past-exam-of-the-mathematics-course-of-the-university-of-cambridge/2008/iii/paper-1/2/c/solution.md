<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The comparison triangle must have third side $d(x,y)$: the printed $d(y,z)$ contains an undefined $z$. Use $A=d(a,x)$, $B=d(a,y)$ and $C=d(x,y)$.

First extend the midpoint inequality along any constant-speed [geodesic](../../../../../../geodesic.md) $\gamma$ from $p$ to $q$. If $L=d(p,q)$, the function $d(z,\gamma(t))^2-L^2t^2$ is midpoint-convex by (a). Iteration proves its convexity bound for dyadic $t$, and [continuity](../../../../../../continuous-function.md) then gives the [Hadamard squared-distance inequality](../../../../../../hadamard-squared-distance-inequality.md)

$$
d(z,\gamma(t))^2\leq(1-t)d(z,p)^2+td(z,q)^2-t(1-t)L^2.
$$

Apply this first to $[a,x]$ with $z=y_t$, and then to $[a,y]$ with $z=x$:

$$
d(x_s,y_t)^2\leq(1-s)t^2B^2+s\bigl[(1-t)A^2+tC^2-t(1-t)B^2\bigr]
-s(1-s)A^2.
$$

Simplification gives

$$
\boxed{d(x_s,y_t)^2\leq s^2A^2+t^2B^2-st(A^2+B^2-C^2).}
$$

In a Euclidean comparison triangle, the cosine rule gives the scalar product of the two [vectors](../../../../../../vector.md) from the common vertex as $(A^2+B^2-C^2)/2$. The squared distance between their multiples $s$ and $t$ is exactly the right side displayed above. Taking nonnegative square roots proves the required triangle comparison, including degenerate Euclidean triangles.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
