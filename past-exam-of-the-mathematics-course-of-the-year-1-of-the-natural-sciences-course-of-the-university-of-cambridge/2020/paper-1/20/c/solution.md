<h1 id="20/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The three components of the [curl](../../../../../curl.md) cancel pairwise:

$$
\nabla\times\mathbf F=(1-1,1-1,1-1)=\mathbf0.
$$

The domain is all of $\mathbb R^3$, which is [simply connected](../../../../../simply-connected-space.md), so this is consistent with a [conservative vector field](../../../../../conservative-vector-field.md). To construct its [scalar potential](../../../../../scalar-potential.md), integrate $\Phi_x=y+z$ to obtain $\Phi=x(y+z)+h(y,z)$. Matching $\Phi_y=x+z$ gives $h_y=z$, hence $h=yz+k(z)$. Finally $\Phi_z=x+y$ forces $k'(z)=0$. Consequently

$$
\boxed{\Phi(x,y,z)=xy+xz+yz+C,\qquad\mathbf F=\nabla\Phi.}
$$

Every [scalar potential](../../../../../scalar-potential.md) differs by a constant on this connected domain. The endpoint values differ by one, agreeing with the [line integral](../../../../../line-integral.md) in part (a).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
