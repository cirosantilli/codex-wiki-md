<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For the negative-sign equation, take a nonzero separated solution $\phi=X(x)Y(y)$. [Separation of variables](../../../../separation-of-variables.md) gives $X''=-\mu X$ and $Y''=-(25-\mu)Y$. The zero [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) on $X$ force $\mu=m^2$ with a positive integer $m$ and $X=\sin mx$, up to a constant. Zero boundary values on $Y$ similarly require $25-m^2=n^2$ with a positive integer $n$. A zero or negative separation eigenvalue would give linear or hyperbolic factors, whose two zero endpoint values force the trivial solution.

The only positive integer pairs with $m^2+n^2=25$ are $(3,4)$ and $(4,3)$. By the complete [Dirichlet eigensystem of a rectangle](../../../../dirichlet-eigensystem-of-a-rectangle.md), these span the whole eigenspace, so

$$
\boxed{\phi(x,y)=A\sin3x\sin4y+B\sin4x\sin3y,\qquad A,B\in\mathbb R.}
$$

For the positive-sign equation there is **only the zero solution**. One can use the same strictly positive eigenvalues of $-\Delta$, or directly apply the [zero Dirichlet solution of the modified Helmholtz equation](../../../../zero-dirichlet-solution-of-the-modified-helmholtz-equation.md). Multiplying by $\phi$ and using [Green's first identity](../../../../green-s-first-identity.md) gives

$$
25\int_\Omega\phi^2\,dx\,dy=\int_\Omega\phi\Delta\phi\,dx\,dy=-\int_\Omega|\nabla\phi|^2\,dx\,dy,
$$

where $\Omega=(0,\pi)^2$. Both nonnegative integrals must vanish, proving $\boxed{\phi=0}$.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [2004](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
