<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Construct the [Lorentz-spinor generators from a Clifford algebra](../../../../../../lorentz-spinor-generators-from-a-clifford-algebra.md) as

$$
M^{\rho\sigma}=\frac14[\gamma^\rho,\gamma^\sigma]
=\frac12\gamma^\rho\gamma^\sigma-\frac12\eta^{\rho\sigma}I_4.
$$

They are antisymmetric in $\rho,\sigma$. Reordering a third [gamma matrix](../../../../../../gamma-matrices.md) with the [Clifford algebra](../../../../../../clifford-algebra.md) yields

$$
[\gamma^\rho\gamma^\sigma,\gamma^\tau]
=2\eta^{\sigma\tau}\gamma^\rho-2\eta^{\rho\tau}\gamma^\sigma,
\qquad
[M^{\rho\sigma},\gamma^\tau]
=\eta^{\sigma\tau}\gamma^\rho-\eta^{\rho\tau}\gamma^\sigma.
$$

Use the [commutator derivation identity](../../../../../../commutator-derivation-identity.md) on the two factors in $M^{\tau\nu}=\frac14[\gamma^\tau,\gamma^\nu]$:

$$
\begin{aligned}
[M^{\rho\sigma},M^{\tau\nu}]
&=\frac14\left([[M^{\rho\sigma},\gamma^\tau],\gamma^\nu]
+[\gamma^\tau,[M^{\rho\sigma},\gamma^\nu]]\right)\\
&=\eta^{\sigma\tau}M^{\rho\nu}-\eta^{\rho\tau}M^{\sigma\nu}
+\eta^{\rho\nu}M^{\sigma\tau}-\eta^{\sigma\nu}M^{\rho\tau}.
\end{aligned}
$$

This derives every [Lorentz algebra](../../../../../../lorentz-algebra.md) commutation relation, so **the matrices $M^{\rho\sigma}$ form its spinor representation**. Their finite exponentials describe the connected [Spinor representation of the Lorentz group](../../../../../../spinor-representation-of-the-lorentz-group.md), more precisely the lift to its double cover.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
