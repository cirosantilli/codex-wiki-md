<h1 id="pollard-s-p-1-algorithm">Pollard's p-1 algorithm</h1>

↑ **Parent:** [Integer factorization](integer-factorization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pollard's_p_−_1_algorithm)

For an [integer](integer-split.md) $n$ to be factored, [John Pollard](john-pollard-mathematician.md)'s method chooses an [integer](integer-split.md) $a$ [coprime](coprime-integers.md) to $n$ and an [exponent](exponent.md) $M$ divisible by many small [prime powers](prime-power.md). Compute $d=\gcd(a^M-1,n)$ by [modular exponentiation](modular-exponentiation.md) and the [Euclidean algorithm](euclidean-algorithm.md). If $1<d<n$, it is a proper [factor](regression-factor.md). If a [prime divisor](prime-factor.md) $p$ of $n$ has $p-1\mid M$, [Fermat's little theorem](fermat-little-theorem.md) ensures $p\mid d$; success requires some other [prime divisor](prime-factor.md) not to divide $a^M-1$. Common choices are $M=B!$ and $M=\operatorname{lcm}(1,\ldots,B)$. The method exploits a smooth $p-1$, rather than a small [factor](regression-factor.md) $p$ itself.

## ↑ Ancestors (5)

1. [Integer factorization](integer-factorization.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-short-options-course-of-the-university-of-oxford/2015/1/b/solution.md)
