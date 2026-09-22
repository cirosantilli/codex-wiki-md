<h1 id="1i/solution">Solution</h1>

↑ **Parent:** [1I](../1i.md)

[Euler's criterion](../../../../../euler-s-criterion.md) states that for an odd [prime number](../../../../../prime-number.md) $p$ and $p\nmid a$,

$$
\boxed{
a^{(p-1)/2}\equiv\left(\frac ap\right)\pmod p
},
$$

where the right-hand side is the [Legendre symbol](../../../../../legendre-symbol.md).

Let $g$ be a [primitive root](../../../../../primitive-root-modulo-n.md) modulo $p$. Its [multiplicative order](../../../../../multiplicative-order.md) is $p-1$, so $g^{(p-1)/2}\ne1$. This power has square $g^{p-1}=1$, and the only roots of $X^2-1$ modulo the odd prime $p$ are $\pm1$. Therefore

$$
g^{(p-1)/2}\equiv-1\pmod p.
$$

Euler's criterion now gives $(g/p)=-1$, so every primitive root is a [quadratic nonresidue](../../../../../quadratic-nonresidue.md).

Now let $p=2^{2^k}+1$ be a [Fermat prime](../../../../../fermat-prime.md), with $k\geq1$. The number of primitive roots modulo $p$ is

$$
\varphi(p-1)
=\varphi\left(2^{2^k}\right)
=2^{2^k-1}
=\frac{p-1}{2}.
$$

There are also exactly $(p-1)/2$ quadratic nonresidues. Since every primitive root is a nonresidue, these equally large sets coincide. Thus every quadratic nonresidue modulo $p$ is a primitive root, as summarized by [Quadratic nonresidues modulo a Fermat prime](../../../../../quadratic-nonresidues-modulo-a-fermat-prime.md).

Finally, $p\equiv1\pmod4$ and $p\equiv2\pmod3$. [Quadratic reciprocity](../../../../../quadratic-reciprocity.md) therefore gives

$$
\left(\frac3p\right)
=\left(\frac p3\right)
=\left(\frac23\right)
=-1.
$$

Hence $3$ is a quadratic nonresidue modulo $p$, and consequently

$$
\boxed{3\text{ is a primitive root modulo every Fermat prime }p
\text{ with }k\geq1}.
$$

## ↑ Ancestors (10)

1. [1I](../1i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
