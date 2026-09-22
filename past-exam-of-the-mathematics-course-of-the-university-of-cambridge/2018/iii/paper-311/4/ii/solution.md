<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In [Minkowski spacetime](../../../../../../minkowski-spacetime.md) with signature $(-+++)$, $p\cdot x=-\omega_{\mathbf p}t+\mathbf p\cdot\mathbf x$, where $\omega_{\mathbf p}=p^0=\sqrt{|\mathbf p|^2+m^2}>0$. Hence $i\partial_t\psi_{\mathbf p}=\omega_{\mathbf p}\psi_{\mathbf p}$: these are [positive-frequency solutions](../../../../../../positive-frequency-solution.md) relative to the inertial time translation.

On a constant-time [Cauchy hypersurface](../../../../../../cauchy-surface.md), the [Klein-Gordon inner product](../../../../../../klein-gordon-inner-product.md) and the spatial [Fourier transform](../../../../../../fourier-transform.md) identity give

$$
(\psi_{\mathbf p},\psi_{\mathbf q})=
\frac{\omega_{\mathbf p}+\omega_{\mathbf q}}{2\sqrt{\omega_{\mathbf p}\omega_{\mathbf q}}}
 e^{i(\omega_{\mathbf p}-\omega_{\mathbf q})t}\delta^3(\mathbf p-\mathbf q)
=\delta^3(\mathbf p-\mathbf q).
$$

Also $(\overline\psi_{\mathbf p},\overline\psi_{\mathbf q})=-\delta^3(\mathbf p-\mathbf q)$ and $(\psi_{\mathbf p},\overline\psi_{\mathbf q})=0$: the latter is proportional to $(\omega_{\mathbf p}-\omega_{\mathbf q})\delta^3(\mathbf p+\mathbf q)$, which vanishes. This is the [Klein-Gordon plane-wave normalization](../../../../../../klein-gordon-plane-wave-normalization.md).

For completeness, spatial Fourier transformation of the field equation gives $\ddot{\widehat\Phi}(t,\mathbf p)+\omega_{\mathbf p}^2\widehat\Phi(t,\mathbf p)=0$. Its solutions have the two branches $e^{\mp i\omega_{\mathbf p}t}$. Selecting the positive-frequency branch leaves precisely the Fourier superpositions of $\psi_{\mathbf p}$. These plane waves form a generalized basis, normalized with the [Dirac delta distribution](../../../../../../dirac-delta-function.md), rather than individually normalizable vectors. For a normalizable packet,

$$
\Phi_+(x)=\int d^3p\,c(\mathbf p)\psi_{\mathbf p}(x),\qquad
\boxed{(\Phi_+,\Phi_+)=\int d^3p\,|c(\mathbf p)|^2>0\quad\text{if }c\ne0.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 311](../../../paper-311-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
