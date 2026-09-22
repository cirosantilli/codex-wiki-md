<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

Writing $p_n=\mathbb P(X=n)$, the ordinary [probability generating function](../../../../../probability-generating-function.md) is

$$
P_X(s)=\mathbb E[s^X]=\sum_{n=1}^Kp_ns^n.
$$

Its finite sum can be differentiated termwise, giving

$$
\boxed{\mathbb EX=P_X'(1).}
$$

The [Dirichlet probability generating function](../../../../../dirichlet-probability-generating-function.md) is the different transform $q(z)=\mathbb E[X^{-z}]$. Evaluating at $z=-1$ gives the first ordinary moment, whereas differentiation gives $q'(z)=-\sum_np_n(\log n)n^{-z}$. Therefore

$$
\boxed{\mathbb EX=q(-1),\qquad\mathbb E[\log X]=-q'(0).}
$$

There is no convergence issue because the support is finite and all its values are positive.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
