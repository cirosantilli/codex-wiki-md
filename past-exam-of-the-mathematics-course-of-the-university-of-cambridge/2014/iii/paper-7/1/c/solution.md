<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Taking the [essential supremum](../../../../../../essential-supremum.md) in the characteristic solution gives the sharper estimate

$$
 \boxed{\|f_t\|_\infty\leq\|f_0\|_\infty+\int_0^t\|h(s,\cdot,\cdot)\|_\infty\,ds.}
$$

Indeed, the bijective [characteristic flow map](../../../../../../characteristic-flow-map.md) preserves each spatial-velocity [essential supremum](../../../../../../essential-supremum.md). If $H_t=\operatorname*{ess\,sup}_{0\leq s\leq t,\ x,v\in\mathbb R}|h(s,x,v)|$, this proves $\|f_t\|_\infty\leq\|f_0\|_\infty+tH_t$. A time-independent source has $H_t=\|h\|_{L^\infty(\mathbb R^2)}$, which is the displayed form. For a time-dependent source, the same symbol must mean a bound uniform over the elapsed time interval; its [norm](../../../../../../norm.md) at the final time alone need not bound the accumulated forcing.

The bound is **sharp**. Take $f_0=1$ and $h=1$, giving $f(t,x,v)=1+t$ and equality for every $t\geq0$. Both functions are smooth and bounded, although their finite-$p$ [integrals](../../../../../../integral.md) over the whole plane are infinite.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
