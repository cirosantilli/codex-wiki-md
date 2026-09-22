<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $\mu$ be the [Möbius function](../../../../../mobius-function.md). Its [Möbius divisor-sum identity](../../../../../mobius-divisor-sum-identity.md) is

$$
\sum_{d\mid n}\mu(d)=\begin{cases}1,&n=1,\\0,&n>1.\end{cases}
$$

Indeed, for $n>1$ the sum is the expansion of $\prod_{p\mid n}(1-1)$; nonsquarefree [divisors](../../../../../divisor.md) contribute zero. Thus, for [arithmetic functions](../../../../../arithmetic-function.md) $a,b$,

$$
\boxed{b(n)=\sum_{d\mid n}a(d)\iff a(n)=\sum_{d\mid n}\mu(d)b(n/d).}
$$

To prove [Möbius inversion](../../../../../mobius-inversion-formula.md), substitute the first formula into the second and collect the coefficient of $a(e)$. It is $\sum_{d\mid n/e}\mu(d)$, which is one for $e=n$ and zero otherwise. Conversely the same [divisor](../../../../../divisor.md) interchange recovers $b$ from the displayed formula for $a$. In [Dirichlet convolution](../../../../../dirichlet-convolution.md) notation this is simply $\mu*\mathbf1=\varepsilon$, where $\varepsilon$ is supported at one.

The [Prime number theorem with classical zero-free-region error](../../../../../prime-number-theorem-with-classical-zero-free-region-error.md) states that some absolute $c>0$ satisfies

$$
\boxed{\Psi(x):=\sum_{n\leq x}\Lambda(n)=x+O\bigl(xe^{-c\sqrt{\log x}}\bigr).}
$$

Here $\Lambda$ is the [Von Mangoldt function](../../../../../von-mangoldt-function.md). An equivalent prime-counting form, after decreasing $c$ if needed, is $\pi(x)=\operatorname{Li}(x)+O(xe^{-c\sqrt{\log x}})$. The contributions of proper [prime powers](../../../../../prime-power.md) are $O(\sqrt x\log^2x)$ and can be absorbed into this error. We use $\Psi$ to keep it distinct from the [Fourier transform](../../../../../fourier-transform.md) appearing in Question 5.

Here is a direct deduction of the requested [Mertens bound from a log-integrable Chebyshev error](../../../../../mertens-bound-from-a-log-integrable-chebyshev-error.md) from the stated [Prime number theorem](../../../../../prime-number-theorem.md). First, the [divisor](../../../../../divisor.md) identity gives

$$
1=\sum_{d\leq x}\mu(d)\left\lfloor\frac xd\right\rfloor,
\qquad \left|\sum_{d\leq x}\frac{\mu(d)}d\right|\leq\frac1x+\frac{\lfloor x\rfloor}{x}\leq2.
$$

Second, the exact [Dirichlet convolution](../../../../../dirichlet-convolution.md) identity

$$
\mu(n)\log n=-(\mu*\Lambda)(n)
$$

follows from $\log=\mathbf1*\Lambda$: multiplication of a [Dirichlet convolution](../../../../../dirichlet-convolution.md) by $\log n$ differentiates its two factors, so applying it to $\mu*\mathbf1=\varepsilon$ and convolving again with $\mu$ gives this formula. Summing it yields

$$
\sum_{n\leq x}\mu(n)\log n=-\sum_{d\leq x}\mu(d)\Psi(x/d)
=-x\sum_{d\leq x}\frac{\mu(d)}d+O\left(x\sum_{d\leq x}\frac{e^{-c\sqrt{\log(x/d)}}}{d}\right).
$$

The last harmonic sum is $O(1)$. To see this without an endpoint approximation, split $x/d$ into dyadic ranges $[2^j,2^{j+1})$. In each range $\sum1/d=O(1)$, and its exponential factor is at most $e^{-c\sqrt{j\log2}}$. Their sum over $j\geq0$ converges. The finitely many terms with $1\leq x/d<2$ obey the same estimate after adjusting the constant in the prime-number-theorem error. Therefore

$$
\sum_{n\leq x}\mu(n)\log n=O(x).
$$

For the [Mertens function](../../../../../mertens-function.md) $M(x)=\sum_{n\leq x}\mu(n)$,

$$
M(x)\log x=\sum_{n\leq x}\mu(n)\log n+\sum_{n\leq x}\mu(n)\log(x/n).
$$

The second sum has absolute value at most $\sum_{n\leq x}\log(x/n)=O(x)$, by an integral comparison or the [Stirling formula](../../../../../stirling-formula.md). Consequently

$$
\boxed{\frac{|M(x)|}{x}\ll\frac1{\log x}\qquad(x\geq2).}
$$

The absolute value in this conclusion is present in the original PDF.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
