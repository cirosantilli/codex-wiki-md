<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Retain $a=p_0^{1/\gamma}/\rho_0$ from part (b), and use time translation invariance to write $G(\mathbf x,t;\mathbf y,\tau)=g(\mathbf x,\mathbf y;t-\tau)$. Define the temporal [Fourier transform](../../../../../../fourier-transform.md) by

$$
\widetilde G(\mathbf x,\mathbf y;\omega)=\int_{\mathbb R}g(\mathbf x,\mathbf y;s)e^{-i\omega s}\,ds.
$$

Multiplying the transformed [Green function](../../../../../../green-s-function.md) equation by $-a(\mathbf x)$ gives

$$
\nabla\cdot(a\nabla\widetilde G)+\frac{a\omega^2}{c_0^2}\widetilde G
=-a(\mathbf y)\delta(\mathbf x-\mathbf y).
$$

This is a symmetric divergence-form spatial operator, although the original unweighted operator need not be symmetric in the ordinary volume measure.

Let $G_j(\mathbf x)=\widetilde G(\mathbf x,\mathbf y_j;\omega)$. The product rule gives the bilinear [Green second identity](../../../../../../green-second-identity.md)

$$
\nabla\cdot\{a(G_1\nabla G_2-G_2\nabla G_1)\}
=G_1\nabla\cdot(a\nabla G_2)-G_2\nabla\cdot(a\nabla G_1).
$$

The frequency terms cancel. Integrating over the domain, the right side becomes

$$
-a(\mathbf y_2)\widetilde G(\mathbf y_2,\mathbf y_1;\omega)
+a(\mathbf y_1)\widetilde G(\mathbf y_1,\mathbf y_2;\omega).
$$

The boundary integral is zero for common homogeneous [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md), [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) or reciprocal [Robin boundary condition](../../../../../../robin-boundary-condition.md) conditions. In an unbounded domain, use the same outgoing limiting-absorption prescription for both [Green functions](../../../../../../green-s-function.md); it gives the corresponding vanishing boundary pairing. This identity has no complex conjugation: it proves transpose [wave reciprocity](../../../../../../wave-reciprocity.md), not a Hermitian or time-reversal identity. We obtain the [weighted acoustic Green-function reciprocity](../../../../../../weighted-acoustic-green-function-reciprocity.md)

$$
\widetilde G(\mathbf y_1,\mathbf y_2;\omega)
=\frac{a(\mathbf y_2)}{a(\mathbf y_1)}\widetilde G(\mathbf y_2,\mathbf y_1;\omega).
$$

The factor is frequency independent, so inverse [Fourier transform](../../../../../../fourier-transform.md) gives the same relation at equal time lag. Both time arguments below have lag $t-\tau_2$, hence

$$
\boxed{G(\mathbf y_1,t;\mathbf y_2,\tau_2)
=G(\mathbf y_2,t+\tau_1-\tau_2;\mathbf y_1,\tau_1)
\frac{[p_0(\mathbf y_2)]^{1/\gamma}\rho_0(\mathbf y_1)}{[p_0(\mathbf y_1)]^{1/\gamma}\rho_0(\mathbf y_2)}.}
$$

Reciprocity exchanges source and receiver while preserving elapsed time; it does not turn a causal response into an advanced one.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
