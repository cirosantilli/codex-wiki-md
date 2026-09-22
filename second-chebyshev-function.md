# Second Chebyshev function

↑ **Parent:** [Chebyshev function](chebyshev-function.md)

The [Second Chebyshev function](second-chebyshev-function.md) is the [partial sum](partial-sum.md) of the [Von Mangoldt function](von-mangoldt-function.md) up to a real cutoff $x\geq0$:

$$
\psi(x)=\sum_{1\leq n\leq x}\Lambda(n).
$$

For example, $\psi(3)=\log6$, $\psi(4)=\log12$, and $\psi(4.5)=\log12$. At $4=2^2$ the jump has size $\log2$; between $4$ and $5$ no new [prime power](prime-power.md) greater than one enters the sum. In contrast, the [Chebyshev theta function](chebyshev-theta-function.md) stays at $\vartheta(4)=\log6$.

There is also an exact connection with the [least common multiple](least-common-multiple.md). For $N=\lfloor x\rfloor\geq1$, each [prime number](prime-number-split.md) $p\leq N$ occurs to the highest exponent $k$ for which $p^k\leq N$, both in that [least common multiple](least-common-multiple.md) and in the accumulated [Von Mangoldt function](von-mangoldt-function.md) weights. Thus

$$
\psi(x)=\log\operatorname{lcm}(1,2,\ldots,N).
$$

This explains the $\log2520$ value at $x=10$: the [least common multiple](least-common-multiple.md) is $2^3\cdot3^2\cdot5\cdot7$. The [Chebyshev theta function](chebyshev-theta-function.md) instead gives the [natural logarithm](natural-logarithm.md) of the [primorial](primorial.md) $2\cdot3\cdot5\cdot7=210$. The additional [prime powers](prime-power.md) retain the highest required multiplicities.

Why is this useful for the distribution of [prime numbers](prime-number-split.md)? The [Prime number theorem](prime-number-theorem.md) has the equivalent forms

$$
\pi(x)\sim\frac{x}{\log x},\qquad\vartheta(x)\sim x,\qquad\psi(x)\sim x
\quad(x\longrightarrow\infty),
$$

where $\pi$ is the [prime-counting function](prime-counting-function.md) and $\sim$ denotes [asymptotic equivalence](asymptotic-equivalence.md). Thus an [arithmetic function](arithmetic-function-split.md) defined using [prime factorization](fundamental-theorem-of-arithmetic.md) has average weight tending to one over long initial intervals of the [positive integers](positive-integer.md). These are substantive [asymptotic equivalences](asymptotic-equivalence.md), not consequences of the definitions or the [Von Mangoldt divisor identity](von-mangoldt-divisor-identity.md) alone. [254A, Notes 2: Complex-analytic multiplicative number theory](254a-analytic-prime-number-theory/254a-notes-2-complex-analytic-multiplicative-number-theory.md)

The elementary reason the two [Chebyshev functions](chebyshev-function.md) have the same leading behavior is that their difference is small compared with $x$. Every additional [prime power](prime-power.md) has base $p\leq\sqrt x$, and for each such [prime number](prime-number-split.md) its total extra weight is at most $\log x$. There are at most $\lfloor\sqrt x\rfloor$ such bases, so

$$
0\leq\psi(x)-\vartheta(x)\leq\lfloor\sqrt x\rfloor\log x,
\qquad
\frac{\psi(x)-\vartheta(x)}x\longrightarrow0.
$$

This transfers $\psi(x)\sim x$ to $\vartheta(x)\sim x$, or conversely, once either is established. [Partial summation](abel-s-summation-formula.md) then relates the [Chebyshev theta function](chebyshev-theta-function.md) to the [prime-counting function](prime-counting-function.md). The estimate controls the extra [prime powers](prime-power.md); proving the leading value itself is the harder [Prime number theorem](prime-number-theorem.md) problem.

**Table of contents**

- [First integral of the Chebyshev function](first-integral-of-the-chebyshev-function.md)
  - [Smoothed explicit formula for the Chebyshev function](smoothed-explicit-formula-for-the-chebyshev-function.md)
- [Integrated Chebyshev sum](integrated-chebyshev-sum.md)
- [Chebyshev estimate](chebyshev-estimate.md)
  - [Chebyshev estimate from central binomial coefficients](chebyshev-estimate-from-central-binomial-coefficients.md)
- [Riemann–von Mangoldt explicit formula](riemann-von-mangoldt-explicit-formula.md)
  - [Truncated explicit formula for the second Chebyshev function](truncated-explicit-formula-for-the-second-chebyshev-function.md)

## ↑ Ancestors (7)

1. [Chebyshev function](chebyshev-function.md)
2. [Von Mangoldt function](von-mangoldt-function.md)
3. [Arithmetic function](arithmetic-function-split.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Chebyshev estimate from central binomial coefficients](chebyshev-estimate-from-central-binomial-coefficients.md)
- [Chebyshev function](chebyshev-function.md)
- [First integral of the Chebyshev function](first-integral-of-the-chebyshev-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-22/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-28/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25/1/solution.md)
- [Prime number asymptotic from Mertens cancellation](prime-number-asymptotic-from-mertens-cancellation.md)
- [Second Chebyshev function](second-chebyshev-function.md)
- [Von Mangoldt function](von-mangoldt-function.md)
