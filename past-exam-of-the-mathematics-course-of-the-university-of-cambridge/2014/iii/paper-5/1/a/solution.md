<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Taylor series](../../../../../../taylor-series.md) definition says that $f\in C^\infty(\mathbb R)$ and, for every $a$, there is $r>0$ such that

$$
f(x)=\sum_{n=0}^\infty\frac{f^{(n)}(a)}{n!}(x-a)^n\qquad(|x-a|<r).
$$

The equivalent [factorial derivative criterion for real analyticity](../../../../../../factorial-derivative-criterion-for-real-analyticity.md) says that, for every $a$, there are a neighborhood $I$ of $a$ and constants $C,A>0$ such that

$$
\boxed{\sup_{x\in I}|f^{(n)}(x)|\leq CA^n n!\quad(n\geq0).}
$$

The uniformity over $I$ matters: bounds only at $a$ do not exclude a [flat function](../../../../../../flat-function.md).

Assume the [factorial derivative criterion for real analyticity](../../../../../../factorial-derivative-criterion-for-real-analyticity.md). The [Taylor theorem with Lagrange remainder](../../../../../../taylor-theorem-with-lagrange-remainder.md) gives

$$
\left|f(a+h)-\sum_{n=0}^{N-1}\frac{f^{(n)}(a)}{n!}h^n\right|\leq C(A|h|)^N
$$

when the segment from $a$ to $a+h$ is contained in $I$. For sufficiently small $|h|<A^{-1}$ the [Taylor remainder](../../../../../../taylor-remainder.md) tends to zero, proving the [Taylor series](../../../../../../taylor-series.md) definition.

Conversely, write the convergent [power series](../../../../../../power-series.md) at $a$ as $\sum b_k h^k$. Choose $\rho$ strictly inside its radius of convergence; then $|b_k|\leq M\rho^{-k}$ for some $M$. Termwise [differentiation](../../../../../../differentiation.md) on $|h|\leq\rho/2$ gives

$$
|f^{(n)}(a+h)|\leq M\rho^{-n}n!\sum_{j=0}^\infty\binom{j+n}{n}2^{-j}
=2M(2/\rho)^n n!.
$$

Here the sum is $(1-1/2)^{-n-1}$, obtained by differentiating the [geometric series](../../../../../../geometric-series.md). This is the required locally uniform bound. **The two definitions of a [real analytic function](../../../../../../real-analytic-function.md) are equivalent.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
