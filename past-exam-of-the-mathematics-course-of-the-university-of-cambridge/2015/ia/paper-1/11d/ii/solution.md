<h1 id="11d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a chord of length $1/2$, consider the [continuous function](../../../../../../continuous-function.md) $h(x)=f(x+1/2)-f(x)$ on $[0,1/2]$. Since $f(0)=f(1)$,

$$
h(1/2)=f(1)-f(1/2)=-h(0).
$$

An endpoint zero already supplies the chord. Otherwise the endpoint values have opposite signs, so the [intermediate value theorem](../../../../../../intermediate-value-theorem.md) supplies $h(\alpha)=0$ at some $\alpha\in(0,1/2)$. Thus **a horizontal chord of length $1/2$ exists**.

For each integer $n>1$, define $h_n(x)=f(x+1/n)-f(x)$ on $[0,1-1/n]$. The sampled differences telescope:

$$
\sum_{j=0}^{n-1}h_n(j/n)=\sum_{j=0}^{n-1}\bigl(f((j+1)/n)-f(j/n)\bigr)=f(1)-f(0)=0.
$$

If any sampled value is zero, it gives the required chord. Otherwise there must be both a positive and a negative sampled value. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md), applied between their sample points, then gives $h_n(\alpha)=0$. Hence **a horizontal chord of length $1/n$ exists for every positive integer $n$**; for $n=1$, the endpoint chord itself suffices. This proves the [horizontal chord of reciprocal-integer length](../../../../../../horizontal-chord-of-reciprocal-integer-length.md) result, without restricting $n$ to powers of two.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
