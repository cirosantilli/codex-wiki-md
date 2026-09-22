<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

A nonzero residue class $a\pmod p$ is a [quadratic residue](../../../../../quadratic-residue.md) if $a\equiv x^2\pmod p$ for some nonzero $x$. If it is a square, [Fermat's little theorem](../../../../../fermat-little-theorem.md) gives $a^{(p-1)/2}=x^{p-1}\equiv1$. Conversely, the map $x\mapsto x^2$ on the nonzero classes identifies exactly the pairs $\{x,-x\}$, giving $(p-1)/2$ distinct squares. They are all roots of $X^{(p-1)/2}-1$ over the field $\mathbb F_p$; a [polynomial](../../../../../polynomial-split.md) of this degree has at most that many roots. Its roots are therefore precisely the squares. This proves [Euler's criterion](../../../../../euler-s-criterion.md)

$$
\boxed{a\text{ is a nonzero quadratic residue }\iff a^{(p-1)/2}\equiv1\pmod p}.
$$

Applying it to $-1$ gives $\boxed{(-1/p)=1\iff p\equiv1\pmod4}$. The exclusion of $a=0$ is the usual nonzero-residue convention needed for this equivalence.

For distinct odd [primes](../../../../../prime-number.md) $p,q$, [quadratic reciprocity](../../../../../quadratic-reciprocity.md) states

$$
\boxed{\left(\frac pq\right)\left(\frac qp\right)=(-1)^{(p-1)(q-1)/4}}.
$$

Using the multiplicativity of the [Legendre symbol](../../../../../legendre-symbol.md), and the supplementary law $(2/p)=(-1)^{(p^2-1)/8}$,

$$
\left(\frac{73}{127}\right)=\left(\frac{127}{73}\right)
=\left(\frac{54}{73}\right)
=\left(\frac2{73}\right)\left(\frac3{73}\right).
$$

The first factor is $1$ because $73\equiv1\pmod8$; the second is $(73/3)=(1/3)=1$ because the reciprocity sign is positive. Thus $\boxed{73\text{ is a quadratic residue modulo }127}$.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
