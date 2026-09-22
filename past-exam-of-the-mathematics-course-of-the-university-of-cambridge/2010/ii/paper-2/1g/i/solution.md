<h1 id="1g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $h=(p-1)/2$. The nonzero [quadratic residues](../../../../../../quadratic-residue.md) in the [finite field](../../../../../../finite-field.md) $\mathbb F_p$ form a [subgroup](../../../../../../subgroup.md) of size $h$: the [group homomorphism](../../../../../../group-homomorphism.md) $x\mapsto x^2$ has [kernel](../../../../../../kernel-of-a-linear-map.md) $\{1,-1\}$. Each square satisfies $u^h=1$ by [Fermat's little theorem](../../../../../../fermat-little-theorem.md). Since a nonzero [polynomial](../../../../../../polynomial-split.md) of degree $h$ has at most $h$ [roots of a polynomial](../../../../../../root-of-a-polynomial.md), these are all the roots of $X^h-1$. For any other nonzero $u$, Fermat's theorem gives $(u^h)^2=1$, so $u^h=-1$. Thus [Euler's criterion](../../../../../../euler-s-criterion.md) follows, and multiplication gives

$$
\chi(mn)\equiv (mn)^h=m^hn^h\equiv\chi(m)\chi(n)\pmod p.
$$

Both sides are $1$ or $-1$, which are distinct modulo the odd [prime number](../../../../../../prime-number.md) $p$, so **$\chi(mn)=\chi(m)\chi(n)$.** Taking $n=-1$ in [Euler's criterion](../../../../../../euler-s-criterion.md) gives **$\chi(-1)=(-1)^{(p-1)/2}$**, which is $1$ for $p\equiv1\pmod4$ and $-1$ for $p\equiv3\pmod4$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1G](../../1g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
