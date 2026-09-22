<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $n=3g-3$. To specify the [Abel map of an algebraic curve](../../../../../../abel-map-of-an-algebraic-curve.md) into $X=\operatorname{Pic}^{g-1}(C)$, use

$$
\alpha(z_1,\ldots,z_n)=\left[\sum_{j=1}^n z_j-K_C\right].
$$

The canonical-class twist is necessary: an untwisted sum has degree $3g-3$, rather than $g-1$. Let $L=\mathcal O_C(2K_C)$. The [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) and [Serre duality](../../../../../../serre-duality.md) give $h^0(L)=n$ and $h^1(L)=0$.

On $C\times C^n$, write $\Gamma_i$ for the graph of the $i$th coordinate, $\mathcal D=\sum_i\Gamma_i$, and $\pi$ for projection to $C^n$. The locally free sheaf $E_L=\pi_*(L|_{\mathcal D})$ has rank $n$; at repeated points it records values and jets. Evaluation gives a morphism of rank-$n$ [vector bundles](../../../../../../vector-bundle.md)

$$
H^0(C,L)\otimes\mathcal O_{C^n}\longrightarrow E_L.
$$

Its kernel at a tuple is $H^0(C,2K_C-\sum z_j)$. By the [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md), this space has the same dimension as $H^0(C,\sum z_j-K_C)$, since both [line bundles](../../../../../../line-bundle.md) have degree $g-1$. Thus its [determinant](../../../../../../determinant.md) vanishes exactly along $\alpha^*\Theta$. This is also an equality of [Cartier divisors](../../../../../../cartier-divisor-split.md) with multiplicities: the evaluation complex computes the [sheaf cohomology](../../../../../../sheaf-cohomology.md) of $L(-\mathcal D)$; [Serre duality](../../../../../../serre-duality.md) identifies its determinant equation, up to an invertible factor, with the defining theta evaluation equation for $K_C\otimes L^{-1}(\mathcal D)$.

To calculate the determinant line, set $\mathcal D_i=\Gamma_1+\cdots+\Gamma_i$. Restriction to the extra graph gives

$$
0\longrightarrow L|_{\Gamma_i}\otimes\mathcal O_{\Gamma_i}(-\mathcal D_{i-1})\longrightarrow L|_{\mathcal D_i}\longrightarrow L|_{\mathcal D_{i-1}}\longrightarrow0.
$$

Projection is exact on these finite relative divisors. On $\Gamma_i\cong C^n$, the first term is $\operatorname{pr}_i^*L\otimes\mathcal O(-\sum_{j<i}\Delta_{ij})$, where $\Delta_{ij}=\{z_i=z_j\}$. Taking [determinants](../../../../../../determinant.md) inductively yields the [evaluation determinant on a product of curves](../../../../../../evaluation-determinant-on-a-product-of-curves.md):

$$
\det E_L\cong\bigotimes_i\operatorname{pr}_i^*L\otimes\mathcal O\left(-\sum_{i<j}\Delta_{ij}\right).
$$

The determinant of the fixed space $H^0(C,L)$ contributes only a constant line. Therefore

$$
\boxed{\alpha^*\Theta\sim2\sum_{i=1}^{3g-3}\operatorname{pr}_i^*K_C-\sum_{i<j}\Delta_{ij}.}
$$

The diagonal subtraction is essential: ordinary evaluation [determinants](../../../../../../determinant.md) vanish when columns coincide, whereas restriction to a repeated-point [Cartier divisor](../../../../../../cartier-divisor-split.md) uses jets. The restriction exact sequences account for those factors in every characteristic.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
