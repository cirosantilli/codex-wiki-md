<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the standard [sl2 Lie algebra](../../../../../../sl2-lie-algebra.md) relations $[h,e]=2e$, $[h,f]=-2f$ and $[e,f]=h$. The [classification of finite-dimensional sl2 representations](../../../../../../classification-of-finite-dimensional-sl2-representations.md) says that every finite-dimensional complex module is a direct sum of $L(m)$, $m\in\mathbb Z_{\geq0}$, where $L(m)$ has [weights](../../../../../../weight-representation-theory.md) $m,m-2,\ldots,-m$. The raising operator $e$ and lowering operator $f$ move weights by two and minus two. On $L(m)$ each therefore has $(m+1)$st power zero. There is consequently one integer $N$ such that $e^N=f^N=0$ on all of $V$.

The [matrix exponentials](../../../../../../matrix-exponential.md) are thus finite [polynomials](../../../../../../polynomial-split.md) in [nilpotent operators](../../../../../../nilpotent-linear-map.md):

$$
\exp(e)=\sum_{j=0}^{N-1}\frac{e^j}{j!},\qquad\exp(-f)=\sum_{j=0}^{N-1}\frac{(-f)^j}{j!}.
$$

Each is a well-defined endomorphism, and its inverse is obtained by negating the argument. Their product is therefore a linear automorphism,

$$
\boxed{s=\exp(e)\exp(-f)\exp(e)\in\operatorname{GL}(V).}
$$

This [Weyl reflection lift in an sl2 representation](../../../../../../weyl-reflection-lift-in-an-sl2-representation.md) is algebraically defined by finite sums; no choice of topology or convergence of an infinite series is needed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
