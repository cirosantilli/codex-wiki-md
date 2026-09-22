<h1 id="10d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) states that, if $f$ is a [continuous function](../../../../../../continuous-function.md) on a [closed interval](../../../../../../closed-real-interval.md) $[a,b]$, every value between $f(a)$ and $f(b)$ equals $f(c)$ for some $c\in[a,b]$. If the value is strictly between the endpoint values, $c$ may be chosen in $(a,b)$.

Here is a proof from the [supremum](../../../../../../supremum.md) property of the real numbers. Suppose $f(a)<y<f(b)$; the reverse inequality is reduced to this case by replacing $f,y$ with $-f,-y$. Let

$$
E=\{t\in[a,b]:f(t)\leq y\},\qquad c=\sup E.
$$

The set is nonempty because it contains $a$ and is bounded above by $b$. [Continuity](../../../../../../continuous-function.md) at $a$ supplies points of $E$ to the right of $a$, while [continuity](../../../../../../continuous-function.md) at $b$ excludes a neighborhood of $b$ from $E$. Hence $a<c<b$. By the definition of [supremum](../../../../../../supremum.md), there are $t_n\in E$ with $t_n\to c$. [Continuity](../../../../../../continuous-function.md) gives $f(c)=\lim f(t_n)\leq y$. If $f(c)<y$, [continuity](../../../../../../continuous-function.md) would give a point just to the right of $c$ still satisfying $f(t)<y$, contradicting that $c$ is an upper bound for $E$. Thus $f(c)=y$. Values equal to either endpoint are attained at that endpoint, completing the proof.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10D](../../10d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
