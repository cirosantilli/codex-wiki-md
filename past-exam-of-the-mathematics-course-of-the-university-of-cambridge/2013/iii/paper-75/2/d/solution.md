<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [bosonic Bogoliubov diagonalization](../../../../../../bosonic-bogoliubov-diagonalization.md) with $A_k=2JS$, $B_k=2JS\gamma_k$. Away from the zero modes, let

$$
a_k=u_k\alpha_k+v_k\alpha_{-k}^\dagger,\qquad
u_k=\sqrt{\frac{A_k/\omega_k+1}{2}},\qquad
v_k=-\operatorname{sgn}(B_k)\sqrt{\frac{A_k/\omega_k-1}{2}},\qquad
\omega_k=\sqrt{A_k^2-B_k^2}.
$$

Here $u_k^2-v_k^2=1$ preserves the [canonical commutation relations](../../../../../../canonical-commutation-relation.md), while the sign of $v_k$ cancels anomalous pairing. In hyperbolic notation $u_k=\cosh\theta_k$, $v_k=\sinh\theta_k$, this condition is $\tanh(2\theta_k)=-B_k/A_k$. Combining the [normal ordering](../../../../../../normal-ordering.md) constants gives

$$
\boxed{H=-NJS(S+1)+\sum_k\omega_k(\alpha_k^\dagger\alpha_k+1/2)+O(S^0),\qquad\omega_k=2JS|\sin k|.}
$$

The dispersion vanishes linearly near $k=0$ and $\pi$, with [spin-wave velocity](../../../../../../spin-wave-velocity.md) $2JS$ in unit lattice spacing. The exact zero modes make the Bogoliubov coefficients singular; use a small infrared regulator or a symmetry-selected reference and treat the global rotations separately. A finite transformation at $\omega_k=0$ is not asserted.

On a [hypercubic lattice](../../../../../../cubic-lattice.md) of coordination $z=2d$, the same [hypercubic antiferromagnetic spin-wave dispersion](../../../../../../hypercubic-antiferromagnetic-spin-wave-dispersion.md) uses

$$
\gamma_{\mathbf k}=\frac1d\sum_{j=1}^d\cos k_j,\qquad
\boxed{\omega_{\mathbf k}=2dJS\sqrt{1-\gamma_{\mathbf k}^2}.}
$$

The corresponding constant is $-dNJS(S+1)$, and $\omega_{\mathbf k}\sim2JS\sqrt d\,|\mathbf k|$ near a Goldstone point. Restoring lattice spacing $a$ multiplies this velocity by $a$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
