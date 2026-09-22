<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the symmetric metric perturbation $h^{\alpha\beta}$ be varied with compact support. Integrating the mixed derivative product by parts makes its integral equal to that of $A_\sigma A^\sigma$. Thus the supplied [massless Fierz-Pauli action](../../../../../../../massless-fierz-pauli-action.md) has, up to a boundary term, density

$$
\mathcal L=-\frac14\partial_\mu h^{\rho\sigma}\partial^\mu h_{\rho\sigma}
+\frac12A_\sigma A^\sigma
-\frac12A^\nu\partial_\nu h
+\frac14\partial_\mu h\partial^\mu h.
$$

For example, the equivalence of the mixed term follows from commuting flat-space partial derivatives after moving one derivative off $h^{\rho\sigma}$. Here $\delta h=\eta_{\alpha\beta}\delta h^{\alpha\beta}$ and $\delta A^\nu=\partial_\mu\delta h^{\mu\nu}$.

Integrating each variation by parts, the four terms contribute respectively

$$
\begin{aligned}
\delta S=\int d^4x\,\delta h^{\alpha\beta}\bigg[
&\frac12\Box h_{\alpha\beta}
-\frac12(\partial_\alpha A_\beta+\partial_\beta A_\alpha)\\
&+\frac12\partial_\alpha\partial_\beta h
+\frac12\eta_{\alpha\beta}\partial_\mu A^\mu
-\frac12\eta_{\alpha\beta}\Box h\bigg].
\end{aligned}
$$

The symmetrization in the second term is required because the varied field is symmetric. Comparing this coefficient with the [Einstein tensor](../../../../../../../einstein-tensor.md) perturbation above gives

$$
\boxed{\delta S=-\int d^4x\,\delta h^{\alpha\beta}\delta G_{\alpha\beta}.}
$$

Thus arbitrary compactly supported variations give **$\delta G_{\alpha\beta}=0$**, exactly the vacuum [Linearized Einstein equations](../../../../../../../linearized-einstein-equations.md). The minus sign and overall normalization of the action do not change those equations; boundary conditions justify the discarded total derivatives.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 50](../../../../paper-50-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
