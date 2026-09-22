<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $w=e^{i\theta}$. By [Euler's formula](../../../../euler-s-formula.md), $w-w^{-1}=2i\sin\theta$. The [binomial theorem](../../../../binomial-theorem.md) gives

$$
(w-w^{-1})^7=w^7-7w^5+21w^3-35w+35w^{-1}-21w^{-3}+7w^{-5}-w^{-7}.
$$

Group opposite powers and use $w^j-w^{-j}=2i\sin(j\theta)$:

$$
(2i)^7\sin^7\theta=2i\big[\sin7\theta-7\sin5\theta+21\sin3\theta-35\sin\theta\big].
$$

Since $(2i)^7=-128i$, division by $-2i$ yields

$$
\boxed{64\sin^7\theta=35\sin\theta-21\sin3\theta+7\sin5\theta-\sin7\theta.}
$$

This derivation is an application of the same exponential representation underlying [De Moivre's theorem](../../../../de-moivre-s-theorem.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
