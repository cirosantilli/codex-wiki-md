<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix an orientation and a positive [volume form](../../../../../../volume-form.md) $\Omega$. Define the [divergence](../../../../../../divergence.md) by the [Lie derivative](../../../../../../lie-derivative-of-a-differential-form.md)

$$
\mathcal L_F\Omega=(\operatorname{div}_\Omega F)\Omega.
$$

A smooth function is a [flow coboundary](../../../../../../flow-coboundary.md) when it equals $Fu$ for some smooth $u$. Every other positive [volume form](../../../../../../volume-form.md) is $e^h\Omega$ for a smooth $h$. The product rule for the [Lie derivative](../../../../../../lie-derivative-of-a-differential-form.md) gives

$$
\mathcal L_F(e^h\Omega)=e^h\bigl(Fh+\operatorname{div}_\Omega F\bigr)\Omega,
\qquad
\operatorname{div}_{e^h\Omega}F=\operatorname{div}_\Omega F+Fh.
$$

Thus changing the reference [volume form](../../../../../../volume-form.md) changes its [divergence](../../../../../../divergence.md) by a [flow coboundary](../../../../../../flow-coboundary.md). If volume forms of either orientation are allowed, take the logarithm of the absolute ratio on each connected component; multiplying a reference form by a constant sign leaves its divergence unchanged.

If $\operatorname{div}_\Omega F=Fu$, the preceding product rule shows

$$
\mathcal L_F(e^{-u}\Omega)=0.
$$

Conversely, if $e^h\Omega$ is invariant, then $\operatorname{div}_\Omega F=-Fh=F(-h)$ is a [flow coboundary](../../../../../../flow-coboundary.md). Vanishing of the [Lie derivative](../../../../../../lie-derivative-of-a-differential-form.md) is equivalent to flow invariance, since $\partial_t\phi_t^*\Omega=\phi_t^*(\mathcal L_F\Omega)$. Hence

$$
\boxed{\phi_t\text{ preserves a smooth volume form}
\iff\operatorname{div}_\Omega F\text{ is a smooth flow coboundary}.}
$$

The equivalence holds for every choice of reference [volume form](../../../../../../volume-form.md), proving the [invariant volume criterion for a smooth flow](../../../../../../invariant-volume-criterion-for-a-smooth-flow.md). The smoothness requirement matters: a merely measurable transfer function does not give a smooth invariant volume form.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
