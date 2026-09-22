<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the endpoint [continuity](../../../../../../continuous-function.md) of $f$ from part [b](../b.md), and interpret the displayed endpoint [derivatives](../../../../../../derivative.md) as one-sided endpoint values. Starting with $f(a)=f(b)=0$, [Rolle's theorem](../../../../../../rolle-theorem.md) gives $c_1\in(a,b)$ with $f'(c_1)=0$. Since also $f'(b)=0$, apply [Rolle's theorem](../../../../../../rolle-theorem.md) to $f'$ on $[c_1,b]$ to obtain $c_2\in(c_1,b)$ with $f''(c_2)=0$. Repeating gives

$$
a<c_1<\cdots<c_{n+1}<b,\qquad f^{(j)}(c_j)=0\quad(1\leq j\leq n+1).
$$

For $j<n$, the lower [derivative](../../../../../../derivative.md) $f^{(j)}$ is [continuous](../../../../../../continuous-function.md) in the interior by [differentiability implies continuity](../../../../../../differentiability-implies-continuity.md), and at $b$ by the existence of its next one-sided [derivative](../../../../../../derivative.md). At the final step, the stipulated [continuity](../../../../../../continuous-function.md) of $f^{(n)}$ on $[a,b]$ and its [differentiability](../../../../../../differentiability.md) on $(a,b)$ give exactly the hypotheses of [Rolle's theorem](../../../../../../rolle-theorem.md) on $[c_n,b]$. Therefore

$$
\boxed{f^{(n+1)}(c_{n+1})=0.}
$$

The endpoint regularity matters: merely assigning arbitrary values to $f$ at $a,b$ while prescribing only the interior [derivatives](../../../../../../derivative.md) would not justify the first application of [Rolle's theorem](../../../../../../rolle-theorem.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
