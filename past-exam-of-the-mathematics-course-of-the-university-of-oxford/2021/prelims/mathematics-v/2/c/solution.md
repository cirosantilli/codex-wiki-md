<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If two solutions exist, their difference $w$ satisfies $\nabla^2w-w=0$ inside $B$ and $w=0$ on the boundary. Suppose $w$ has a positive value. [Continuity](../../../../../../continuous-function.md) on the closed ball gives a positive [maximum](../../../../../../maximum-of-a-subset-of-a-total-order.md) at an interior point, where the [Hessian matrix](../../../../../../hessian-matrix.md) is negative semidefinite and hence $\nabla^2w\leq0$. But the equation gives $\nabla^2w=w>0$, a contradiction. A negative [minimum](../../../../../../minimum-of-a-subset-of-a-total-order.md) similarly contradicts $\nabla^2w=w<0$.

Thus $\boxed{w=0}$, proving uniqueness by the [maximum principle for the modified Helmholtz equation](../../../../../../maximum-principle-for-the-modified-helmholtz-equation.md). Here a classical solution is understood to be $C^2$ inside and continuous up to the boundary; mere first differentiability would not define the displayed [Laplacian](../../../../../../laplacian.md) classically. With enough boundary regularity, the alternative [Green's first identity](../../../../../../green-s-first-identity.md) proof is $0=\int_Bw(\nabla^2w-w)=-\int_B(|\nabla w|^2+w^2)$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
