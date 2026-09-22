<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Suppress tildes in the normalized equation and let $X=x-vt$. A [Gross–Pitaevskii solitary wave](../../../../../../gross-pitaevskii-solitary-wave.md) stationary in these translating coordinates obeys

$$
\boxed{\nabla^2\psi+(1-|\psi|^2)\psi-2iv\partial_X\psi=0,\qquad
\psi(X,y)\to1\ \text{as }X^2+y^2\to\infty.}
$$

The boundary fixes the bulk [complex argument](../../../../../../argument-complex-analysis.md) and describes a localized disturbance with zero net [vortex](../../../../../../phase-vortex.md) [winding number](../../../../../../winding-number.md); a vortex pair is possible. No extra plane-wave factor is needed when only the coordinates are changed. A full [Galilean transformation](../../../../../../galilean-transformation.md) of the field would additionally change the bulk flow and its [complex argument](../../../../../../argument-complex-analysis.md) convention.

Subtract the uniform background from the [grand potential](../../../../../../grand-potential.md). A convenient dimensionless [energy](../../../../../../energy.md) and the [renormalized momentum of a condensate](../../../../../../renormalized-momentum-of-a-condensate.md) are

$$
\boxed{E=\frac12\int_{\mathbb R^2}\left[|\nabla\psi|^2+\frac12(1-|\psi|^2)^2\right]dX\,dy,}
$$



$$
\boxed{\mathbf p=\frac1{2i}\int_{\mathbb R^2}\left[(\psi^*-1)\nabla\psi-(\psi-1)\nabla\psi^*\right]dX\,dy.}
$$

The subtraction in $\mathbf p$ removes the troublesome background [complex argument](../../../../../../argument-complex-analysis.md) [gradient](../../../../../../gradient.md). In particular, for the usual subsonic localized far field $\psi-1=O(r^{-1})$, $\nabla\psi=O(r^{-2})$, and $1-|\psi|^2=O(r^{-2})$, the [energy density](../../../../../../energy-density.md) is $O(r^{-4})$ and the [momentum](../../../../../../momentum.md) integrand is $O(r^{-3})$, both integrable in two dimensions. Merely writing $\psi\to1$ without sufficient decay is not by itself a convergence proof. The common solitary-wave branch is subsonic: linearizing this normalization gives $\omega^2=k^2/2+k^4/4$ and [speed of sound](../../../../../../speed-of-sound.md) $1/\sqrt2$.

[Integration by parts](../../../../../../integration-by-parts.md), with decaying variations and their boundary terms vanishing, gives

$$
\frac{\delta E}{\delta\psi^*}=-\frac12\nabla^2\psi+\frac12(|\psi|^2-1)\psi,
\qquad \frac{\delta p_x}{\delta\psi^*}=-i\partial_X\psi.
$$

Thus the translating equation is precisely $\delta(E-vp_x)=0$. Along a differentiable family $\psi_\lambda$ with fixed bulk normalization, evaluate this stationarity on $\partial_\lambda\psi$ to obtain

$$
\frac{dE}{d\lambda}=v\frac{dp_x}{d\lambda},\qquad
\boxed{\frac{dE}{dp_x}=v}
$$

where $dp_x/d\lambda\ne0$. This [energy–momentum slope of a solitary wave](../../../../../../energy-momentum-slope-of-a-solitary-wave.md) does not require differentiating the [Lagrange multiplier](../../../../../../lagrange-multiplier.md) $v$ inside the field variation. At a turning point the parametrized identity remains true, while $E$ need not be a single-valued function of $p_x$ locally. The chosen factors make $i\psi_t=\delta E/\delta\psi^*$, consistent with the normalized equation; changing the normalization of $E$ alone would change the claimed slope.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
