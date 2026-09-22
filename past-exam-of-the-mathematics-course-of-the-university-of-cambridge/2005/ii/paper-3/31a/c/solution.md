<h1 id="31a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\Psi=\mu e^{-i(kx+2k^2t)\sigma}$. The [Lax pair](../../../../../../lax-pair.md) becomes $\Psi_x=U\Psi$, $\Psi_t=V\Psi$, with

$$
U=-ik\sigma+Q,\qquad V=-2ik^2\sigma+2kQ-i(Q^2+Q_x)\sigma.
$$

Equality of mixed derivatives, using invertibility, gives the [zero-curvature condition](../../../../../../zero-curvature-condition.md) $U_t-V_x+[U,V]=0$. The terms quadratic in $k$ cancel. The terms linear in $k$ cancel because $\sigma Q=-Q\sigma$, $\sigma Q_x=-Q_x\sigma$ and $Q^2$ commutes with $\sigma$. For the constant term, the identities

$$
[Q,Q^2\sigma]=2Q^3\sigma,\qquad
[Q,Q_x\sigma]=(QQ_x+Q_xQ)\sigma
$$

cancel the differentiated $Q^2$ term, leaving $Q_t+iQ_{xx}\sigma-2iQ^3\sigma=0$. Multiplying by $i$ proves

$$
\boxed{iQ_t-Q_{xx}\sigma_3+2Q^3\sigma_3=0.}
$$

Once $S$ is known, its time dependence enters through the explicit exponential conjugation. The boundary relation and normalization form a linear problem for $\mu$, and $Q=i[\sigma,\mu_1]$ reconstructs the nonlinear solution. This is the requested linearization. Its disadvantage as an initial-value method is that it does not itself determine $S$ from a prescribed $Q(x,0)$. The [inverse scattering transform](../../../../../../inverse-scattering-transform.md) supplies that direct-scattering step, including any discrete spectral data and their [pole](../../../../../../pole.md) conditions, before reconstruction. Solvability cannot be inferred merely from writing an arbitrary jump.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [31A](../../31a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
