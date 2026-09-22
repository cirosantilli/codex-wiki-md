<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Using $z=x+iy$, the energy is

$$
E=\frac12\int_{\mathbb R^2}
(|\partial_x\phi|^2+|\partial_y\phi|^2)\,dx\,dy.
$$

Because $|\phi|=1$, both derivatives are tangent to $S^2$ and $|\phi\times\partial_y\phi|=|\partial_y\phi|$. Completing the square gives

$$
E=\frac12\int|\partial_x\phi\mp\phi\times\partial_y\phi|^2\,dx\,dy
\left|\int\phi\mathbin\cdot
(\partial_x\phi\times\partial_y\phi)\,dx\,dy\right|.
$$

The final integral is $4\pi|\deg\phi|$ by the [topological degree](../../../../../../topological-degree.md) formula. Thus

$$
\boxed{E\geq4\pi|\deg\phi|},
\qquad
\boxed{c=4\pi}.
$$

Equality holds exactly when the appropriate first-order Bogomolny equation is satisfied:

$$
\boxed{\partial_x\phi=\pm\phi\times\partial_y\phi},
$$

with the sign chosen to match the degree.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 313](../../../paper-313-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
