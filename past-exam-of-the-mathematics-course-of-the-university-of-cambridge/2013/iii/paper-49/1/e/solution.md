<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Expand $T=T^\mu{}_{\nu}\,\partial_\mu\otimes dx^\nu$. Using the [tensor Lie derivative](../../../../../../lie-derivative-of-a-tensor-field.md) of functions, vectors and covectors and its [Leibniz rule](../../../../../../leibniz-rule.md) gives

$$
\boxed{(\mathcal L_XT)^\mu{}_{\nu}
=X^\rho\partial_\rho T^\mu{}_{\nu}
-T^\rho{}_{\nu}\partial_\rho X^\mu
+T^\mu{}_{\rho}\partial_\nu X^\rho.}
$$

The contravariant slot has a minus sign and the covariant slot a plus sign.

For the [commutator identity for Lie derivatives](../../../../../../commutator-identity-for-lie-derivatives.md), put $D=[\mathcal L_X,\mathcal L_Y]-\mathcal L_{[X,Y]}$. The commutator of two [tensor derivations](../../../../../../tensor-derivation.md) is itself a [tensor derivation](../../../../../../tensor-derivation.md), and $D$ commutes with [tensor contractions](../../../../../../tensor-contraction.md). On a function, $Df=XYf-YXf-[X,Y]f=0$. On a [vector field](../../../../../../vector-field.md) $Z$,

$$
DZ=[X,[Y,Z]]-[Y,[X,Z]]-[[X,Y],Z]=0
$$

by the [Jacobi identity](../../../../../../jacobi-identity.md), which follows here by expanding the commutators of the operators $X,Y,Z$ acting on functions. For a type $(1,1)$ tensor, $T(Z)$ is a [vector field](../../../../../../vector-field.md), and contraction compatibility gives

$$
0=D(T(Z))=(DT)(Z)+T(DZ)=(DT)(Z).
$$

As this holds for every $Z$, $DT=0$. Therefore

$$
\boxed{\mathcal L_X\mathcal L_YT-\mathcal L_Y\mathcal L_XT=\mathcal L_{[X,Y]}T.}
$$

The derivation argument also establishes the identity for arbitrary tensor types by applying it to covector–vector pairings and then to [tensor products](../../../../../../tensor-product.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
