<h1 id="11/c/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Induction from $M^2=M$ gives $M^j=M$ for every integer $j\geq1$. Separate the zeroth term of the [matrix exponential](../../../../../matrix-exponential.md) series:

$$
\begin{aligned}
e^{\alpha M}
&=I+\sum_{j=1}^\infty\frac{\alpha^jM^j}{j!}
=I+M\sum_{j=1}^\infty\frac{\alpha^j}{j!}\\
&=I+(e^\alpha-1)M.
\end{aligned}
$$

Therefore the [exponential of an idempotent linear map](../../../../../exponential-of-an-idempotent-linear-map.md) is

$$
\boxed{e^{\alpha M}=I+(e^\alpha-1)M=(I-M)+e^\alpha M.}
$$

The last form shows its action directly: it multiplies the [image of a linear map](../../../../../image-of-a-linear-map.md) of $M$ by $e^\alpha$ and fixes its [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md). No Hermiticity assumption on the [idempotent matrix](../../../../../idempotent-matrix.md) is needed.

## ↑ Ancestors (13)

1. [Vi](../vi.md)
2. [C](../../c.md)
3. [11](../../../11.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the mathematical methods I course of the University of Oxford](../../../../split.md)
6. [Mathematical methods I course of the University of Oxford](../../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
