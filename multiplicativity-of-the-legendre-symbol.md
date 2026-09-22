# Multiplicativity of the Legendre symbol

↑ **Parent:** [Legendre symbol](legendre-symbol.md)

For an [odd prime](odd-prime.md) $p$ and any [integers](integer-split.md) $a,b$, the [Legendre symbol](legendre-symbol.md) obeys

$$
\left(\frac{ab}{p}\right)=
\left(\frac ap\right)\left(\frac bp\right).
$$

In particular, if $p\nmid a$, then $(a^{-1}/p)=(a/p)$, where $a^{-1}$ is a [modular multiplicative inverse](modular-multiplicative-inverse.md). Multiplication by a nonzero square also leaves the [Legendre symbol](legendre-symbol.md) unchanged: $(ar^2/p)=(a/p)$ for $p\nmid r$.[Ben Lynn, Quadratic Residues, The Legendre Symbol: multiplicativity and invariance under a nonzero square factor](quadratic-residues-by-ben-lynn.md)

The [subgroup](subgroup.md) and [coset](coset.md) arguments under [quadratic residue](quadratic-residue-split.md) and [quadratic nonresidue](quadratic-nonresidue.md) prove the sign rule without computing a large power: square times square is square, square times nonsquare is nonsquare, and nonsquare times nonsquare is square. If either factor is zero modulo $p$, both sides of the identity vanish. On $\mathbb F_p^\times$, the [Legendre symbol](legendre-symbol.md) is thus a [group homomorphism](group-homomorphism.md) to $\{1,-1\}$ whose [kernel of a group homomorphism](kernel-of-a-group-homomorphism.md) is the [quadratic residue](quadratic-residue-split.md) [subgroup](subgroup.md). Viewed on all [integers](integer-split.md), it is a [completely multiplicative function](completely-multiplicative-function.md) and a [Dirichlet character](dirichlet-character.md) modulo $p$.

<a id="image-products-modulo-seven-the-legendre-symbol-reduces-a-six-by-six-table-to-sign-multiplication"></a>
![](quadratic-residue-character-product-table.png)

**[Figure 2](#image-products-modulo-seven-the-legendre-symbol-reduces-a-six-by-six-table-to-sign-multiplication). Products modulo seven: the Legendre symbol reduces a six-by-six table to sign multiplication**. Rows and columns put [quadratic residues](quadratic-residue-split.md) $1,2,4$ before [quadratic nonresidues](quadratic-nonresidue.md) $3,5,6$. Every cell displays the product modulo seven and its [Legendre symbol](legendre-symbol.md). The four blocks have signs $+1,-1,-1,+1$, showing the [subgroup](subgroup.md) and its other [coset](coset.md).

For an original calculation, factor the numerator $30=2\cdot3\cdot5$. Modulo seven, $(30/7)=(2/7)(3/7)(5/7)=1\cdot(-1)\cdot(-1)=1$, agreeing with $30\equiv2\pmod7$. Modulo eleven, the signs are instead $-1,1,1$, giving $(30/11)=-1$, agreeing with $30\equiv8\pmod{11}$. The same factorization can therefore certify different square behavior at different [prime numbers](prime-number-split.md).

Alternatively, [Euler's criterion](euler-s-criterion.md) gives $(ab)^{(p-1)/2}\equiv a^{(p-1)/2}b^{(p-1)/2}$ modulo $p$. For nonzero factors both sides correspond to signs in $\{1,-1\}$. Since $p$ is odd, these signs are distinct modulo $p$, so the [modular congruence](modular-congruence.md) proves the asserted equality of [integers](integer-split.md), not merely an equality of representatives.

## ↑ Ancestors (6)

1. [Legendre symbol](legendre-symbol.md)
2. [Quadratic residue](quadratic-residue-split.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Computing Legendre symbols by quadratic reciprocity](computing-legendre-symbols-by-quadratic-reciprocity.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/17g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/17g/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/1g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/11h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/11h/iii/solution.md)
- [Quadratic nonresidue](quadratic-nonresidue.md)
