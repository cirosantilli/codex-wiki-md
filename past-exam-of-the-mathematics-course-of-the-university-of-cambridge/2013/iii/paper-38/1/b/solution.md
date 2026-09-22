<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The increasing baseline order is $1/5,1/4,1/2,3/4$. A [water-filling algorithm](../../../../../../water-filling-algorithm.md) with three active coordinates gives

$$
\tau=\frac{1+1/5+1/4+1/2}{3}=\frac{13}{20},
\qquad \frac12<\frac{13}{20}<\frac34.
$$

Therefore, in the original coordinate order,

$$
\boxed{x^*=\left(\frac25,\frac3{20},\frac9{20},0\right).}
$$

The first three shifted coordinates all equal $13/20$, the fourth remains $3/4$, and the allocations sum to one. For an explicit [KKT](../../../../../../karush-kuhn-tucker-conditions.md) certificate take $\lambda=20/13$, $\nu_1=\nu_2=\nu_3=0$, and $\nu_4=20/13-4/3=8/39$. The [strict convexity](../../../../../../strictly-convex-function.md) established above makes this optimum unique.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
