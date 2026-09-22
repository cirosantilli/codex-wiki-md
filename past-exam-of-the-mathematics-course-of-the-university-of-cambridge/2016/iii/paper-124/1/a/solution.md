<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [additive arithmetic function](../../../../../../additive-function-number-theory.md) satisfies $f(mn)=f(m)+f(n)$ for [coprime integers](../../../../../../coprime-integers.md) $m,n$; a [completely additive arithmetic function](../../../../../../completely-additive-arithmetic-function.md) satisfies this for all positive $m,n$. In either case $f(1)=0$. The [Fundamental theorem of arithmetic](../../../../../../fundamental-theorem-of-arithmetic.md) gives $f(n)=\sum_{p^k\parallel n}f(p^k)$, where $p^k\parallel n$ means that the [prime valuation](../../../../../../prime-valuation.md) of $n$ at $p$ is exactly $k$.

Under the [discrete uniform distribution](../../../../../../discrete-uniform-distribution.md) on $[N]$, the [expectation](../../../../../../expected-value.md) of the [indicator function](../../../../../../indicator-function.md) of $p^k\parallel n$ is

$$
\frac1N\left(\left\lfloor\frac N{p^k}\right\rfloor-\left\lfloor\frac N{p^{k+1}}\right\rfloor\right)=\frac1{p^k}\left(1-\frac1p\right)+O(N^{-1}).
$$

The formula remains valid when $p^{k+1}>N$. Applying [linearity of expectation](../../../../../../linearity-of-expectation.md) to the finite [prime power](../../../../../../prime-power.md) decomposition proves **the required mean formula**:

$$
\boxed{\mathbb E_N f=\sum_{p^k\le N}\frac{f(p^k)}{p^k}\left(1-\frac1p\right)+O\left(\frac1N\sum_{p^k\le N}|f(p^k)|\right).}
$$

For the last assertion, write the [excess prime-factor multiplicity](../../../../../../excess-prime-factor-multiplicity.md) directly as a sum of nonnegative [indicator functions](../../../../../../indicator-function.md):

$$
\Omega(n)-\omega(n)=\sum_p\sum_{k\ge2}\mathbf1_{p^k\mid n}.
$$

Here $\omega$ is the [prime omega function](../../../../../../prime-omega-function.md) and $\Omega$ is the [total number of prime factors](../../../../../../total-number-of-prime-factors.md). The [expectation](../../../../../../expected-value.md) is bounded independently of $N$, since

$$
\mathbb E_N(\Omega-\omega)\le\sum_p\sum_{k\ge2}\frac1{p^k}=\sum_p\frac1{p(p-1)}\le\sum_{m=2}^\infty\frac1{m(m-1)}=1.
$$

Thus [Markov inequality](../../../../../../markov-inequality.md) gives **vanishing probability on every diverging scale**:

$$
\boxed{\mathbb P_N(\Omega-\omega\ge t(N))\le\frac1{t(N)}\longrightarrow0.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
