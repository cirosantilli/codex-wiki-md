<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
W(n)=\sum_{d\mid n}\mu(d)f\left(\frac{\log d}{\log D}\right).
$$

If $Y<n\leq Y+X$ is prime, then $n>D=X^{1/10}$. Since $f$ is supported on $[-1,1]$, the only divisor of $n$ contributing to $W(n)$ is $d=1$, and $W(n)=f(0)=1$. Every summand $W(n)^2$ is nonnegative, so

$$
\sum_{Y<n\leq Y+X}W(n)^2\geq\pi(Y+X)-\pi(Y).
$$

Let

$$
z_j=\frac{1-2\pi it_j}{\log D}.
$$

Since $g$ is the [Fourier transform](../../../../../../fourier-transform.md) of $x\mapsto e^xf(x)$, the [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md) gives the [Fourier representation of a smooth Selberg weight](../../../../../../fourier-representation-of-a-smooth-selberg-weight.md)

$$
f\left(\frac{\log d}{\log D}\right)
=\int_{-\infty}^{\infty}g(t)d^{-(1-2\pi it)/\log D}\,dt.
$$

Expanding the square, interchanging the absolutely convergent sums and integrals, and using

$$
\#\{Y<n\leq Y+X:[d_1,d_2]\mid n\}
=\frac X{[d_1,d_2]}+O(1),
$$

we obtain

$$
\sum_{Y<n\leq Y+X}W(n)^2
=X\iint_{\mathbb R^2}g(t_1)g(t_2)H(t_1,t_2,D)\,dt_1dt_2+O(D^2).
$$

The error is $O(D^2)$ because the support of $f$ restricts both divisors to $d_j\leq D$. The main factor is

$$
H(t_1,t_2,D)
=\sum_{d_1,d_2\geq1}
\frac{\mu(d_1)\mu(d_2)}{[d_1,d_2]d_1^{z_1}d_2^{z_2}},
$$

and its [Euler product](../../../../../../euler-product.md) is

$$
\boxed{
H(t_1,t_2,D)
=\prod_p\left(
1-p^{-1-z_1}-p^{-1-z_2}+p^{-1-z_1-z_2}
\right).}
$$

It remains to estimate the integral using the assumed zeta-factor bound. The transform $g$ is a [Schwartz function](../../../../../../schwartz-function.md), since $e^xf(x)$ is smooth and compactly supported. We may therefore truncate to $|t_1|,|t_2|\leq T$, losing an arbitrarily large negative power of $T$. Uniformly in the needed truncated range, the standard estimates near the pole of the [Riemann zeta function](../../../../../../riemann-zeta-function.md) give

$$
\left|\zeta\left(1+\frac{1-2\pi it}{\log D}\right)^{-1}\right|
\ll\frac{1+|t|}{\log D}
$$

and

$$
\left|\zeta\left(1+\frac{2-2\pi i(t_1+t_2)}{\log D}\right)\right|
\ll\frac{\log D}{1+|t_1+t_2|}+O(\log(2+T)).
$$

After multiplication, one net factor $(\log D)^{-1}$ remains. The polynomial factors in $t_1,t_2$ are integrable against the rapidly decreasing $g(t_1)g(t_2)$, and choosing $T$ as a sufficiently large power of $\log D$ makes the tails negligible. Hence

$$
\iint_{\mathbb R^2}|g(t_1)g(t_2)H(t_1,t_2,D)|\,dt_1dt_2
\ll\frac1{\log D}.
$$

Since $D=X^{1/10}$ and $D^2=X^{1/5}\ll X/\log X$,

$$
\boxed{\pi(Y+X)-\pi(Y)\ll\frac X{\log D}\ll\frac X{\log X}.}
$$

This proves the [short-interval prime upper bound from a smooth divisor weight](../../../../../../short-interval-prime-upper-bound-from-a-smooth-divisor-weight.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
