<h1 id="5d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Fermat-Euler theorem](../../../../../../euler-s-theorem.md) states that for an [integer](../../../../../../integer.md) $a$ and a positive [integer](../../../../../../integer.md) $n$ with $\gcd(a,n)=1$,

$$
\boxed{a^{\varphi(n)}\equiv1\pmod n,}
$$

where the [Euler totient function](../../../../../../euler-totient-function.md) $\varphi(n)$ counts the [residue classes](../../../../../../residue-class.md) coprime to $n$. For $n\ge2$, choose a [reduced residue system](../../../../../../reduced-residue-system.md) $r_1,\ldots,r_{\varphi(n)}$. Multiplication by the [unit modulo n](../../../../../../unit-modulo-n.md) $a$ preserves coprimality and is injective on these [residue classes](../../../../../../residue-class.md): $ar_i\equiv ar_j\pmod n$ implies $r_i\equiv r_j\pmod n$, because $a$ has a [multiplicative inverse](../../../../../../multiplicative-inverse.md) modulo $n$. It therefore permutes the [reduced residue system](../../../../../../reduced-residue-system.md), giving

$$
a^{\varphi(n)}\prod_i r_i\equiv\prod_i r_i\pmod n.
$$

The product is also a [unit modulo n](../../../../../../unit-modulo-n.md), so it can be cancelled. This proves the [Fermat-Euler theorem](../../../../../../euler-s-theorem.md). For $n=1$ every [modular congruence](../../../../../../modular-congruence.md) is automatic; one may use $\varphi(1)=1$.

For a [prime number](../../../../../../prime-number.md) $p$, the [Euler totient function](../../../../../../euler-totient-function.md) has value $\varphi(p)=p-1$. Thus $a^{p-1}\equiv1\pmod p$ whenever $p\nmid a$. Multiplying by $a$, and treating $p\mid a$ separately, gives the all-integer version of [Fermat's little theorem](../../../../../../fermat-little-theorem.md):

$$
\boxed{a^p\equiv a\pmod p\quad\text{for every integer }a.}
$$

Finally, [Wilson theorem](../../../../../../wilson-s-theorem.md) states that for every [prime number](../../../../../../prime-number.md) $p$, $\boxed{(p-1)!\equiv-1\pmod p}$. Its converse is also true: an [integer](../../../../../../integer.md) $n>1$ is prime exactly when $(n-1)!\equiv-1\pmod n$. For the converse, any proper divisor $1<d<n$ would divide both $(n-1)!$ and $n$, contradicting that congruence.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5D](../../5d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
