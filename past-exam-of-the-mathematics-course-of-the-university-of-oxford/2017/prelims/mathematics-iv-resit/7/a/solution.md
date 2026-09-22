<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Start with $[a_0,b_0]=[a,b]$. At stage $n$, form the [midpoint](../../../../../../midpoint.md) $c_n=(a_n+b_n)/2$. If $f(c_n)=0$, stop; for a [sequence](../../../../../../sequence.md) defined for all later indices, repeat $c_n$ forever. Otherwise retain the half-[interval](../../../../../../interval-mathematics.md) with opposite endpoint signs: set $[a_{n+1},b_{n+1}]=[a_n,c_n]$ if $f(a_n)f(c_n)<0$, and $[a_{n+1},b_{n+1}]=[c_n,b_n]$ otherwise. This is the [bisection method](../../../../../../bisection-method.md).

If it never stops, the [closed intervals](../../../../../../closed-real-interval.md) are nested, retain $f(a_n)f(b_n)<0$, and have lengths

$$
b_n-a_n=\frac{b-a}{2^n}\longrightarrow0.
$$

By the [nested interval theorem](../../../../../../nested-interval-theorem.md), there is a unique real $\xi$ in their intersection. In particular, $a_n\to\xi$, $b_n\to\xi$, and the [sequence](../../../../../../sequence.md) of [midpoints](../../../../../../midpoint.md) satisfies

$$
|c_n-\xi|\leq\frac{b-a}{2^{n+1}}\longrightarrow0.
$$

Since $f$ is [continuous](../../../../../../continuous-function.md), $f(a_n)f(b_n)\to f(\xi)^2$. All these products are negative, so their [limit of a sequence](../../../../../../limit-of-a-sequence.md) is nonpositive. Therefore $f(\xi)^2\leq0$, forcing $f(\xi)=0$. We have proved that the [sequence](../../../../../../sequence.md) is a [convergent sequence](../../../../../../convergent-sequence.md) whose [limit of a sequence](../../../../../../limit-of-a-sequence.md) is a [zero of a function](../../../../../../zero-of-a-function.md):

$$
\boxed{c_n\longrightarrow\xi,\qquad f(\xi)=0,\qquad |c_n-\xi|\leq\frac{b-a}{2^{n+1}}.}
$$

The [error bound](../../../../../../error-bound.md) applies at every stage before exact termination; after termination the error is zero. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) also guarantees a [zero of a function](../../../../../../zero-of-a-function.md) in each retained [interval](../../../../../../interval-mathematics.md), but the nested-[interval](../../../../../../interval-mathematics.md) argument identifies the particular one to which the [sequence](../../../../../../sequence.md) of [midpoints](../../../../../../midpoint.md) converges.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
