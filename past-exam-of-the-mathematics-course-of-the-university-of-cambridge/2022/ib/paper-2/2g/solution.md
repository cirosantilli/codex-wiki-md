<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

Because $f$ is a bijection and $e$ is a metric,

$$
d'(x,y)=e(f(x),f(y))
$$

is nonnegative, symmetric, obeys the triangle inequality, and vanishes exactly when $x=y$. Hence it is a metric. Its open sets are precisely the inverse images under $f$ of $e$-open sets in $N$. Since $f:(M,d)\to(N,e)$ is a [homeomorphism](../../../../../homeomorphism.md), these are exactly the $d$-open sets. Thus $d'$ and $d$ are [equivalent metrics](../../../../../equivalence-of-metrics.md).

Let

$$
h(x)=\frac12+\frac1\pi\arctan x,
$$

a homeomorphism $\mathbb R\to(0,1)$, and define

$$
\boxed{d'(x,y)=|h(x)-h(y)|}.
$$

This metric induces the standard topology on $\mathbb R$. However, the sequence $x_n=n$ is $d'$-Cauchy because $h(n)\to1$. If it converged to $x\in\mathbb R$, then continuity of $h$ would give $h(x)=1$, impossible. Therefore $(\mathbb R,d')$ is not complete.

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
