# Multiplication by a unit permutes reduced residues

↑ **Parent:** [Euler's theorem](euler-s-theorem.md)

Choose a [reduced residue system](reduced-residue-system.md) $u_1,\ldots,u_{\varphi(n)}$. For a [unit modulo n](unit-modulo-n.md) $a$, the [bijection](bijection.md) $u\mapsto au$ on the [unit group](unit-group.md) has inverse $u\mapsto a^{-1}u$. Comparing products before and after this [permutation](permutation.md) gives

$$
P=\prod_{i=1}^{\varphi(n)}u_i
\equiv\prod_{i=1}^{\varphi(n)}(au_i)
=a^{\varphi(n)}P\pmod n.
$$

The product $P$ is a [unit](unit-in-a-ring.md); its [modular inverse](modular-multiplicative-inverse.md) cancels it, proving [Euler's theorem](euler-s-theorem.md). Merely being nonzero would not justify cancellation.[pp. 2–3, Section 2: permutation of the units, comparison of products, cancellation](euler%E2%80%99s-theorem-by-keith-conrad.md)

In the modulo-twelve example, $P=1\cdot5\cdot7\cdot11=385\equiv1\pmod{12}$. The permuted representatives $5,1,11,7$ have the same product, while the unreduced products $(5\cdot1)(5\cdot5)(5\cdot7)(5\cdot11)$ equal $5^4P$. Equating these products modulo twelve exposes the fourth power without calculating it directly. Using all nonzero [congruence classes](congruence-class.md) instead would include [nonunits](nonunit.md), whose product need not permit cancellation.

## ↑ Ancestors (5)

1. [Euler's theorem](euler-s-theorem.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
