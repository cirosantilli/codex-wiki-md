<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the PDF's convention in which $C$ multiplies $\psi^*$, rather than $\bar\psi^T$. Its unitarity converts the given [gamma matrix](../../../../../../gamma-matrices.md) identity into

$$
\gamma^\mu C=-C(\gamma^\mu)^*.
$$

Applying it twice gives

$$
M^{\rho\sigma}C
=\frac14[\gamma^\rho,\gamma^\sigma]C
=C\frac14[(\gamma^\rho)^*,(\gamma^\sigma)^*]
=C(M^{\rho\sigma})^*.
$$

For real infinitesimal [Lorentz transformation](../../../../../../lorentz-transformation.md) parameters,

$$
C\left(I+\frac12\Omega_{\rho\sigma}M^{\rho\sigma}\right)^*
=\left(I+\frac12\Omega_{\rho\sigma}M^{\rho\sigma}\right)C.
$$

Therefore **$\psi^c=C\psi^*$ transforms in exactly the same spinor representation as $\psi$**. The coordinate pullback is real and transforms identically as well. This is the [antilinear charge-conjugation intertwiner](../../../../../../antilinear-charge-conjugation-intertwiner.md) relation; exponentiating also gives $CS^*=SC$ for connected transformations.

For real mass, complex conjugation of the free [Dirac equation](../../../../../../dirac-equation.md) gives $(-i\gamma^{\mu*}\partial_\mu-m)\psi^*=0$. Multiply by $C$ and move it through the [gamma matrices](../../../../../../gamma-matrices.md):

$$
0=C(-i\gamma^{\mu*}\partial_\mu-m)\psi^*
=(i\gamma^\mu\partial_\mu-m)C\psi^*.
$$

Thus

$$
\boxed{(i\gamma^\mu\partial_\mu-m)\psi^c=0.}
$$

As an explicit check, in the given [Weyl representation of the gamma matrices](../../../../../../weyl-representation-of-the-gamma-matrices.md) one may take $C=i\gamma^2$. It is unitary and obeys the required conjugation identity. The free-equation conclusion does not assert that a charge-conjugated field retains the same charge in a fixed electromagnetic background.

## ↑ Ancestors (11)

1. [D](../d.md)
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
