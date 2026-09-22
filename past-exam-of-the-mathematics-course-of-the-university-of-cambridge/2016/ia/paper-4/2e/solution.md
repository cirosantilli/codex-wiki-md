<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

For a nonempty [set](../../../../../set-split.md) $S\subseteq\mathbb R$, an [upper bound in a partially ordered set](../../../../../upper-bound-in-a-partially-ordered-set.md) is a real number $u$ such that $s\leq u$ for every $s\in S$. Its [supremum](../../../../../supremum.md), or least upper bound, is an upper bound $L$ with $L\leq u$ for every upper bound $u$. The [least-upper-bound property](../../../../../least-upper-bound-property.md) asserts that every nonempty set of [real numbers](../../../../../real-number.md) bounded above has a real [supremum](../../../../../supremum.md).

Let $(x_n)$ be a bounded, increasing [sequence](../../../../../sequence.md); here increasing allows $x_{n+1}=x_n$. Apply the [least-upper-bound property](../../../../../least-upper-bound-property.md) to its set of terms and put $L=\sup\{x_n:n\geq1\}$. Given $\varepsilon>0$, the number $L-\varepsilon$ cannot be an upper bound, so some $x_N$ satisfies $x_N>L-\varepsilon$. The [monotone sequence](../../../../../monotone-sequence.md) property then gives

$$
L-\varepsilon<x_N\leq x_n\leq L\qquad(n\geq N).
$$

Hence $|x_n-L|<\varepsilon$ for all $n\geq N$. This proves the [monotone bounded sequence](../../../../../monotone-bounded-sequence.md) result, with **limit** $\boxed{x_n\longrightarrow L}$.

For the two [series](../../../../../series-mathematics.md), define their partial sums $A_N=\sum_{n=1}^N a_n$ and $B_N=\sum_{n=1}^N b_n$. Positivity makes both partial-sum sequences increasing, and termwise comparison gives $0<B_N\leq A_N$. Since $(A_N)$ is a [convergent sequence](../../../../../convergent-sequence.md), it is bounded above, and therefore so is $(B_N)$. Applying the [monotone bounded sequence](../../../../../monotone-bounded-sequence.md) result already proved shows that $(B_N)$ converges. By the definition of a [convergent series](../../../../../convergent-series.md), **$\sum_{n=1}^\infty b_n$ converges**. This is the [comparison test for series](../../../../../comparison-test-for-series.md) for positive terms.

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
