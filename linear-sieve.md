# Linear sieve

↑ **Parent:** [Number-theoretic sieve](number-theoretic-sieve.md)

A [number-theoretic sieve](number-theoretic-sieve.md) that visits each [composite number](composite-number.md) exactly once, through its [smallest prime factor](smallest-prime-factor.md). Keep a growing list of [prime numbers](prime-number-split.md); for each $i$, generate $ip$ only for stored primes $p\le\operatorname{spf}(i)$. Each composite $m$ has a unique representation $m=\operatorname{spf}(m)(m/\operatorname{spf}(m))$ admitted by this rule, giving $O(N)$ arithmetic updates up to $N$.

## ↑ Ancestors (4)

1. [Number-theoretic sieve](number-theoretic-sieve.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
