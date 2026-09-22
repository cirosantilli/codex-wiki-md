<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For an odd [prime number](../../../../../prime-number-split.md) $p$, [Euler's criterion](../../../../../euler-s-criterion.md) states that

$$
\boxed{a^{(p-1)/2}\equiv\left(\frac ap\right)\pmod p,}
$$

where the [Legendre symbol](../../../../../legendre-symbol.md) is zero if $p\mid a$, one if $a$ is a nonzero [quadratic residue](../../../../../quadratic-residue-split.md), and minus one otherwise. Including the zero case makes this formulation valid for every [integer](../../../../../integer-split.md) $a$.

Apply [Euler's criterion](../../../../../euler-s-criterion.md) to $a$, $b$, and $ab$. Multiplication in [modular arithmetic](../../../../../modular-arithmetic-split.md) gives

$$
\left(\frac{ab}p\right)\equiv (ab)^{(p-1)/2}
\equiv a^{(p-1)/2}b^{(p-1)/2}
\equiv\left(\frac ap\right)\left(\frac bp\right)\pmod p.
$$

If $p$ divides either factor, both sides are zero. Otherwise both sides belong to $\{-1,1\}$; these two values are distinct modulo the odd [prime number](../../../../../prime-number-split.md) $p$. The congruence is therefore an equality of [integers](../../../../../integer-split.md), proving [multiplicativity of the Legendre symbol](../../../../../multiplicativity-of-the-legendre-symbol.md):

$$
\boxed{\left(\frac{ab}p\right)=\left(\frac ap\right)\left(\frac bp\right).}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
