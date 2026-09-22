<h1 id="6e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Suppose $x$ is a [quadratic nonresidue](../../../../../../quadratic-nonresidue.md). On the nonzero [residue classes](../../../../../../residue-class.md) modulo $p$, define the [involution](../../../../../../involution.md)

$$
T(a)=xa^{-1}.
$$

It is an [involution](../../../../../../involution.md) because $T(T(a))=a$. A fixed point would satisfy $a^2=x$, which is excluded by the [quadratic nonresidue](../../../../../../quadratic-nonresidue.md) hypothesis. Thus it partitions the $p-1$ classes into $(p-1)/2$ disjoint pairs $\{a,xa^{-1}\}$, each with product $x$. Consequently

$$
\prod_{a=1}^{p-1}a\equiv x^{(p-1)/2}\pmod p.
$$

Now evaluate the same product by pairing every class with its own [modular inverse](../../../../../../modular-multiplicative-inverse.md). The only classes equal to their [modular inverses](../../../../../../modular-multiplicative-inverse.md) solve $(a-1)(a+1)=0$ and hence are $1$ and $-1$. All other pairs have product one. The complete product is therefore $-1$, so

$$
\boxed{x^{(p-1)/2}\equiv-1\pmod p.}
$$

Together with the preceding part, this is [Euler's criterion](../../../../../../euler-s-criterion.md); the pairing argument establishes the converse without assuming it.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
