<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

The second [equilibrium point](../../../equilibrium-point-of-a-dynamical-system.md) equation gives $y=-(x+1)/2$. Substituting into the first gives $x+e^{(x-1)/2}=0$, so $x<0$. Put $x=-a$, with $a>0$. Then

$$
a=e^{-(a+1)/2}
\iff ae^{(a+1)/2}=1,\qquad y=(a-1)/2.
$$

The function $h(a)=ae^{(a+1)/2}$ is strictly increasing on $a\geq0$, since $h'(a)=e^{(a+1)/2}(1+a/2)>0$. It starts at zero and tends to infinity, so it takes the value one exactly once. Moreover $h(1)=e>1$, so $0<a<1$. This proves uniqueness of the stated [equilibrium point](../../../equilibrium-point-of-a-dynamical-system.md).

At that point $e^{x+y}=a$, and the [Jacobian matrix](../../../jacobian-matrix.md) is

$$
J=\begin{pmatrix}1+a&a\\1&2\end{pmatrix}.
$$

Its trace is $3+a$ and determinant $2+a$. The characteristic discriminant is $(3+a)^2-4(2+a)=(a+1)^2$, so its two [eigenvalues](../../../eigenvalue.md) are

$$
\boxed{\lambda_1=1,\qquad\lambda_2=2+a.}
$$

They are distinct and positive, with [eigenvectors](../../../eigenvector.md) $(1,-1)$ and $(a,1)$ respectively. Thus **the linearized [critical point](../../../critical-point.md) is an [unstable node](../../../unstable-node.md)**. It is a [hyperbolic equilibrium](../../../hyperbolic-equilibrium-point.md), so the original nonlinear [equilibrium point](../../../equilibrium-point-of-a-dynamical-system.md) is also locally repelling; this last observation is stronger than the requested linearized classification.

## ↑ Ancestors (11)

1. [9](../9.md)
2. [2007](../../2007-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
