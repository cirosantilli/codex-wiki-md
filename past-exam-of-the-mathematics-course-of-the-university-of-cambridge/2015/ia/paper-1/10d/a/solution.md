<h1 id="10d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We use the [Bolzano-Weierstrass theorem](../../../../../../bolzano-weierstrass-theorem.md): every bounded real sequence has a convergent subsequence. If $f$ were unbounded on $[a,b]$, there would be $x_n\in[a,b]$ with $|f(x_n)|\geq n$. The [Bolzano-Weierstrass theorem](../../../../../../bolzano-weierstrass-theorem.md) gives a subsequence $x_{n_k}\to c$, and the closed interval contains $c$. Since $f$ is a [continuous function](../../../../../../continuous-function.md), $f(x_{n_k})\to f(c)$, contradicting $|f(x_{n_k})|\geq n_k\to\infty$. Thus **$f$ is bounded**.

Let $s=\sup_{x\in[a,b]}f(x)$. By the definition of the [supremum](../../../../../../supremum.md), choose $y_n$ with $s-1/n<f(y_n)\leq s$. Again the [Bolzano-Weierstrass theorem](../../../../../../bolzano-weierstrass-theorem.md) gives $y_{n_k}\to d\in[a,b]$. Continuity yields $f(d)=s$. Applying the same argument to $-f$ gives a point where $f$ attains its [infimum](../../../../../../infimum.md). Therefore **both the supremum and the infimum are attained**. This proves the [extreme value theorem](../../../../../../extreme-value-theorem.md) for a closed bounded interval.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10D](../../10d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
