<h1 id="23h/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For integer $k\geq1$, define $f_k(n)=f(k,n)$. The assumed monotonicity in $t$ gives

$$
f_k(n)\uparrow\lim_{t\to\infty}f(t,n)
$$

for every $n$. Apply the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) on $\mathbb N$ with counting measure:

$$
\lim_{k\to\infty}\sum_{n\geq1}f(k,n)
=\sum_{n\geq1}\lim_{k\to\infty}f(k,n)
=\sum_{n\geq1}\lim_{t\to\infty}f(t,n).
$$

The function $t\mapsto\sum_nf(t,n)$ is itself nondecreasing, and the positive integers are cofinal in $\mathbb R$ as $t\to\infty$, so its limit over real $t$ equals its limit over integer $k$. Therefore

$$
\boxed{
\lim_{t\to\infty}\sum_{n\geq1}f(t,n)
=\sum_{n\geq1}\lim_{t\to\infty}f(t,n)}.
$$

Without monotonicity, take

$$
f(t,n)=\mathbf1_{[n,n+1)}(t)
\qquad(t\geq1).
$$

For each fixed $n$, $f(t,n)\to0$, so the sum of the pointwise limits is zero. At every $t\geq1$, however, exactly one term is one, so $\sum_nf(t,n)=1$ and its limit is one. This [moving-spike obstruction to interchanging a limit and an infinite sum](../../../../../../moving-spike-obstruction-to-interchanging-a-limit-and-an-infinite-sum.md) gives the required counterexample.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [23H](../../23h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
