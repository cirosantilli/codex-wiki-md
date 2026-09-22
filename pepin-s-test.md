<h1 id="pepin-s-test">Pépin's test</h1>

↑ **Parent:** [Fermat prime](fermat-prime.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pépin's_test)

For $n\geq1$, [Pépin's test](pepin-s-test.md) says that the [Fermat number](fermat-number.md) $F_n$ is a [prime number](prime-number-split.md) exactly when the displayed [modular congruence](modular-congruence.md) holds. [Modular exponentiation](modular-exponentiation.md) evaluates it by [exponentiation by squaring](exponentiation-by-squaring.md) without constructing the enormous ordinary power. The index restriction excludes $F_0=3$, where the base itself is divisible by the candidate.[slide 14](primality-testing-then-and-now-by-carl-pomerance.md)

For a proof outline of sufficiency, any [prime factor](prime-factor.md) $p$ of a passing candidate gives $3$ [multiplicative order](multiplicative-order.md) exactly $F_n-1$, a [power of two](power-of-two.md): its half-power is $-1$, rather than $1$. [Fermat's little theorem](fermat-little-theorem.md) forces $F_n-1\mid p-1$, so $p\geq F_n$, and hence $p=F_n$. Conversely, for a prime candidate, $F_n\equiv5\pmod{12}$; [quadratic reciprocity](quadratic-reciprocity.md) and [Euler's criterion](euler-s-criterion.md) give the required half-power. At $n=1$, the check is $3^2\equiv4=-1\pmod5$.

## ↑ Ancestors (6)

1. [Fermat prime](fermat-prime.md)
2. [Prime number](prime-number-split.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Fermat prime](fermat-prime.md)
- [Pépin's test](pepin-s-test.md)
- [Primality testing: then and now by Carl Pomerance](primality-testing-then-and-now-by-carl-pomerance.md)
