<h1 id="p/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret the weighted function space as measurable functions modulo equality [almost everywhere](../../../../../almost-everywhere.md), so the integral form is a genuine [inner product](../../../../../inner-product-split.md). Assume $q\in\Pi_k\subseteq V$. If the residual is [orthogonal](../../../../../orthogonal-vectors.md) to $\Pi_k$, then for $p\in\Pi_k$,

$$
\|f-p\|^2=\|(f-q)+(q-p)\|^2=\|f-q\|^2+\|q-p\|^2\ge\|f-q\|^2.
$$

Thus $q$ is a [best approximation](../../../../../best-approximation-in-a-normed-space.md). Conversely, if it is best, take any $r\in\Pi_k$ and vary through $q+tr$. The [polynomial](../../../../../polynomial-split.md)

$$
\|f-q-tr\|^2=\|f-q\|^2-2t\langle f-q,r\rangle+t^2\|r\|^2
$$

has a [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md) at $t=0$, so its [derivative](../../../../../derivative.md) there vanishes. Hence $\boxed{\langle f-q,r\rangle=0}$ for every $r\in\Pi_k$. The same [Pythagorean identity](../../../../../pythagorean-theorem-in-an-inner-product-space.md) proves uniqueness of the [best approximation](../../../../../best-approximation-in-a-normed-space.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [P](../../../p.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
