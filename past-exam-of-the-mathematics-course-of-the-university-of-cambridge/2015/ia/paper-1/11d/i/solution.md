<h1 id="11d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) says that if $f:[a,b]\to\mathbb R$ is a [continuous function](../../../../../../continuous-function.md), then every value between $f(a)$ and $f(b)$ is attained at some point of $[a,b]$.

Endpoint values are already attained. Suppose $f(a)<y<f(b)$ and define $E=\{x\in[a,b]:f(x)<y\}$. It is nonempty and bounded above, so $c=\sup E$ exists. Continuity at $a$ ensures that $E$ contains points to the right of $a$, and continuity at $b$ ensures that no point sufficiently close to $b$ belongs to $E$. Hence $a<c<b$.

By the definition of the [supremum](../../../../../../supremum.md), there are points of $E$ approaching $c$. If $f(c)>y$, continuity would exclude all such nearby points from $E$, a contradiction. If $f(c)<y$, continuity would put some point to the right of $c$ in $E$, again a contradiction. Therefore **$f(c)=y$**. When $f(a)>f(b)$, apply this argument to $-f$. This proves the [intermediate value theorem](../../../../../../intermediate-value-theorem.md) in all cases.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11D](../../11d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
