<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret strict ellipticity as uniform ellipticity up to the boundary, as required for the global [elliptic boundary value problem](../../../../../../elliptic-boundary-value-problem-split.md). Mere pointwise positive definiteness in the interior is insufficient: $L=x^2D^2$ on $(0,1)$ has trivial homogeneous Dirichlet kernel but $Lu=1$ has no $C^2$ solution up to $x=0$.

Set $X=\{u\in C^{2,\alpha}(\overline\Omega):u|_{\partial\Omega}=0\}$ and $Y=C^{0,\alpha}(\overline\Omega)$. The [Fredholm alternative for an elliptic Dirichlet problem](../../../../../../fredholm-alternative-for-an-elliptic-dirichlet-problem.md) says $L:X\to Y$ is a [Fredholm operator](../../../../../../fredholm-operator.md) of index zero. Its [null space](../../../../../../kernel-of-a-linear-map.md) $N$ is finite dimensional, its range is closed, and the range codimension equals $\dim N$. Hence $\boxed{N=\{0\}\iff L:X\to Y\text{ is invertible}}$; in this case every forcing has a unique solution.

Otherwise there are nonzero homogeneous solutions and finitely many compatibility conditions: $Lu=f$ is solvable exactly when $\ell(f)=0$ for every continuous linear functional on $Y$ vanishing on $L(X)$. When solvable, its solutions are $u_0+N$. This [Fredholm solvability condition](../../../../../../fredholm-solvability-condition.md) can be expressed with formal-adjoint null solutions for smoother coefficients. The functional formulation avoids differentiating the merely $C^{0,\alpha}$ coefficients.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
