# Proof of Korselt criterion

↑ **Parent:** [Korselt criterion](korselt-criterion.md)

For sufficiency, let $N$ be composite and squarefree, with $p-1\mid N-1$ for every [prime factor](prime-factor.md) $p$. For any [integer](integer-split.md) $a$ [coprime](coprime-integers.md) to $N$, [Fermat's little theorem](fermat-little-theorem.md) gives $a^{N-1}\equiv1\pmod p$ for every such $p$. Their product is $N$, so the [Chinese remainder theorem](chinese-remainder-theorem.md) gives the required congruence modulo $N$.

For necessity, first rule out a repeated factor. If $N=p^km$ with $k\ge2$ and $\gcd(p,m)=1$, the [Chinese remainder theorem](chinese-remainder-theorem.md) supplies $a\equiv1+p\pmod{p^k}$ and $a\equiv1\pmod m$. This $a$ is [coprime](coprime-integers.md) to $N$. But the [binomial theorem](binomial-theorem.md) gives

$$
a^{N-1}\equiv(1+p)^{N-1}\equiv1+(N-1)p\equiv1-p\not\equiv1\pmod{p^2},
$$

contradicting the [Carmichael number](carmichael-number.md) condition. Hence $N$ is squarefree.

Now choose a [primitive root](primitive-root-modulo-n.md) $g$ modulo a [prime factor](prime-factor.md) $p$. Lift it to a [unit](unit-in-a-ring.md) modulo $N$ by prescribing $a\equiv g\pmod p$ and $a\equiv1\pmod{N/p}$. The [Chinese remainder theorem](chinese-remainder-theorem.md) applies because $N$ is squarefree. The Carmichael congruence implies $g^{N-1}\equiv1\pmod p$. Since $g$ has [multiplicative order](multiplicative-order.md) $p-1$, that order divides $N-1$. This proves the other condition.[Theorem 2 proof, printed p. 2: repeated prime factors, primitive roots and Chinese remainder lifting](carmichael-numbers-and-korselt-s-criterion-by-keith-conrad.md)

## ↑ Ancestors (6)

1. [Korselt criterion](korselt-criterion.md)
2. [Carmichael number](carmichael-number.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-4/7e/solution.md)
