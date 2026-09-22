<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a constant-coefficient [linear multistep method](../../../../linear-multistep-method-split.md), [zero-stability](../../../../zero-stability.md) means uniform boundedness of the propagation of starting perturbations as $h\to0$. Equivalently, every solution of the homogeneous [linear recurrence](../../../../linear-recurrence-relation.md)

$$
\sum_{j=0}^k\alpha_jv_{n+j}=0
$$

satisfies $|v_n|\leq K\max_{0\leq j<k}|v_j|$ for all $n\geq0$, with $K$ independent of $n$ and the starting values. The equivalent [root condition for a multistep method](../../../../root-condition-for-a-multistep-method.md) is that every [root of a polynomial](../../../../root-of-a-polynomial.md) $\zeta$ of the degree-$k$ [polynomial](../../../../polynomial-split.md) $\rho$ satisfies $|\zeta|\leq1$, and every root on $|\zeta|=1$ is simple. Indeed, a root of multiplicity $m$ produces recurrence modes $n^q\zeta^n$, $0\leq q<m$: repeated roots strictly inside the disk are harmless, whereas roots outside it or repeated roots on its boundary produce unbounded modes.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../../numerical-linear-algebra-and-numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
6. [MSc in mathematical modelling and scientific computing course of the University of Oxford](../../../../msc-in-mathematical-modelling-and-scientific-computing-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
