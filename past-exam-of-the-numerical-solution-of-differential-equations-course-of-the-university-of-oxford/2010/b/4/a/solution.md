<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce $v=u'$ and solve the initial-value system

$$
u'=v,\qquad v'=p(x)v+q(x)u-f(x,u),\qquad u(0)=\alpha,\quad v(0)=s.
$$

The unknown initial slope $s$ is the [shooting method](../../../../../shooting-method.md) parameter. Integrate to one and solve the scalar residual equation $R(s)=u(1;s)-\beta=0$, using a secant iteration or a bracketed [root](../../../../../root-of-a-root-system.md) finder when suitable data are available.

For a Newton update, integrate the sensitivity equations along the current shot:

$$
w'=z,\qquad z'=p(x)z+[q(x)-f_u(x,u)]w,\qquad w(0)=0,\quad z(0)=1.
$$

Then $R'(s)=w(1)$ and the update is $s\leftarrow s-R(s)/w(1)$ when this derivative is nonzero. After a [root](../../../../../root-of-a-root-system.md) has been found, the corresponding shot satisfies both endpoint conditions. This formulation does not presume that a nonlinear boundary-value problem necessarily has a unique solution.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
