# Elementary primorial bound

↑ **Parent:** [Primorial](primorial.md)

For every real $X\geq1$,

$$
P(X)\leq4^X.
$$

For integer $n$, strong induction proves this by splitting according to parity. If $n=2k$, every prime in $(k,2k]$ divides $\binom{2k}{k}$, so

$$
P(2k)\leq P(k)\binom{2k}{k}\leq4^k4^k.
$$

If $n=2k+1$, the [valuation of a near-central binomial coefficient](valuation-of-a-near-central-binomial-coefficient.md) gives

$$
P(2k+1)\leq P(k+1)\binom{2k+1}{k+1}\leq4^{k+1}4^k.
$$

The binomial estimates follow from the binomial theorem; in the odd case the two equal central coefficients together are at most $2^{2k+1}$. The result for real $X$ follows by replacing $X$ with $\lfloor X\rfloor$.

## ↑ Ancestors (5)

1. [Primorial](primorial.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4/11g/c/solution.md)
