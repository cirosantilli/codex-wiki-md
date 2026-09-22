<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take an affinely parametrized [null geodesic congruence](../../../../../../null-geodesic-congruence.md), $\nabla_kk=0$. Choose the auxiliary [null vector](../../../../../../null-vector.md) and a transverse orthonormal screen basis to undergo [parallel transport](../../../../../../parallel-transport.md) along each ray. For the unprojected tensor $C_{ab}=\nabla_bk_a$, the product rule and the [Ricci identity](../../../../../../curvature-commutator-on-a-covariant-tensor.md) yield

$$
\begin{aligned}
k^c\nabla_cC_{ab}
&=\nabla_b(k^c\nabla_ck_a)-(\nabla_bk^c)(\nabla_ck_a)
+k^c[\nabla_c,\nabla_b]k_a\\
&=-(\nabla_bk^c)(\nabla_ck_a)-R_{acbd}k^ck^d.
\end{aligned}
$$

Here the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) convention is the one in Question 1; its last-index antisymmetry converts the covector commutator to the displayed curvature term. Because $C_{ab}k^a=C_{ab}k^b=0$, inserting the [screen-space projector](../../../../../../screen-space-projector.md) in the product term adds only terms killed by these contractions. Parallel propagation makes differentiation commute with the screen projection. Therefore, in screen indices $A,B$,

$$
\frac{dB_{AB}}{d\lambda}=-B_{AC}B^C{}_B-R_{AcBd}k^ck^d.
$$

This is the optical matrix evolution equation. Its trace has curvature contraction $q^{ab}R_{acbd}k^ck^d=R_{cd}k^ck^d$: the additional terms in $q^{ab}-g^{ab}$ vanish by curvature antisymmetry. Write $B=(\theta/2)q+\sigma+\omega$ using the [null expansion](../../../../../../null-expansion.md), [null shear](../../../../../../null-shear.md), and [null twist](../../../../../../null-twist.md). Symmetric--antisymmetric cross terms have zero trace, $\sigma$ is trace-free, and

$$
\operatorname{tr}(B^2)=\frac12\theta^2+\sigma_{ab}\sigma^{ab}-\omega_{ab}\omega^{ab}.
$$

The minus sign in the last trace comes from $\omega_{ab}=-\omega_{ba}$ and the positive screen metric. Taking the trace therefore derives the [Null Raychaudhuri equation](../../../../../../null-raychaudhuri-equation.md):

$$
\boxed{\frac{d\theta}{d\lambda}=-\frac12\theta^2-\sigma_{ab}\sigma^{ab}+\omega_{ab}\omega^{ab}-R_{ab}k^ak^b.}
$$

For a nonaffine tangent obeying $\nabla_kk=\kappa k$, the same product-rule derivation adds $+\kappa\theta$ on the right; the projected derivative of $\kappa$ multiplies $k_a$ and vanishes. In $D$ dimensions the quadratic [null expansion](../../../../../../null-expansion.md) term is $-\theta^2/(D-2)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
