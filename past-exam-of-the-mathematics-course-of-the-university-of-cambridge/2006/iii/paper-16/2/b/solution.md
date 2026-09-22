<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the integer [degree of a map between oriented manifolds](../../../../../../degree-of-a-map-between-oriented-manifolds.md) be $d\ne0$, so $f_*[X]=d[Y]$. For any nonzero $\alpha\in H^k(Y;\mathbb Q)$, nondegeneracy of the [Poincare duality pairing](../../../../../../poincare-duality-pairing.md) supplies $\gamma\in H^{n-k}(Y;\mathbb Q)$ with $\langle\alpha\smile\gamma,[Y]\rangle\ne0$. Naturality of the [cup product](../../../../../../cup-product.md) and its evaluation gives

$$
\langle f^*\alpha\smile f^*\gamma,[X]\rangle=\langle\alpha\smile\gamma,f_*[X]\rangle=d\langle\alpha\smile\gamma,[Y]\rangle\ne0.
$$

Thus $f^*\alpha\ne0$, proving injectivity of pullback on rational [cohomology](../../../../../../cohomology-split.md). By the [universal coefficient theorem for cohomology](../../../../../../universal-coefficient-theorem-for-cohomology.md), these finite-dimensional rational [cohomology](../../../../../../cohomology-split.md) groups are the duals of the corresponding [homology](../../../../../../homology-split.md) groups, and the dual of $f_*$ is $f^*$. Injectivity of the dual map therefore proves

$$
\boxed{f_*:H_k(X;\mathbb Q)\twoheadrightarrow H_k(Y;\mathbb Q)\quad\text{for every }k.}
$$

One can see the surjection constructively. Given $u\in H_k(Y;\mathbb Q)$, choose its [Poincare dual](../../../../../../poincare-dual.md) $\eta\in H^{n-k}(Y;\mathbb Q)$ with $\eta\cap[Y]=u$. Then $v=d^{-1}(f^*\eta\cap[X])$ satisfies $f_*v=d^{-1}(\eta\cap f_*[X])=u$ by [naturality of the cap product](../../../../../../naturality-of-the-cap-product.md). Division by $d$ is the reason rational coefficients suffice.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
