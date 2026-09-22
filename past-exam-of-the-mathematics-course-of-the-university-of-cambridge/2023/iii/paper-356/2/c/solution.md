<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A centered nearest-neighbour discretization of drift--diffusion is obtained from

$$
\boxed{k_i^+=\frac D{h^2}+\frac{v(x_i)}{2h},
\qquad
k_i^-=\frac D{h^2}-\frac{v(x_i)}{2h}.}
$$

For sufficiently small $h$ these rates are nonnegative. Taylor expansion of the mean equations gives

$$
\partial_tc=D\partial_x^2c-\partial_x(vc).
$$

Absorption into the target to the left of the first compartment gives

$$
\boxed{c(0,t)=0,}
$$

while the absence of outward jumps at the right endpoint gives the [zero-flux boundary condition](../../../../../../zero-flux-boundary-condition.md)

$$
\boxed{v(L)c(L,t)-D\partial_xc(L,t)=0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
