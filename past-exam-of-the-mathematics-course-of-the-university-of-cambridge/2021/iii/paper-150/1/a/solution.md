<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Begin with the [Von Mangoldt divisor identity](../../../../../../von-mangoldt-divisor-identity.md)

$$
\log n=\sum_{d\mid n}\Lambda(d).
$$

Summing it for $n\leq x$ and reversing the order gives

$$
\log\lfloor x\rfloor!
=\sum_{d\leq x}\Lambda(d)\left\lfloor\frac xd\right\rfloor
=x\sum_{d\leq x}\frac{\Lambda(d)}d+O(\psi(x)).
$$

The given bound $\psi(x)\ll x$ and the [Stirling formula](../../../../../../stirling-formula.md) therefore imply

$$
A(x):=\sum_{d\leq x}\frac{\Lambda(d)}d=\log x+O(1).
$$

Apply [partial summation](../../../../../../abel-s-summation-formula.md) with the weight $1/\log n$. Writing $A(t)=\log t+E(t)$, where $E(t)=O(1)$, gives

$$
\sum_{2\leq n\leq x}\frac{\Lambda(n)}{n\log n}
=\frac{A(x)}{\log x}
+\int_2^x\frac{A(t)}{t(\log t)^2}\,dt
=\log\log x+C+O\left(\frac1{\log x}\right).
$$

Indeed, the integral of $E(t)/(t(\log t)^2)$ converges, and its tail from $x$ to infinity is $O(1/\log x)$.

Grouping the left side by [prime powers](../../../../../../prime-power.md) yields

$$
\sum_{2\leq n\leq x}\frac{\Lambda(n)}{n\log n}
=\sum_{p^k\leq x}\frac1{kp^k}
=\sum_{p\leq x}\frac1p
+\sum_{\substack{k\geq2\\p^k\leq x}}\frac1{kp^k}.
$$

The full double series over $k\geq2$ converges. Its tail beyond $x$ is $O(x^{-1/2})$: split at $p=\sqrt x$, use a geometric series for $p\leq\sqrt x$, and compare $\sum_{p>\sqrt x}p^{-2}$ with the corresponding sum over integers. Absorbing its limit into the constant proves the [Mertens theorem for reciprocal primes](../../../../../../mertens-second-theorem.md)

$$
\boxed{\sum_{p\leq x}\frac1p
=\log\log x+c+O\left(\frac1{\log x}\right)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
