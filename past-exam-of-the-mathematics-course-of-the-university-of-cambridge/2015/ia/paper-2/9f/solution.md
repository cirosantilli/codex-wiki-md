<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

Let $N=a+b$ and measure Lionel's fortune in unit stakes. This is [gambler's ruin](../../../../../gambler-s-ruin.md): the fortune moves by $+1$ with probability $p$ and $-1$ with probability $q$, stopping at $0$ or $N$. Let $m_i$ be the [expected value](../../../../../expected-value.md) of the absorption time starting at $i$. It is finite: from any interior state, a run of $N$ wins or losses has a fixed positive probability of absorption within $N$ steps, giving a geometric bound on survival over successive blocks. [First-step analysis](../../../../../first-step-analysis.md) therefore gives

$$
m_i=1+pm_{i+1}+qm_{i-1},\qquad m_0=m_N=0.
$$

For $p\ne q$, the [homogeneous solution](../../../../../homogeneous-solution.md) of the recurrence is $A+B(q/p)^i$, and a [particular solution](../../../../../particular-solution.md) is $-i/(p-q)$. Put $\rho=q/p$. Imposing the two endpoint [boundary conditions](../../../../../boundary-condition.md) gives the [expected duration of biased gambler's ruin](../../../../../expected-duration-of-biased-gambler-s-ruin.md)

$$
m_i=\frac{N(1-\rho^i)/(1-\rho^N)-i}{p-q}.
$$

Consequently **the expected number of games is**

$$
\boxed{\mathbb E[T]=\frac{(a+b)\dfrac{1-(q/p)^a}{1-(q/p)^{a+b}}-a}{p-q}.}
$$

The denominator and numerator have matching signs, so this is positive. As a check its continuous limit at $p=q=1/2$ is $a b$, the [expected duration of symmetric gambler's ruin](../../../../../expected-duration-of-symmetric-gambler-s-ruin.md).

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
