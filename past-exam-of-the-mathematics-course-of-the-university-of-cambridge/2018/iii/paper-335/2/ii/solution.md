<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix a receiver position $\boldsymbol\zeta$ and define $g_{\boldsymbol\zeta}(\mathbf z)=G_L(\boldsymbol\zeta,\mathbf z)$. Choose the two scalar fields in the [Wigner distribution](../../../../../../wigner-distribution.md) to be $u=v=g_{\boldsymbol\zeta}$. [Fourier inversion](../../../../../../fourier-inversion-theorem.md) in the separation variable gives

$$
g_{\boldsymbol\zeta}(\mathbf z)\overline{g_{\boldsymbol\zeta}(\mathbf z')}
=\int_{\mathbb R^2}e^{i\mathbf p\cdot(\mathbf z-\mathbf z')}W[g_{\boldsymbol\zeta},g_{\boldsymbol\zeta}]\left(\frac{\mathbf z+\mathbf z'}2,\mathbf p\right)\,d\mathbf p.
$$

Indeed, substituting the defining [Wigner distribution](../../../../../../wigner-distribution.md) makes the $\mathbf p$ integral a $(2\pi)^2$ [Dirac delta function](../../../../../../dirac-delta-function.md), canceling its normalization and setting the separation equal to $\mathbf z-\mathbf z'$.

Average over the receiver plane, including the [aperture](../../../../../../aperture.md):

$$
\mathcal W_A(\mathbf Z,\mathbf p)=\int_{\mathbb R^2}a(\boldsymbol\zeta)W[g_{\boldsymbol\zeta},g_{\boldsymbol\zeta}](\mathbf Z,\mathbf p)\,d\boldsymbol\zeta.
$$

Then the [receiver-averaged Wigner distribution](../../../../../../receiver-averaged-wigner-distribution.md) represents the back-propagated field as

$$
\boxed{\Psi_B(0,\mathbf z)=\int_{\mathbb R^2}\int_{\mathbb R^2}e^{i\mathbf p\cdot(\mathbf z-\mathbf z')}\mathcal W_A\left(\frac{\mathbf z+\mathbf z'}2,\mathbf p\right)\overline{f(\mathbf z')}\,d\mathbf p\,d\mathbf z'.}
$$

The fast decay of $f$ justifies its use as a test function. For oscillatory [Green functions](../../../../../../green-s-function.md) that are not integrable, the [Wigner distribution](../../../../../../wigner-distribution.md) and its inversion can be understood as [tempered distributions](../../../../../../tempered-distribution.md), or derived with smooth cutoffs before taking their limits.

The printed $W_A$ expression can also be used literally, but its displayed $\mathbf z'$ integral is over source-plane coordinates, not receiver positions. The missing receiver average and source weight can be encoded by choosing vector fields whose channels are the receivers. Let

$$
u(\mathbf z;\boldsymbol\zeta)=a(\boldsymbol\zeta)^{1/2}g_{\boldsymbol\zeta}(\mathbf z),\qquad
v(\mathbf z;\boldsymbol\zeta)=f(\mathbf z)u(\mathbf z;\boldsymbol\zeta).
$$

Contract the receiver channels in the product of the vector fields, so that

$$
u(\mathbf z)v(\mathbf z')^*:=\int_{\mathbb R^2}u(\mathbf z;\boldsymbol\zeta)\overline{v(\mathbf z';\boldsymbol\zeta)}\,d\boldsymbol\zeta
=K_A(\mathbf z,\mathbf z')\overline{f(\mathbf z')}.
$$

With exactly the printed definition

$$
W_A[u,v](\mathbf z,\mathbf p)=\int_{\mathbb R^2}e^{-i\mathbf p\cdot\mathbf z'}W[u,v]\left(\frac{\mathbf z+\mathbf z'}2,\mathbf p\right)\,d\mathbf z',
$$

the same [Fourier inversion](../../../../../../fourier-inversion-theorem.md) now yields the requested compact form

$$
\boxed{\Psi_B(0,\mathbf z)=\int_{\mathbb R^2}e^{i\mathbf p\cdot\mathbf z}W_A[u,v](\mathbf z,\mathbf p)\,d\mathbf p.}
$$

For a finite array, the receiver integral in the contraction is a weighted sum. For a continuous array, these are fields valued in the receiver [Hilbert space](../../../../../../hilbert-space-split.md). An uncontracted vector outer product instead gives a matrix-valued [Wigner distribution](../../../../../../wigner-distribution.md), whose receiver trace must be taken. Thus the printed formula is usable with these choices and this contraction convention, but its phrase “over the plane of the receiver” does not describe the displayed integral.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
