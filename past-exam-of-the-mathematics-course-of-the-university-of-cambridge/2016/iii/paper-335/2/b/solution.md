<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\mathbf r=R\boldsymbol\theta$, $|\boldsymbol\theta|=1$. Uniformly for $\mathbf r'$ in the source ball,

$$
|\mathbf r-\mathbf r'|=R-\boldsymbol\theta\cdot\mathbf r'+O(r_0^2/R),\qquad
|\mathbf r-\mathbf r'|^{-1}=R^{-1}+O(r_0/R^2).
$$

For fixed $k$ and $r_0$, the [outgoing Green function for the three-dimensional Helmholtz equation](../../../../../../outgoing-green-function-for-the-three-dimensional-helmholtz-equation.md) therefore has the [far-field approximation for an outgoing source](../../../../../../far-field-approximation-for-an-outgoing-source.md)

$$
G_k(R\boldsymbol\theta,\mathbf r')
=\frac{e^{ikR}}{4\pi R}e^{-ik\boldsymbol\theta\cdot\mathbf r'}+O(R^{-2}).
$$

Substitution into the source integral yields

$$
\psi(R\boldsymbol\theta,k)=\frac{e^{ikR}}R f_\infty(\boldsymbol\theta,k)+O(R^{-2}),\qquad
\boxed{f_\infty(\boldsymbol\theta,k)
=-\frac1{4\pi}\int_A Q(\mathbf r')e^{-ik\boldsymbol\theta\cdot\mathbf r'}\,d^3\mathbf r'.}
$$

Thus the [source-to-far-field operator at fixed frequency](../../../../../../source-to-far-field-operator-at-fixed-frequency.md) is

$$
\boxed{T:L^2(A)\longrightarrow L^2(S_1),\qquad
(TQ)(\boldsymbol\theta)=-\frac1{4\pi}\int_AQ(\mathbf r')e^{-ik\boldsymbol\theta\cdot\mathbf r'}\,d^3\mathbf r'.}
$$

It samples the [Fourier transform](../../../../../../fourier-transform.md) of the source on the sphere of radius $k$. Its square-integrable kernel makes it a [Hilbert-Schmidt operator](../../../../../../hilbert-schmidt-operator.md), hence a [compact operator](../../../../../../compact-operator-split.md). In fact

$$
\|T\|_{\rm HS}^2=\frac{|A||S_1|}{16\pi^2}
=\frac{|A|}{4\pi}=\frac{r_0^3}{3}.
$$

Use complex [inner products](../../../../../../inner-product.md) linear in the first argument: $(f,g)=\int f\overline g$. Interchanging the volume and surface integrals gives

$$
(TQ,g)_{L^2(S_1)}
=\int_A Q(\mathbf r')\overline{\left[
-\frac1{4\pi}\int_{S_1}g(\boldsymbol\theta)e^{ik\boldsymbol\theta\cdot\mathbf r'}\,dS(\boldsymbol\theta)\right]}\,d^3\mathbf r'.
$$

Hence **the [adjoint source-to-far-field operator](../../../../../../adjoint-source-to-far-field-operator.md) is**

$$
\boxed{(T^*g)(\mathbf r')=-\frac1{4\pi}\int_{S_1}
g(\boldsymbol\theta)e^{ik\boldsymbol\theta\cdot\mathbf r'}\,dS(\boldsymbol\theta).}
$$

This is a normalized [Herglotz wave function](../../../../../../herglotz-wave-function.md); the change in exponential sign comes from the [complex conjugation](../../../../../../complex-conjugation.md) in the [adjoint operator](../../../../../../adjoint-operator.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
