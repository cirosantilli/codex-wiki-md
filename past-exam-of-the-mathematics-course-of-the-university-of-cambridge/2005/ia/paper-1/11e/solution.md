<h1 id="11e/solution">Solution</h1>

↑ **Parent:** [11E](../11e.md)

To prove the required zero-existence statement directly, let $S=\{x\in[a,b]:f(x)\le0\}$ and $c=\sup S$. This set is nonempty and bounded. Continuity and the strict signs at the endpoints give a right neighbourhood of $a$ with negative values and a left neighbourhood of $b$ with positive values; consequently $a<c<b$. If $f(c)<0$, continuity would give points of $S$ to the right of $c$, contradicting its upper-bound property. If $f(c)>0$, continuity would give an interval immediately to the left of $c$ containing no points of $S$, contradicting the approximation property of its [supremum](../../../../../supremum.md). Hence **$f(c)=0$ for some $c\in(a,b)$**, proving this form of the [intermediate value theorem](../../../../../intermediate-value-theorem.md).

For the half-interval claim, put $H(x)=g(x+1/2)-g(x)$ on $[0,1/2]$. It is a [continuous function](../../../../../continuous-function.md) and

$$
H(1/2)=g(1)-g(1/2)=g(0)-g(1/2)=-H(0).
$$

If either endpoint value is zero, it supplies the answer. Otherwise the signs are opposite, so the [intermediate value theorem](../../../../../intermediate-value-theorem.md), applied also to $-H$ if necessary, gives an interior zero. Thus **$g(c+1/2)=g(c)$ for some $c\in[0,1/2]$**.

For general positive integer $n$, define $H_n(x)=g(x+1/n)-g(x)$ on $[0,(n-1)/n]$. At its grid points,

$$
\sum_{k=0}^{n-1}H_n(k/n)=\sum_{k=0}^{n-1}\bigl[g((k+1)/n)-g(k/n)\bigr]=g(1)-g(0)=0.
$$

If a sampled value is zero, it is the desired point. If none is zero, not all sampled values can have the same sign, so two have opposite signs; continuity gives a zero between their grid points. This proves the [horizontal chord of reciprocal-integer length](../../../../../horizontal-chord-of-reciprocal-integer-length.md):

$$
\boxed{\exists c_n\in[0,(n-1)/n]\quad g(c_n+1/n)=g(c_n).}
$$

For $n=1$ the interval is the single point zero, which works by the endpoint equality itself. The proof does not require a differentiable function or a periodic extension.

## ↑ Ancestors (10)

1. [11E](../11e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
