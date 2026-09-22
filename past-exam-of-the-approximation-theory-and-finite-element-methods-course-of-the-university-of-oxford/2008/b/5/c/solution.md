<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Testing against compactly supported smooth [functions](../../../../../function-split.md) gives the distributional identity $u''=\cos x\,u-f$. The right side belongs to $L^2$, since $u\in H^1$ and $\cos x$ is bounded. Therefore $u'\in H^1$ and **$u\in H^2(0,1)$**. This also makes the endpoint [derivative](../../../../../derivative.md) traces meaningful, and integrating the weak form by parts recovers the Robin conditions.

The standard piecewise linear [finite element interpolation estimate](../../../../../finite-element-interpolation-estimate.md) is

$$
\|u-I_hu\|_{L^2}\leq C_0h^2\|u''\|_{L^2},\qquad
\|(u-I_hu)'\|_{L^2}\leq C_1h\|u''\|_{L^2},
$$

with constants independent of $h$. Hence $\|u-I_hu\|_{H^1}\leq Ch\|u''\|_{L^2}$ for $h\leq1$. By [Céa's lemma](../../../../../cea-s-lemma.md), with the fixed continuity and [coercivity](../../../../../coercive-function.md) constants of $a$,

$$
\boxed{\|u-u_h\|_{H^1}\leq Ch\|u''\|_{L^2}=O(h).}
$$

The constant depends on the continuous problem but not on [mesh](../../../../../finite-element-mesh.md) refinement.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
