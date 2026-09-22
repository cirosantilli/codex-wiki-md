<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply the [Abelian group criterion for a product of two prime squares](../../../../abelian-group-criterion-for-a-product-of-two-prime-squares.md) with the smaller and larger primes in their correct order. For $p<11$, all such [groups](../../../../group-split.md) are [Abelian](../../../../abelian-group.md) exactly when $p\nmid11^2-1=120$. Of the primes $2,3,5,7$, only $7$ qualifies. For $p>11$, the criterion is $11\nmid p^2-1$, equivalently $p\not\equiv\pm1\pmod{11}$. Therefore the exact answer is

$$
\boxed{p=7\quad\text{or}\quad p>11\text{ prime with }p\not\equiv1,10\pmod{11}.}
$$

Equivalently, among the stipulated primes $p\ne11$, exclude $2,3,5$ and the residue classes $\pm1$ modulo $11$.

For completeness, the necessity in that criterion supplies actual counterexamples at every excluded prime. If $\ell<q$ and $\ell\mid q^2-1$, the [multiplicative group of a finite field is cyclic](../../../../multiplicative-group-of-a-finite-field-is-cyclic.md), so choose $\alpha\in\mathbb F_{q^2}^{\times}$ of order $\ell$. Let a generator of $C_{\ell^2}$ act on the additive [group](../../../../group-split.md) of $\mathbb F_{q^2}$ by multiplication by $\alpha$. This defines a nontrivial [group action](../../../../group-action-split.md), hence a nonabelian [semidirect product](../../../../semidirect-product.md) of order $\ell^2q^2$. Use $(\ell,q)=(p,11)$ for $p=2,3,5$, and $(\ell,q)=(11,p)$ for $p\equiv\pm1\pmod{11}$ with $p>11$. Thus no excluded prime can be restored to the answer.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
