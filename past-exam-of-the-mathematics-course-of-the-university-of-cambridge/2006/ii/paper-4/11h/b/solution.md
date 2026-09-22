<h1 id="11h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the plain pseudoprime assertion use the [Fermat primality test](../../../../../../fermat-primality-test.md). In the finite [group of units modulo an integer](../../../../../../multiplicative-group-of-integers-modulo-n.md), let

$$
L=\{b\in(\mathbb Z/N\mathbb Z)^\times:b^{N-1}=1\}.
$$

It is the [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md), because the unit group is an [abelian group](../../../../../../abelian-group.md). The given witness makes $L$ a proper [subgroup](../../../../../../subgroup.md). By [Lagrange's theorem for finite groups](../../../../../../lagrange-s-theorem.md), $|L|\le\varphi(N)/2$. Thus at least half of all units fail the test. Removing base one removes a passing base, so among the permitted $1<b<N$ there remain $\varphi(N)-|L|$ failures out of $\varphi(N)-1$ bases, still at least half.

The same argument works for the Euler–Jacobi test: its passing bases form the kernel of $b\mapsto b^{(N-1)/2}(b/N)^{-1}$. One must not assert that strong-test passing bases form a [subgroup](../../../../../../subgroup.md); the kernel argument above concerns the Fermat statement requested here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11H](../../11h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
