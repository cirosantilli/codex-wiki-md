<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

When $u_0=0$, the field theory is a [Gaussian field theory](../../../../../../gaussian-field-theory.md), so integrating out short-wavelength modes can be done exactly rather than merely at a saddle. Introduce an ultraviolet momentum cutoff $\Lambda$ and a scale factor $b>1$, then split $\phi=\phi_<+\phi_>$ into $|q|<\Lambda/b$ and $\Lambda/b<|q|<\Lambda$. Orthogonality of [Fourier modes](../../../../../../fourier-mode.md) eliminates cross terms in the quadratic Hamiltonian. A constant source couples only to the zero-momentum mode and therefore does not couple to $\phi_>$.

Before rescaling, the [Gaussian functional integral](../../../../../../gaussian-functional-integral.md) factorizes:

$$
Z[h]=Z_>(r_0)\int\mathcal D\phi_<\,e^{-H_<[\phi_<,h]},
$$

where $H_<$ has the original $r_0$ and $h$, restricted to low momenta. Up to a field-independent normalization, the eliminated modes contribute

$$
\Delta F_>=\frac12\operatorname{Tr}_>\log(-\nabla^2+r_0).
$$

The determinant affects the additive [free energy](../../../../../../thermodynamic-free-energy.md), but generates neither a mass correction nor a source correction, since no interaction mixes low and high modes. This remains true beyond the [Landau approximation](../../../../../../landau-approximation.md): it is an exact integration of a [Gaussian field theory](../../../../../../gaussian-field-theory.md), not neglect of the high-mode fluctuations.

To restore the original cutoff, use $x=bx'$, $q'=bq$, and choose the field rescaling

$$
\phi'(x')=b^{(D-2)/2}\phi_<(bx').
$$

Substitution into the low-mode Hamiltonian gives the [Gaussian momentum-shell scaling](../../../../../../gaussian-momentum-shell-scaling.md)

$$
H_< =\int d^Dx'\left[
\frac12(\nabla'\phi')^2+\frac12b^2r_0\phi'^2
-b^{(D+2)/2}h\phi'\right].
$$

The [gradient](../../../../../../gradient.md) coefficient is unchanged: the volume factor is $b^D$, the two derivatives contribute $b^{-2}$, and the two fields contribute $b^{2-D}$. The mass term gains $b^2$, while the source term gains $b^{(D+2)/2}$. Thus

$$
\boxed{r_0'=b^2r_0,\qquad h'=b^{(D+2)/2}h,\qquad u_0'=0.}
$$

For a nonconstant source the corresponding formula is $h'(x')=b^{(D+2)/2}h(bx')$, after restricting its coupling to retained modes. The constant-source case avoids that extra source filtering.

Writing $b=e^\ell$, the exact Gaussian [renormalization-group flow](../../../../../../renormalization-group-flow.md) has

$$
\boxed{\frac{dr_0}{d\ell}=2r_0,\qquad
\frac{dh}{d\ell}=\frac{D+2}{2}h.}
$$

Both perturbations are relevant at the massless zero-source [Gaussian fixed point](../../../../../../gaussian-fixed-point.md), with $y_t=2$ and $y_h=(D+2)/2$. There is no anomalous field rescaling here, so $\eta=0$ and the [correlation-length critical exponent](../../../../../../correlation-length-critical-exponent.md) is again $\nu=1/y_t=1/2$. The coefficient changes arise from rescaling, not from an interaction-induced shift in $r_0$ during shell integration.

A stable real [Gaussian functional integral](../../../../../../gaussian-functional-integral.md) requires $r_0>0$, or an infrared prescription that treats the zero mode at the massless point. With $u_0=0$ and $r_0<0$, the field energy is unbounded below; the [Gaussian field theory](../../../../../../gaussian-field-theory.md) alone cannot describe a stable ordered phase. The scaling laws are therefore interpreted about the [Gaussian fixed point](../../../../../../gaussian-fixed-point.md) from the stable side, with finite-volume zero-mode regularization when needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 303](../../../paper-303-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
