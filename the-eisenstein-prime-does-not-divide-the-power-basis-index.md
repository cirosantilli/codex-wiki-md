# The Eisenstein prime does not divide the power-basis index

↑ **Parent:** [Integral basis](integral-basis.md)

Let $f=X^n+a_{n-1}X^{n-1}+\cdots+a_0\in\mathbb Z[X]$ satisfy [Eisenstein's criterion](eisenstein-criterion.md) at a [prime number](prime-number-split.md) $p$, and let $\theta$ be a root. Then

$$
p\nmid[\mathcal O_{\mathbb Q(\theta)}:\mathbb Z[\theta]].
$$

Indeed, $\theta^n/p$ is an [algebraic integer](algebraic-integer.md), whereas for $p\nmid r$ and $0\le i<n$ the [field norm](field-norm.md) of $r\theta^i/p$ has $p$-adic valuation $i-n<0$, so that element is not integral. If $\gamma=p^{-1}\sum_{i=0}^{n-1}r_i\theta^i$ is integral, multiply it by $\theta^{n-1}$. Every term except $r_0\theta^{n-1}/p$ is integral; thus $p\mid r_0$. Subtract $r_0/p$, multiply the remainder by $\theta^{n-2}$, and continue to obtain $p\mid r_i$ for every $i$. Hence there is no element of order $p$ in the finite group $\mathcal O_{\mathbb Q(\theta)}/\mathbb Z[\theta]$, proving the claim. The result concerns the Eisenstein prime only: other primes may still divide the index.

## ↑ Ancestors (6)

1. [Integral basis](integral-basis.md)
2. [Algebraic number theory](algebraic-number-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
