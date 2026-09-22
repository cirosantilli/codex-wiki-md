<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $M=\|f\|_\infty$, the [essential supremum](../../../../essential-supremum.md) of $|f|$. If $M=0$, $f=0$ [almost everywhere](../../../../almost-everywhere.md) and every [Lp norm](../../../../lp-norm.md) is zero. Suppose $M>0$. Since $|f|\leq M$ [almost everywhere](../../../../almost-everywhere.md) and $m((0,1))=1$,

$$
\|f\|_p\leq M\qquad(1\leq p<\infty).
$$

For any $a$ with $0<a<M$, the [measurable set](../../../../measurable-set.md) $A_a=\{x\in(0,1):|f(x)|>a\}$ has positive [Lebesgue measure](../../../../lebesgue-measure.md); otherwise $a$ would be an essential upper bound. Hence

$$
\|f\|_p^p\geq\int_{A_a}|f|^p\,dx\geq a^pm(A_a),\qquad
\|f\|_p\geq a\,m(A_a)^{1/p}.
$$

For fixed $a$, $m(A_a)^{1/p}\to1$. Thus $\liminf_{p\to\infty}\|f\|_p\geq a$. Letting $a\uparrow M$ and combining with the upper bound proves

$$
\boxed{\lim_{p\to\infty}\|f\|_p=\|f\|_\infty.}
$$

The positive-measure superlevel sets explain why the [Lp norms converge to the supremum norm](../../../../lp-norms-converge-to-the-supremum-norm.md) even when the essential maximum is never attained.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
