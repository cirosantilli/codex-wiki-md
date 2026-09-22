<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For the real lattice version of the [Stone-Weierstrass theorem](../../../../stone-weierstrass-theorem.md), let $f\in C_{\mathbb R}(\Omega)$ and $\varepsilon>0$. For any $x,y\in\Omega$, separation of points and constants give $h_{xy}\in L$ matching $f$ at both $x$ and $y$: take an affine combination of a separating function, and for $x=y$ take a constant. Fix $x$. The open sets where $h_{xy}>f-\varepsilon$ cover $\Omega$ as $y$ varies. Compactness gives finitely many such functions; their maximum $g_x$ belongs to the lattice $L$, satisfies $g_x>f-\varepsilon$ everywhere, and has $g_x(x)=f(x)$. The open sets where $g_x<f+\varepsilon$ now cover $\Omega$ as $x$ varies. Choose finitely many and take their minimum $h\in L$. Then $f-\varepsilon<h<f+\varepsilon$ everywhere. Thus **$L$ is uniformly dense** in the real continuous functions.

For the complex \*-algebra, its real subalgebra $A_{\mathbb R}$ of [Hermitian C-star elements](../../../../hermitian-element-of-a-c-star-algebra.md) contains the real and imaginary parts of every member. It separates points, because at least one of those parts distinguishes any pair distinguished by a complex function. Its uniform [closure](../../../../closure-topology.md) is a unital real subalgebra and is a lattice by the allowed result. The real theorem makes this [closure](../../../../closure-topology.md) all of $C_{\mathbb R}(\Omega)$. Approximating the real and imaginary parts separately proves **$A$ is uniformly dense in $C(\Omega)$**.

On $[0,1]$, the algebra of polynomials in $t^2$ is unital, closed under conjugation, and separates points because $t\mapsto t^2$ is injective there. Choose $p(t^2)$ within $\varepsilon/3$ of $a(t)$, and correct its endpoints by

$$
b(t)=p(t^2)+[a(0)-p(0)](1-t^2)+[a(1)-p(1)]t^2.
$$

This is still a [polynomial](../../../../polynomial-split.md) in $t^2$ and has exactly the requested endpoint values. The correction has absolute value at most $\varepsilon/3$, because it is a [convex combination](../../../../convex-combination.md) of two errors of that size. Therefore

$$
\boxed{b(0)=a(0),\quad b(1)=a(1),\quad\|a-b\|_\infty<2\varepsilon/3<\varepsilon.}
$$

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
