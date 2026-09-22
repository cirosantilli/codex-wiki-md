<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For fixed $\mu\ne0$, a large positive root must lie close to a [pole](../../../../../../pole.md) of the [tangent function](../../../../../../tangent-function.md): away from its [poles](../../../../../../pole.md), $\tan x$ cannot balance the unbounded right side. Label the adjacent [poles](../../../../../../pole.md) by $a_n=(n+1/2)\pi$ and write $x_n=a_n+\delta_n$. The [Taylor series](../../../../../../taylor-series.md) of $-\cot\delta$ gives

$$
-\frac1\delta+\frac\delta3+\frac{\delta^3}{45}+\cdots=\mu(a_n+\delta).
$$

Seek the [asymptotic expansion](../../../../../../asymptotic-expansion.md) $\delta=A/a_n+B/a_n^3+\cdots$. The coefficients of $a_n$ and $a_n^{-1}$ give

$$
-\frac1A=\mu,\qquad \frac B{A^2}+\frac A3=\mu A.
$$

Thus the [large roots near tangent poles](../../../../../../large-roots-near-tangent-poles.md) satisfy

$$
\boxed{x_n=a_n-\frac1{\mu a_n}+\frac{1/(3\mu^3)-1/\mu^2}{a_n^3}+O(a_n^{-5})}.
$$

The first correction already supplies the requested dependence on $\mu$. For $\mu>0$ the root approaches the [pole](../../../../../../pole.md) from below; for $\mu<0$ it approaches from above. This labels roots by their nearby [poles](../../../../../../pole.md), avoiding an irrelevant finite shift in the enumeration of positive roots.

**No positivity restriction on $\mu$ is required.** The expansion requires $\mu\ne0$ fixed and $|\mu|a_n\gg1$, so the displacement is small. It is not uniform as $\mu\to0$. At $\mu=0$ the roots are exactly $n\pi$, a different leading sequence; these cannot be recovered by setting $\mu=0$ in the [pole](../../../../../../pole.md) expansion. If $\mu$ varies with $n$, its size must be checked against the small-displacement and successive-term conditions rather than using the fixed-parameter remainder blindly.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
