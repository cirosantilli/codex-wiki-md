<h1 id="12e/solution">Solution</h1>

↑ **Parent:** [12E](../12e.md)

First establish the interior convergence lemma for a [power series](../../../../../power-series.md). If $\sum a_nw^n$ converges at some $w\ne0$, its terms are bounded: $|a_nw^n|\leq M$ for a finite $M$. For every $|z|<|w|$,

$$
|a_nz^n|\leq M\left(\frac{|z|}{|w|}\right)^n.
$$

Comparison with a convergent [geometric series](../../../../../geometric-series.md) proves [absolute convergence](../../../../../absolute-convergence.md) at $z$.

Now let

$$
R=\sup\{|w|:\textstyle\sum a_nw^n\text{ converges}\}\in[0,\infty].
$$

The set contains zero, since at $w=0$ only the constant term remains. If $|z|<R$, the definition of [supremum](../../../../../supremum.md) gives a point of convergence $w$ with $|w|>|z|$. The lemma proves [absolute convergence](../../../../../absolute-convergence.md) at $z$. If $|z|>R$, convergence would place $|z|$ in the set defining $R$, a contradiction. This proves the existence of a [radius of convergence](../../../../../radius-of-convergence.md), including $R=0$ and $R=\infty$:

$$
\boxed{\text{Convergence for }|z|<R,\qquad\text{divergence for }|z|>R.}
$$

The proof leaves behavior on $|z|=R$ open; it need not be uniform around that circle. The two examples illustrate opposite possibilities.

## ↑ Ancestors (10)

1. [12E](../12e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
