<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The small-[slope](../../../../slope.md) excess length is $\int(w')^2/2$, so the first term is the work needed against uniform [tension](../../../../tension.md). The second is the [potential energy](../../../../potential-energy.md) of the downward distributed load. Their sum is total [potential energy](../../../../potential-energy.md) subject to the obstacle [constraint](../../../../constraint-mechanics.md).

Expand the difference exactly:

$$
U[v]-U[w]=T\int w'(v'-w')\,dx+\int p(v-w)\,dx+\frac T2\int(v'-w')^2\,dx.
$$

The first two integrals together are nonnegative by part (b), and the square is nonnegative. Thus

$$
\boxed{U[w]\leq U[v]\quad\text{for every admissible }v.}
$$

For $T>0$ this also proves [uniqueness](../../../../uniqueness.md): equality for two [minimizers](../../../../global-minimizer.md) forces identical derivatives, and the fixed endpoints remove their additive constant. The [convex](../../../../convex-function.md) admissible set and strictly [convex](../../../../convex-function.md) energy make the [variational inequality](../../../../variational-inequality.md) a global minimization condition.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
