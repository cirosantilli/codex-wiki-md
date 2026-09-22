<h1 id="11i/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Factor $n=\prod_jq_j^{e_j}$. Since it is not a square, one exponent, say $e_1$, is odd. Choose a nonzero [quadratic nonresidue](../../../../../../quadratic-nonresidue.md) $a$ modulo $q_1$; one exists because the squaring map on the nonzero residues is two-to-one and hence has only $(q_1-1)/2$ images. The [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) supplies a positive odd [integer](../../../../../../integer.md) $m>1$ satisfying

$$
m\equiv1\pmod4,\qquad m\equiv a\pmod{q_1},\qquad m\equiv1\pmod{q_j}\quad(j>1).
$$

Then $\gcd(m,n)=1$ and $(m/n)=(-1)^{e_1}=-1$. The [Jacobi reciprocity law](../../../../../../jacobi-reciprocity-law.md) proved in part (i), together with $m\equiv1\pmod4$, gives $(n/m)=-1$. Factoring $m=\prod_\ell p_\ell^{r_\ell}$ gives

$$
-1=\left(\frac nm\right)=\prod_\ell\left(\frac n{p_\ell}\right)^{r_\ell}.
$$

All $p_\ell$ are odd and none divides $n$. At least one factor must be negative, yielding **an odd [prime number](../../../../../../prime-number.md) $\boxed{p\text{ with }(n/p)=-1}$**. No theorem about primes in arithmetic progressions is needed.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11I](../../11i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
