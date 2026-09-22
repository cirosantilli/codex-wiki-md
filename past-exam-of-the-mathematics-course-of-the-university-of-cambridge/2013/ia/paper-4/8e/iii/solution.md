<h1 id="8e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [finite prime-power Teichmuller representative](../../../../../../finite-prime-power-teichmuller-representative.md) has an explicit description. Let $y$ be the unique least nonnegative residue satisfying

$$
\boxed{y\equiv x^{p^{n-1}}\pmod{p^n}.}
$$

Repeated [Fermat's little theorem](../../../../../../fermat-little-theorem.md) gives $y\equiv x\pmod p$. Part (ii) gives

$$
y^p\equiv x^{p^n}\equiv x^{p^{n-1}}\equiv y\pmod{p^n},
$$

so this residue has both required properties.

For uniqueness, suppose $z$ also has them. From $z^p\equiv z\pmod{p^n}$, raising congruences to the $p$th power repeatedly gives $z^{p^j}\equiv z\pmod{p^n}$ for every $j\geq0$. Meanwhile $z\equiv x\pmod p$ and the lifting result with $r=n-1$ imply

$$
z^{p^{n-1}}\equiv x^{p^{n-1}}\pmod{p^n}.
$$

Hence $z\equiv y\pmod{p^n}$. Both lie between zero and $p^n-1$, so $z=y$. Thus **existence and uniqueness hold for every residue class, including zero**, without needing a general [Hensel lemma](../../../../../../hensel-s-lemma.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [8E](../../8e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
