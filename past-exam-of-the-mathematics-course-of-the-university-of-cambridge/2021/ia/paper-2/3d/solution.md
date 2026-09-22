<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

After $n$ tosses, the next total is even if either the current total is even and a tail occurs, or the current total is odd and a head occurs. Therefore

$$
q_{n+1}=(1-p)q_n+p(1-q_n)
=p+(1-2p)q_n.
$$

Since $q_0=1$, subtracting the fixed point $1/2$ gives

$$
q_{n+1}-\frac12
=(1-2p)\left(q_n-\frac12\right).
$$

Thus

$$
\boxed{
q_n=\frac{1+(1-2p)^n}{2}}.
$$

The formula also covers the endpoint cases $p=0$ and $p=1$.

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
