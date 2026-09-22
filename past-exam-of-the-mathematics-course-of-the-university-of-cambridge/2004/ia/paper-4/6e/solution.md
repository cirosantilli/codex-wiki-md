<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

For a [prime number](../../../../../prime-number.md) $p$ and an [integer](../../../../../integer.md) $x$ [coprime](../../../../../coprime-integers.md) to $p$, multiplication by $x$ permutes the nonzero residue classes modulo $p$. Indeed, $ax\equiv bx\pmod p$ implies $a\equiv b\pmod p$, and none of the products is zero. Taking the product over the $p-1$ classes gives

$$
x^{p-1}(p-1)!\equiv(p-1)!\pmod p.
$$

The [factorial](../../../../../factorial.md) is [coprime](../../../../../coprime-integers.md) to $p$ and can be cancelled, proving [Fermat little theorem](../../../../../fermat-little-theorem.md): $\boxed{x^{p-1}\equiv1\pmod p}$.

Now $n=mp$ and $x$ is [coprime](../../../../../coprime-integers.md) to $n$, so it is [coprime](../../../../../coprime-integers.md) to $p$. Since $(n-1)-(m-1)=m(p-1)$, the proved theorem gives

$$
x^{n-1}=x^{m-1}(x^{p-1})^m\equiv x^{m-1}\pmod p.
$$

Thus the two specified [integer congruences](../../../../../integer-congruence.md) modulo $p$ are equivalent. In this particular step the additional hypothesis $(m,p)=1$ is not needed; it will hold for the squarefree factorization used next.

If $n$ is a [squarefree integer](../../../../../squarefree-integer.md), its distinct [prime factors](../../../../../prime-factor.md) are pairwise [coprime](../../../../../coprime-integers.md). Consequently $n$ divides $x^{n-1}-1$ exactly when every [prime factor](../../../../../prime-factor.md) does. Applying the preceding equivalence with $m=n/p$ proves

$$
\boxed{x^{n-1}\equiv1\pmod n\quad\Longleftrightarrow\quad
x^{(n/p)-1}\equiv1\pmod p\text{ for every }p\mid n.}
$$

Finally retain this squarefree hypothesis. If $p-1$ divides $n-1$, write $n-1=k_p(p-1)$. [Fermat little theorem](../../../../../fermat-little-theorem.md) gives $x^{n-1}=(x^{p-1})^{k_p}\equiv1\pmod p$ for every [prime factor](../../../../../prime-factor.md). Their pairwise coprimality then gives $\boxed{x^{n-1}\equiv1\pmod n}$. For composite $n$ this is the sufficient direction of the [Korselt criterion](../../../../../korselt-criterion.md) for a [Carmichael number](../../../../../carmichael-number.md); primality is not excluded by the requested implication.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
