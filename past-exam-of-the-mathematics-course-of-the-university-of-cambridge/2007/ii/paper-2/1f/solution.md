<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

Write $p=8k+7$. In [Gauss's lemma](../../../../../gauss-s-lemma-riemannian-geometry.md), for the multiplier 2, precisely the integers $j$ with $p/4<j\le(p-1)/2$ give residues $2j>p/2$. Their number is

$$
\frac{p-1}{2}-\left\lfloor\frac p4\right\rfloor=(4k+3)-(2k+1)=2k+2.
$$

It is even, so the [Legendre symbol](../../../../../legendre-symbol.md) $(2/p)=1$: **2 is a [quadratic residue](../../../../../quadratic-residue.md) modulo $p$.** For completeness, the sign rule follows by replacing those large residues by their negatives; the resulting absolute residues permute $1,\ldots,(p-1)/2$. Multiplying them and cancelling their nonzero product gives $2^{(p-1)/2}\equiv(-1)^{2k+2}=1\pmod p$, equivalent to the residue assertion by [Euler's criterion](../../../../../euler-s-criterion.md).

Now take the prime $p=2q+1$. The condition $q\equiv3\pmod4$ gives $p\equiv7\pmod8$, so $2^q\equiv1\pmod p$. Thus $p$ divides $2^q-1$. For integers $q>3$, $2^q-1>2q+1$ (true at 4 and preserved on increasing $q$), so this divisor is proper and **$2^q-1$ is composite**. At $q=3$, the divisor is the number itself: $2^3-1=2\cdot3+1=7$. The congruence still holds, but it does not establish compositeness.

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
