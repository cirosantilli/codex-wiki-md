<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Parallel transport](../../../../../../parallel-transport.md) the auxiliary [null vector](../../../../../../null-vector.md) $N$ and a screen basis along each generator of the [null geodesic congruence](../../../../../../null-geodesic-congruence.md). This keeps the [screen-space projector](../../../../../../screen-space-projector.md) fixed under the corresponding transported [derivative](../../../../../../derivative.md). Use the curvature convention $[\nabla_c,\nabla_b]V_a=-R^d{}_{acb}V_d$.

With $B_{ab}=\nabla_bU_a$, differentiation of the affine [geodesic equation](../../../../../../geodesic-equation.md) gives

$$
U^c\nabla_cB_{ab}
=-(\nabla_bU^c)(\nabla_cU_a)-R^d{}_{acb}U^cU_d.
$$

Here the first term comes from commuting the [derivative](../../../../../../derivative.md) past $U^c$, and the second from the curvature commutator. The constraints $B_{ab}U^a=B_{ab}U^b=0$ follow respectively from the null normalization and affine [geodesic equation](../../../../../../geodesic-equation.md). Projecting onto the screen therefore yields the optical [matrix](../../../../../../matrix.md) equation

$$
\frac{D\widehat B_{IJ}}{d\lambda}
=-\widehat B_{IK}\widehat B_{KJ}-\mathcal R_{IJ},\qquad
\mathcal R_{IJ}=R_{acbd}e_I^aU^ce_J^bU^d.
$$

The trace of the tidal [matrix](../../../../../../matrix.md) is $R_{ab}U^aU^b$; extra terms from replacing the screen trace by the [spacetime](../../../../../../spacetime.md) trace vanish by curvature antisymmetry. Taking the trace gives

$$
\frac{d\theta}{d\lambda}=-\operatorname{tr}(\widehat B^2)-R_{ab}U^aU^b.
$$

Decompose the [optical tensor](../../../../../../optical-tensor.md) as $\widehat B=\tfrac12\theta I+\widehat\sigma+\widehat\omega$. The [null shear](../../../../../../null-shear.md) is symmetric and trace-free and the [null twist](../../../../../../null-twist.md) is antisymmetric. Their cross traces vanish, and

$$
\operatorname{tr}(\widehat B^2)
=\frac12\theta^2+\widehat\sigma^{ab}\widehat\sigma_{ab}
-\widehat\omega^{ab}\widehat\omega_{ab}.
$$

The negative sign in the last term is the identity $\operatorname{tr}(\widehat\omega^2)=-\sum_{I,J}\widehat\omega_{IJ}^2$ on the positive-definite screen. Substitution proves the four-dimensional [Null Raychaudhuri equation](../../../../../../null-raychaudhuri-equation.md):

$$
\boxed{\frac{d\theta}{d\lambda}
=-\frac12\theta^2-\widehat\sigma^{ab}\widehat\sigma_{ab}
+\widehat\omega^{ab}\widehat\omega_{ab}-R_{ab}U^aU^b.}
$$

The coefficient is $1/(D-2)$ in $D$ [spacetime](../../../../../../spacetime.md) dimensions; the factor $1/2$ here belongs to the four-dimensional congruence in this question, not the five-dimensional geometry of the next question.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 311](../../../paper-311-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
