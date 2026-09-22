<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [principal complex logarithm](../../../../principal-complex-logarithm.md) at each stage of the nested [complex exponentiation](../../../../complex-exponentiation.md). Since $\operatorname{Log}i=i\pi/2$,

$$
i^i=e^{i\operatorname{Log}i}=e^{-\pi/2}.
$$

This inner value is positive real, so its [principal complex logarithm](../../../../principal-complex-logarithm.md) is $-\pi/2$. Consequently

$$
\boxed{(i^i)^i=e^{i(-\pi/2)}=-i=0-i.}
$$

One must retain the parentheses: [complex exponentiation is not associative](../../../../complex-exponentiation-is-not-associative.md). If all [complex logarithm](../../../../complex-logarithm.md) branches are allowed, the inner values are $e^{-\pi/2-2\pi k}$. Taking the outer logarithm with an independent integer branch index $\ell$ yields $\exp[-i\pi/2-2\pi ik-2\pi\ell]=-ie^{-2\pi\ell}$. Thus the complete multivalued set is $\{-ie^{-2\pi\ell}:\ell\in\mathbb Z\}$, and the boxed answer selects its principal evaluation.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
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
