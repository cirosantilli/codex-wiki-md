<h1 id="9d/solution">Solution</h1>

↑ **Parent:** [9D](../9d.md)

Use the position-space [momentum operator](../../../../../momentum-operator.md) $P_j=-i\hbar\partial_j$ and set $F=(x+iy)z$. Direct differentiation gives

$$
L_zF=-i\hbar(x\partial_y-y\partial_x)F=-i\hbar(ix-y)z=\hbar F.
$$

To compute the squared [orbital angular momentum](../../../../../orbital-angular-momentum.md), write $D_x=y\partial_z-z\partial_y$, $D_y=z\partial_x-x\partial_z$, $D_z=x\partial_y-y\partial_x$, so $L_j=-i\hbar D_j$. Expanding the products, including derivatives of their variable coefficients, gives

$$
D_x^2+D_y^2+D_z^2=r^2\Delta-E^2-E,\qquad E=x\partial_x+y\partial_y+z\partial_z.
$$

For example $D_x^2=y^2\partial_z^2+z^2\partial_y^2-2yz\partial_y\partial_z-y\partial_y-z\partial_z$; summing the three cyclic expressions proves the identity.

Here $\Delta F=0$ and $EF=2F$, so $E^2F=4F$. Therefore

$$
\boxed{\mathbf L^2F=6\hbar^2F,\qquad L_zF=\hbar F}.
$$

This is the [angular momentum of a homogeneous harmonic polynomial](../../../../../angular-momentum-of-a-homogeneous-harmonic-polynomial.md), with angular quantum numbers $\ell=2,m=1$. The polynomial is a nonzero angular [eigenfunction](../../../../../eigenfunction.md); by itself it is not a normalizable full-space [wavefunction](../../../../../wave-function.md).

## ↑ Ancestors (10)

1. [9D](../9d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
