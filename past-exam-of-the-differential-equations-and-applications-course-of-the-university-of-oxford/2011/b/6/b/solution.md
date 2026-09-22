<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $F(p,q)=p^2+pq-1$. Parametrize the initial line by $x_0=s>0$, $y_0=0$, $u_0=2s^2$. Initial compatibility gives $p=4s$, and $F=0$ then gives $q=1/(4s)-4s$. The characteristic formula in part (a) yields

$$
\boxed{x=s+\tau\left(4s+\frac1{4s}\right),\quad y=4s\tau,\quad u=2s^2+2\tau,\qquad s>0.}
$$

Since $y>0$, take $\tau>0$. To select the branch connected smoothly to the initial data, stop each characteristic before its coordinate map folds. Its [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
J=4s-\frac{2\tau}{s},
$$

so this branch has $0<\tau<2s^2$. Eliminating $\tau=y/(4s)$ gives

$$
x-y=s+\frac{y}{16s^2},\qquad u=2s^2+\frac{y}{2s},\qquad s>\frac12y^{1/3}.
$$

For fixed $y>0$, the right side defining $x-y$ is strictly increasing on that selected branch. At its lower endpoint it equals $3y^{1/3}/4$, and it tends to infinity as $s\to\infty$. Thus it gives exactly one $s$ for every point in

$$
\boxed{y>0,\qquad x>y+\frac34y^{1/3}.}
$$

Substituting that unique $s$ into the formula for $u$ gives the required classical solution. As $y\downarrow0$ at fixed $x>0$, $s\to x$, and $u\to2x^2$ as required.

Without the pre-fold branch restriction, the algebraic equation also has a smaller positive root. That root tends to zero as $y\downarrow0$, and its $u$ tends to zero rather than $2x^2$, so it does not solve the prescribed initial-boundary problem. The fold $J=0$ is the [characteristic caustic](../../../../../characteristic-caustic.md); uniqueness here is for the classical branch continued from the given initial data before that fold.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
