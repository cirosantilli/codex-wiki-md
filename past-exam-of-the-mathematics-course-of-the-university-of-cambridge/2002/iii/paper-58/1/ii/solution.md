<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At the double threshold, $L\psi_0=L\psi_1=0$. For $j\ge2$, $q_j^2\ge9\pi^2/4$, so $|K^*-q_j^2|\ge13\pi^2/8>3\pi^2/8$ and every remaining [eigenvalue](../../../../../../eigenvalue.md) is strictly negative. There is a [spectral gap](../../../../../../spectral-gap.md) separating this two-dimensional kernel from the stable modes. The [centre manifold theorem](../../../../../../centre-manifold-theorem.md) therefore gives a two-dimensional state [centre manifold](../../../../../../center-manifold.md), with

$$
\psi=A\psi_0+B\psi_1+h(A,B),\qquad h=O((|A|+|B|)^2),\qquad \langle h,\psi_j\rangle=0\quad(j=0,1).
$$

If the two detuning parameters are adjoined as variables with zero time derivatives, the extended [centre manifold](../../../../../../center-manifold.md) has total dimension four; its state fibers still have dimension two.

The only nontrivial spatial [symmetry](../../../../../../symmetry-physics.md) of the bounded interval is the [reflection](../../../../../../reflection-mathematics.md) $x\mapsto-x$. Since $\psi_0$ is even and $\psi_1$ odd, its [group action](../../../../../../group-action.md) on the amplitudes is $(A,B)\mapsto(A,-B)$. Thus [equivariance](../../../../../../equivariant-map.md) requires $\dot A$ to be even and $\dot B$ odd in $B$. There is no sign symmetry $\psi\mapsto-\psi$, because the quadratic nonlinearity breaks it. The general smooth form is $\dot A=F(A,B^2)$, $\dot B=B G(A,B^2)$, with the zero solution preserved. The [quadratic even-odd mode interaction](../../../../../../quadratic-even-odd-mode-interaction.md) follows on truncation:

$$
\dot A=\lambda_1A+a_1A^2+a_2B^2+O(3),\qquad
\dot B=\lambda_2B+a_3AB+O(3).
$$

Writing $m=\mu-\mu^*$ and $\kappa=K-K^*$, the exact linear growth rates are $m-3\pi^2\kappa/4-\kappa^2$ and $m+3\pi^2\kappa/4-\kappa^2$. To first order in detuning,

$$
\boxed{\lambda_1=m-\frac{3\pi^2}{4}\kappa,\qquad \lambda_2=m+\frac{3\pi^2}{4}\kappa.}
$$

The [orthogonal projection](../../../../../../orthogonal-projection.md) of the quadratic term onto the neutral [eigenfunctions](../../../../../../eigenfunction.md) determines the leading coefficients. Both [eigenfunctions](../../../../../../eigenfunction.md) have squared $L^2$ norm one, and parity kills the unwanted products. The quadratic correction $h$ contributes no term through $Lh$, since $L$ is [self-adjoint](../../../../../../self-adjoint-operator.md) and the projected modes lie in its kernel. Consequently

$$
a_1=\int_{-1}^1\psi_0^3\,dx,\qquad
a_2=\int_{-1}^1\psi_0\psi_1^2\,dx,\qquad
a_3=2\int_{-1}^1\psi_0\psi_1^2\,dx.
$$

These projections are also a concrete way of computing the [normal form](../../../../../../normal-form-dynamical-systems.md). In this normalization they give $a_1=8/(3\pi)$, $a_2=32/(15\pi)$ and $a_3=64/(15\pi)$, consistent with the stated coefficient ratios.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
