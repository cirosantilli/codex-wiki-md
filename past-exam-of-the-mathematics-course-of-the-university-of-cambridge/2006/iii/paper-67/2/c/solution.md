<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take any [trigonometric polynomial](../../../../../../trigonometric-polynomial.md) $t\in\mathcal T_n$. The reproduction property in (a) gives

$$
f-v_{n,m}f=(f-t)-v_{n,m}(f-t).
$$

By (b),

$$
\|f-v_{n,m}f\|_\infty\leq\left(2+\frac{2n}{m}\right)\|f-t\|_\infty.
$$

Taking the infimum over $t\in\mathcal T_n$ yields the [polynomial reproduction error bound](../../../../../../polynomial-reproduction-error-bound.md) for this operator. With $E_n(f)=\inf_{t\in\mathcal T_n}\|f-t\|_\infty$ and $n/m\leq M$, it becomes

$$
\boxed{\|f-v_{n,m}f\|_\infty\leq2(M+1)E_n(f).}
$$

This is a near-best [uniform approximation](../../../../../../uniform-approximation-split.md) estimate; it follows from reproduction and boundedness without requiring the [de la Vallée Poussin sum](../../../../../../de-la-vallee-poussin-sum.md) itself to be a best approximant.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
