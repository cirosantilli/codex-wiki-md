<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [relative-error approximation for minimization](../../../../../../relative-error-approximation-for-minimization.md) convention: an $\varepsilon$-approximation returns a feasible solution of value $Y$ with $Y\leq(1+\varepsilon)Y^*$ on every instance, where $Y^*$ is the optimum. Equivalently the relative excess is at most $\varepsilon$; the multiplicative-ratio convention reports $1+\varepsilon$ instead.

Before item $j$ is assigned, the total load already placed is $\sum_{i<j}w_i$. The lighter of two bins has load at most half that total. Positivity of the weights gives

$$
L_j\leq\frac12\sum_{i<j}w_i\leq\frac12(s-w_j).
$$

Choose a bin attaining the final maximum load $Y$, and let $j$ be its last assigned item. No later item enters that bin, so

$$
Y=L_j+w_j\leq\frac{s+w_j}{2}\leq\frac s2+\frac{w_{\max}}2.
$$

Every feasible schedule has $Y^*\geq s/2$ and $Y^*\geq w_{\max}$. Hence

$$
Y\leq\frac s2+\frac{w_{\max}}2\leq Y^*+\frac12Y^*=\frac32Y^*.
$$

The ordered weights $1,1,2$ make the greedy loads $1,1$ after two assignments and then $3,1$, regardless of how the final tie is resolved. The optimal partition has loads $2,2$. Thus the factor $3/2$ is attained, not merely a loose bound. We conclude the sharp [greedy two-bin scheduling bound](../../../../../../greedy-two-bin-scheduling-bound.md)

$$
\boxed{\varepsilon_{\min}=\frac12\text{ in relative-error notation, or ratio }\frac32.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
