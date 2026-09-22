<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use signature $(-,+,+,+)$ and write $h_{ij}$ for the spatial [induced metric](../../../../../../induced-metric.md), $D_i$ for its [spatial covariant derivative](../../../../../../spatial-covariant-derivative.md), and $q^2=h^{ij}D_i\phi D_j\phi$. The negative [shift vector](../../../../../../shift-vector.md) convention gives $n^\mu=N^{-1}(1,N^i)$ and $\Pi=n^\mu\partial_\mu\phi$. Decomposing the [scalar field](../../../../../../scalar-field.md) derivative gives

$$
\partial_\mu\phi=-n_\mu\Pi+D_\mu\phi,\qquad g^{\mu\nu}\partial_\mu\phi\partial_\nu\phi=-\Pi^2+q^2.
$$

Varying the [scalar field](../../../../../../scalar-field.md) matter [action](../../../../../../action.md) with respect to the inverse [metric tensor](../../../../../../metric-tensor.md), including the variation of $\sqrt{-g}$, gives the [stress-energy tensor](../../../../../../stress-energy-tensor.md)

$$
\boxed{T_{\mu\nu}=\partial_\mu\phi\partial_\nu\phi-g_{\mu\nu}\left[\tfrac12g^{\alpha\beta}\partial_\alpha\phi\partial_\beta\phi+V\right].}
$$

Raising both indices gives the requested $T^{\mu\nu}$. Contracting with the [unit normal](../../../../../../unit-normal.md) twice, or once with the [spatial projection tensor](../../../../../../spatial-projection-tensor.md), gives

$$
\boxed{\rho=\tfrac12\Pi^2+\tfrac12q^2+V=N^2T^{00},\qquad \mathcal J_i=-\Pi D_i\phi.}
$$

Projecting both indices of the [stress-energy tensor](../../../../../../stress-energy-tensor.md) onto the spatial hypersurface gives

$$
S_{ij}=D_i\phi D_j\phi+h_{ij}\left(\tfrac12\Pi^2-\tfrac12q^2-V\right),\qquad
\boxed{S=\tfrac32\Pi^2-\tfrac12q^2-3V,\quad \widetilde S_{ij}=D_i\phi D_j\phi-\tfrac13h_{ij}q^2.}
$$

**Two printed identifications require correction.** The [canonical momentum](../../../../../../canonical-momentum.md) of the displayed density is $\pi_\phi=\sqrt h\,\Pi$, not $\Pi$: explicitly $\mathcal L_m=N\sqrt h[\Pi^2/2-q^2/2-V]$ and differentiation with respect to $\dot\phi$ supplies $\sqrt h$. Thus $\Pi$ is the [normal scalar-field momentum](../../../../../../normal-scalar-field-momentum.md). Also, the printed trace-free stress has an extra factor $1/2$ and uses $\delta_{ij}$ where the general spatial [induced metric](../../../../../../induced-metric.md) requires $h_{ij}$. In an orthonormal spatial frame the latter becomes $\delta_{ij}$, but the coefficient is still one. For a gradient $(q,0,0)$ in that frame, direct projection gives $\widetilde S_{11}=2q^2/3$, rather than the printed $q^2/3$. The PDF's energy-density gradient is spatial $\partial_i\phi\partial^i\phi$; the TeX aid's spacetime index there is an OCR defect.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
