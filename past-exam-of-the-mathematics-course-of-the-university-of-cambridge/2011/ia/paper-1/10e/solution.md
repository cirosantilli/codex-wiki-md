<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

The [intermediate value theorem](../../../../../intermediate-value-theorem.md) states that if $f:[a,b]\to\mathbb R$ is [continuous](../../../../../continuous-function.md), then every real value between $f(a)$ and $f(b)$ is attained at some $c\in[a,b]$. Here is a proof using [completeness of the real numbers](../../../../../completeness-of-the-real-numbers.md). Endpoint values are immediate, so suppose $f(a)<y<f(b)$; reversing the sign of $f$ handles the other ordering. Let

$$
S=\{x\in[a,b]:f(x)<y\},\qquad c=\sup S.
$$

The set is nonempty and bounded above. [Continuity](../../../../../continuous-function.md) at $a$ puts points to the right of $a$ in $S$, while [continuity](../../../../../continuous-function.md) at $b$ excludes an entire interval to the left of $b$, so $a<c<b$. If $f(c)<y$, [continuity](../../../../../continuous-function.md) puts some point larger than $c$ in $S$, contradicting its [supremum](../../../../../supremum.md). If $f(c)>y$, [continuity](../../../../../continuous-function.md) excludes $S$ in a neighborhood of $c$, contradicting the existence of points of $S$ arbitrarily close to its [supremum](../../../../../supremum.md) from below. Therefore $f(c)=y$, proving the theorem.

For the fixed-point assertion, put $g(x)=f(x)-x$. This is [continuous](../../../../../continuous-function.md), with $g(0)=f(0)\ge0$ and $g(1)=f(1)-1\le0$. If either endpoint value is zero it already gives a [fixed point](../../../../../fixed-point.md); otherwise the [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives an interior zero. Hence

$$
\boxed{\text{Every continuous self-map of }[0,1]\text{ has a fixed point.}}
$$

The proof needs both [continuity](../../../../../continuous-function.md) and the closed-interval endpoint information; the following counterexamples separate those hypotheses.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
