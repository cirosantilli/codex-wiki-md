<h1 id="j/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The integral [Gauss's law](../../../../gauss-s-law.md) is

$$
\int_{\partial V}\mathbf E\cdot\mathbf n\,dS
=\frac{Q(V)}{\epsilon_0}
=\frac1{\epsilon_0}\int_V\rho\,dV.
$$

The [divergence theorem](../../../../divergence-theorem.md) makes the left side $\int_V\nabla\cdot\mathbf E\,dV$. If the differential relation $\nabla\cdot\mathbf E=\rho/\epsilon_0$ holds, this proves the integral law. Conversely, if the integral identity holds for every suitable volume and the fields are sufficiently regular, a nonzero value of $\nabla\cdot\mathbf E-\rho/\epsilon_0$ would persist in sign on a small neighborhood and contradict its zero integral. The differential law follows.

For a sphere of radius $r$, spherical symmetry makes the flux $4\pi r^2E(r)$ and the enclosed charge $4\pi\int_0^rs^2\rho(s)\,ds$. Hence

$$
\boxed{E(r)=\frac1{\epsilon_0r^2}\int_0^rs^2\rho(s)\,ds.}
$$

There is no extra point charge at the origin in the stipulated density distribution. Outside the charge support,

$$
Q=4\pi\int_0^as^2\rho(s)\,ds,\qquad
\boxed{E(r)=\frac{Q}{4\pi\epsilon_0r^2}\quad(r>a).}
$$

## ↑ Ancestors (12)

1. [1](../1.md)
2. [J](../../j.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
