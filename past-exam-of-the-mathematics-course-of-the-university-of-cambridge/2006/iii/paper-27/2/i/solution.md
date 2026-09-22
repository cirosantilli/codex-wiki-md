<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Mahler theorem](../../../../../../mahler-s-theorem.md) states that a function $f:\mathbb Z_p\to\mathbb Q_p$ is continuous if and only if it has a unique expansion

$$
f(x)=\sum_{n\ge0}c_n\binom xn,\qquad c_n\in\mathbb Q_p,\quad c_n\longrightarrow0,
$$

and the expansion converges uniformly. Moreover $\|f\|_\infty=\sup_n|c_n|_p$; in particular $f$ takes values in $\mathbb Z_p$ exactly when all $c_n$ belong to $\mathbb Z_p$. Here $\binom{x}{0}=1$ and $\binom{x}{n}=x(x-1)\cdots(x-n+1)/n!$. These [binomial polynomials](../../../../../../binomial-polynomial.md) are continuous and integer-valued on $\mathbb Z_p$, since they are integer-valued on the dense nonnegative integers. The coefficient condition $c_n\to0$ therefore makes the series uniformly convergent.

Evaluate at a nonnegative integer $m$. Terms with $n>m$ vanish, giving the finite triangular relation $f(m)=\sum_{n=0}^m\binom mn c_n$. [Binomial inversion](../../../../../../binomial-inversion.md) gives the [Mahler coefficients](../../../../../../mahler-coefficient.md)

$$
\boxed{c_n=\sum_{j=0}^n(-1)^{n-j}\binom njf(j)=(\Delta^nf)(0),\qquad\Delta f(x)=f(x+1)-f(x).}
$$

To obtain the generating function, multiply the last finite identity by $T^n/n!$ and compare coefficients. Setting $n=j+k$ yields

$$
\sum_{n\ge0}\frac{c_n}{n!}T^n=\sum_{j,k\ge0}\frac{(-1)^k f(j)}{j!k!}T^{j+k}=\boxed{e^{-T}\sum_{j\ge0}\frac{f(j)}{j!}T^j.}
$$

The [Mahler coefficient exponential generating function](../../../../../../mahler-coefficient-exponential-generating-function.md) is an identity in $\mathbb Q_p[[T]]$: each coefficient is a finite sum. It does not assert convergence for every $p$-adic substitution for $T$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
