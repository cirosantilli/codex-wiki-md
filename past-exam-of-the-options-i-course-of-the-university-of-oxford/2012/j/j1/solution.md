<h1 id="j/j1/solution">Solution</h1>

↑ **Parent:** [J1](../j1.md)

The interior [time-independent Schrödinger equation](../../../../time-independent-schrodinger-equation.md) for a free particle is

$$
\boxed{-\frac{\hbar^2}{2m}(\psi_{xx}+\psi_{yy})=E\psi.}
$$

Confinement by the rectangular infinite well imposes [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md): $\psi=0$ at $x=0,b$ and $y=0,\sqrt5b$. The wave function is [square-integrable](../../../../square-integrable-function.md) and may be normalized to unit [probability](../../../../probability.md) on the rectangle.

Separation of variables gives products of the one-dimensional well states,

$$
\psi_{n,\ell}(x,y)=\frac{2}{5^{1/4}b}\sin\frac{n\pi x}{b}\sin\frac{\ell\pi y}{\sqrt5b},
\qquad n,\ell=1,2,\ldots.
$$

The Hamiltonian is the sum of the independent $x$ and $y$ kinetic-energy operators, so the one-dimensional energies add. Put $C=\pi^2\hbar^2/(2mb^2)$. Then

$$
E_{n,\ell}=C\left(n^2+\frac{\ell^2}{5}\right).
$$

For $n=1$, increasing $\ell$ gives $6C/5,9C/5,14C/5,21C/5$. The smallest energy with $n\geq2$ is also $21C/5$, attained at $(2,1)$; all $n\geq3$ give larger energies. Thus the ground and first three distinct excited energy levels are

$$
\boxed{\begin{array}{c|c|c}
\text{level}&E& (n,\ell)\\\hline
\text{ground}&6C/5&(1,1)\\
\text{first excited}&9C/5&(1,2)\\
\text{second excited}&14C/5&(1,3)\\
\text{third excited}&21C/5&(1,4),(2,1)
\end{array}}
$$

The largest listed energy therefore has [energy-level degeneracy](../../../../energy-level-degeneracy.md) $\boxed{2}$, since the two product eigenfunctions are linearly independent and no other pair solves $5n^2+\ell^2=21$.

## ↑ Ancestors (12)

1. [J1](../j1.md)
2. [J](../../j.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
