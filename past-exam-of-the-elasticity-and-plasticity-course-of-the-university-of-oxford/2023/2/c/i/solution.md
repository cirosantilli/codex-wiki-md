<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With zero [tension](../../../../../tension.md) and zero distributed load, a free interval satisfies $w''''=0$. Before contact the entire [elastic beam](../../../../../elastic-beam.md) is free, so $w$ is a cubic [polynomial](../../../../../polynomial-split.md). The four end [boundary conditions](../../../../../boundary-condition.md) determine it uniquely. Reflection $x\mapsto-x$ preserves those [boundary conditions](../../../../../boundary-condition.md), so the unique solution is an [even function](../../../../../even-function.md) and its odd terms vanish. Direct substitution gives

$$
\boxed{w(x)=\frac{\alpha}{2L}(x^2-L^2).}
$$

For $\alpha\geq0$, its minimum occurs at $x=0$ and is $-\alpha L/2$. The constraint $w\geq-H$ is therefore satisfied exactly when $\alpha\leq2H/L$. The first contact is at the midpoint:

$$
\boxed{\alpha_{\mathrm{first}}=\frac{2H}{L}.}
$$

At equality the [normal contact force](../../../../../normal-contact-force.md) is still zero. The uniqueness used here can also be checked by integrating $v''''v$ for the difference of two solutions with homogeneous [clamped boundary conditions](../../../../../clamped-boundary-condition.md), which gives $\int_{-L}^L(v'')^2\,dx=0$ and hence $v=0$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../../split.md)
6. [Elasticity and plasticity course of the University of Oxford](../../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
