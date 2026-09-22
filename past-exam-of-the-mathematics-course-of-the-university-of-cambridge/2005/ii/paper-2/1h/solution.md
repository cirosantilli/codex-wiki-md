<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

Let $g$ generate the [cyclic group](../../../../../cyclic-group.md) of nonzero residues, whose order $p-1=2^{2^n}$ is a power of two. Write $a=g^j$. Its [multiplicative order](../../../../../multiplicative-order.md) is $(p-1)/\gcd(j,p-1)$, so it is a [primitive root](../../../../../primitive-root-modulo-n.md) precisely when $j$ is odd. The [quadratic residues](../../../../../quadratic-residue.md) are exactly the even powers of $g$. Thus **the primitive roots are precisely the quadratic nonresidues**, with nonzero [residue](../../../../../residue.md) classes understood.

For $n\geq1$, $p\equiv1\pmod4$, so [quadratic reciprocity](../../../../../quadratic-reciprocity.md) gives $(7/p)=(p/7)$. Since $2^3\equiv1\pmod7$ and $2^n$ alternates between $1$ and $2$ modulo three, $p$ is respectively $3$ or $5$ modulo seven. The nonzero squares modulo seven are $1,2,4$. Consequently $(7/p)=-1$, and

$$
\boxed{7\text{ is a primitive root modulo every Fermat prime }2^{2^n}+1\text{ with }n\geq1.}
$$

There is a genuine endpoint exception if the printed form permits $n=0$: then $p=3$ and $7\equiv1\pmod3$, which has order one and is not primitive. The first equivalence remains true for $p=3$, but the final assertion requires excluding that prime.

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
