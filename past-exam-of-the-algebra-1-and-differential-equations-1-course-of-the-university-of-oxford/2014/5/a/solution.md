<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The **[maximum principle for subharmonic functions](../../../../maximum-principle-for-subharmonic-functions.md)** here states that if $u\in C^2(D)\cap C(\overline D)$ and $\Delta u=f\geq0$ in $D$, then

$$
\boxed{\max_{\overline D}u=\max_{\partial D}u.}
$$

If $f\leq0$, apply this to $-u$ to obtain the corresponding minimum principle. In particular a [harmonic function](../../../../harmonic-function.md) has both its maximum and minimum on the boundary. Without a sign condition on $f$, this conclusion need not hold.

First suppose $\Delta u>0$. By [compactness](../../../../compact-space.md) and continuity, $u$ attains a maximum on $\overline D$. At an interior maximum, the first derivatives vanish and the [Hessian matrix](../../../../hessian-matrix.md) is negative semidefinite. Its trace is then nonpositive, contradicting $\Delta u>0$. Thus a maximum lies on the boundary.

For the non-strict case put $u_\epsilon=u+\epsilon(x^2+y^2)$, with $\epsilon>0$. Then $\Delta u_\epsilon=f+4\epsilon>0$, so the strict case yields, for $z\in\overline D$,

$$
u(z)+\epsilon|z|^2\leq\max_{\partial D}(u+\epsilon)
=\max_{\partial D}u+\epsilon.
$$

Let $\epsilon\downarrow0$. This gives $u(z)\leq\max_{\partial D}u$, proving the theorem. The argument proves the weak maximum principle; it does not claim that every maximizer must be on the boundary when $u$ is constant.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
