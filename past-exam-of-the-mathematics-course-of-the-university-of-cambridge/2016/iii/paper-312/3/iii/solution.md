<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose the arbitrary normalization of the complex [plane wave](../../../../../../plane-wave.md) polarization so that $h_{ij}=u_iu_jh(\eta)e^{ikz}$ with $\mathbf u=(1,i,0)$. For $\mathbf e=(\sin\theta\cos\varphi,\sin\theta\sin\varphi,\cos\theta)$, contraction gives

$$
(u_ie^i)^2=\sin^2\theta\,e^{2i\varphi}.
$$

At the observer origin, write $\mu=\cos\theta$. The [tensor CMB line-of-sight source](../../../../../../tensor-cmb-line-of-sight-source.md) is

$$
\Theta(\mathbf e)=-\frac12\sin^2\theta\,e^{2i\varphi}\int_{\eta_*}^{\eta_0}\dot h(\eta)e^{-ik(\eta_0-\eta)\mu}\,d\eta.
$$

The rest of the expression is independent of $\varphi$. Projection onto $Y_{\ell m}^*\propto e^{-im\varphi}$ therefore gives zero unless $m=2$. This is the [helicity selection for tensor CMB multipoles](../../../../../../helicity-selection-for-tensor-cmb-multipoles.md). It applies to the specified complex helicity mode; taking a physical real field also introduces the conjugate mode and its conjugate azimuthal dependence.

For the very long wavelength solution during matter domination, differentiation gives $\dot h=-h_{\mathrm{prim}}k^2\eta/5+O(k^4\eta^3)$. Expand the [plane wave](../../../../../../plane-wave.md) factor once to obtain

$$
\Theta=\frac{h_{\mathrm{prim}}k^2}{10}\sin^2\theta e^{2i\varphi}[A_0-ik\mu A_1]+O(h_{\mathrm{prim}}k^4\eta_0^4),
$$

where

$$
A_0=\frac{\eta_0^2-\eta_*^2}{2},\qquad A_1=\frac{\eta_0^3}{6}-\frac{\eta_0\eta_*^2}{2}+\frac{\eta_*^3}{3}.
$$

Let $\mathcal N_{22}=\tfrac14\sqrt{15/(2\pi)}$. Then $Y_{22}=\mathcal N_{22}\sin^2\theta e^{2i\varphi}$ and $Y_{32}=\sqrt7\mathcal N_{22}\mu\sin^2\theta e^{2i\varphi}$. Reading off the [long-wavelength tensor CMB quadrupole and octupole](../../../../../../long-wavelength-tensor-cmb-quadrupole-and-octupole.md) yields

$$
\Theta_{22}=\frac{h_{\mathrm{prim}}k^2A_0}{10\mathcal N_{22}},\qquad\frac{\Theta_{32}}{\Theta_{22}}=-\frac{ik}{\sqrt7}\frac{A_1}{A_0}.
$$

In the limit $\eta_*/\eta_0\to0$,

$$
\boxed{\Theta_{22}=\frac{h_{\mathrm{prim}}}{20\mathcal N_{22}}(k\eta_0)^2+O((k\eta_0)^4),\qquad\Theta_{32}=-\frac{i}{3\sqrt7}(k\eta_0)\Theta_{22}+O((k\eta_0)^5).}
$$

A perfectly frozen tensor produces no redshift; the first contribution comes from its order-$k^2\eta^2$ evolution. The extra spatial phase makes the octupole one power of $k\eta_0$ smaller than the quadrupole.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
