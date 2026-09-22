<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One form of the [Jacobi triple product](../../../../../../jacobi-triple-product.md) is, for $0<|q|<1$ and $z\ne0$,

$$
\boxed{\sum_{n\in\mathbb Z}q^{n^2}z^n
=\prod_{j=1}^\infty(1-q^{2j})(1+zq^{2j-1})(1+z^{-1}q^{2j-1}).}
$$

Both sides converge locally uniformly on the punctured $z$ plane. Here is a finite-product proof which also determines the multiplicative constant.

Put $Q=q^2$ and $(Q;Q)_m=\prod_{j=1}^m(1-Q^j)$, with value one at $m=0$. Define the [Gaussian binomial coefficient](../../../../../../gaussian-binomial-coefficient.md) ${m\brack k}_Q=(Q;Q)_m/[(Q;Q)_k(Q;Q)_{m-k}]$. The recurrence ${m\brack k}_Q={m-1\brack k}_Q+Q^{m-k}{m-1\brack k-1}_Q$ proves by induction that

$$
\prod_{j=0}^{m-1}(1+tQ^j)
=\sum_{k=0}^mQ^{k(k-1)/2}{m\brack k}_Qt^k.
$$

Rewrite the two finite factors as

$$
\prod_{j=1}^N(1+zq^{2j-1})(1+z^{-1}q^{2j-1})
=z^{-N}q^{N^2}\prod_{j=0}^{2N-1}(1+zq^{1-2N}Q^j).
$$

The finite identity, with $n=k-N$, makes this $\sum_{n=-N}^Nz^nq^{n^2}{2N\brack N+n}_Q$. Multiply by $(Q;Q)_N$. For each fixed integer $n$, the resulting coefficient tends to one, because $(Q;Q)_m$ tends to a nonzero limit and ${2N\brack N+n}_Q\to1/(Q;Q)_\infty$.

All finite $(Q;Q)_m$ are uniformly bounded above and away from zero. Thus these coefficients have one uniform bound, and $\sum_{n\in\mathbb Z}|q|^{n^2}|z|^n$ is uniformly summable on compact annuli. Dominated convergence passes the limit through the finite sums and proves the boxed formula. At $q=0$ the formula follows by its limiting value one. The frequently used alternative form is

$$
\prod_{j\geq1}(1-t^j)(1+u t^{j-1})(1+u^{-1}t^j)
=\sum_{m\in\mathbb Z}u^m t^{m(m-1)/2},\qquad |t|<1.
$$

It follows by the substitution $q^2=t$, $z=u/q$, and is the version used for the charge-counting identity in Question 8.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
