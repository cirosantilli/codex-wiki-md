<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $p$ be the midpoint of a geodesic $[y_1,y_2]\subseteq Y$ and put $L=d(y_1,y_2)$. Apply the [geodesic quadrilateral in a hyperbolic metric space](../../../../../../geodesic-quadrilateral-in-a-hyperbolic-metric-space.md) bound to the quadrilateral with consecutive vertices $y_1,z_1,z_2,y_2$. The point $p$ is within $2\delta$ of one of the other three sides. It cannot be within $2\delta$ of $[z_1,z_2]\subseteq Z$, because every point of $Y$ has distance greater than $2\delta$ from every point of $Z$.

By symmetry there is therefore a point $q\in[y_1,z_1]$ with $d(p,q)\le2\delta$. The [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
d(y_1,q)\ge d(y_1,p)-d(p,q)\ge L/2-2\delta
$$

and hence

$$
d(z_1,p)
\le d(z_1,q)+2\delta
=d(z_1,y_1)-d(y_1,q)+2\delta
\le d(z_1,y_1)-L/2+4\delta.
$$

Since $p\in Y$ and $y_1$ is a closest point of $Y$ to $z_1$, we also have $d(z_1,y_1)\le d(z_1,p)$. Therefore $L\le8\delta$, as required.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
