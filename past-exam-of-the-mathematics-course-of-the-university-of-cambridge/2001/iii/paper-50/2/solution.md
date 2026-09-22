<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let the perturbation [velocity](../../../../../velocity.md) and [pressure](../../../../../pressure.md) be $(u,w,p)(z)e^{ik(x-ct)}$, with real $k>0$. Linearizing the [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) about the [inviscid parallel shear flow](../../../../../inviscid-parallel-shear-flow.md) gives

$$
ik(U-c)u+U'w=-ikp/\rho_0,\qquad ik(U-c)w=-p'/\rho_0,\qquad iku+w'=0.
$$

Use $u=\phi'$, $w=-ik\phi$ to satisfy [incompressibility](../../../../../incompressible-flow.md). The first momentum equation gives $p/\rho_0=-(U-c)\phi'+U'\phi$; differentiate it and use the second equation. The [Rayleigh equation for inviscid shear flow](../../../../../rayleigh-equation-for-inviscid-shear-flow.md) follows:

$$
\boxed{(U-c)(\phi''-k^2\phi)-U''\phi=0,\qquad \phi\to0\quad(z\to\pm\infty).}
$$

A growing temporal [normal mode](../../../../../normal-mode.md) has $c_i=\operatorname{Im}c>0$ and growth rate $kc_i$.

[Rayleigh's inflection-point theorem](../../../../../rayleigh-s-inflection-point-theorem.md) states that such an instability of a smooth parallel profile requires $U''$ to change sign somewhere. To prove it, divide by $U-c$, multiply by $\phi^*$, integrate over $z$ and integrate the second derivative by parts. Decay removes the endpoint terms, giving

$$
\int_{-\infty}^\infty(|\phi'|^2+k^2|\phi|^2)\,dz+\int_{-\infty}^\infty\frac{U''}{U-c}|\phi|^2\,dz=0.
$$

Taking the imaginary part yields

$$
c_i\int_{-\infty}^\infty\frac{U''|\phi|^2}{(U-c_r)^2+c_i^2}\,dz=0.
$$

The weighting is nonnegative. A one-signed $U''$ that is not identically zero cannot satisfy this identity for a nontrivial mode; otherwise the mode vanishes on an interval and uniqueness of the differential equation forces it to vanish throughout. If $U''\equiv0$, the real part of the identity is already a strictly positive integral for a nontrivial decaying mode. This proves the necessary sign-change condition.

[Fjørtoft's theorem](../../../../../fjortoft-theorem.md) strengthens this: if $U_s$ is the velocity at an inflection point, instability requires $U''(U-U_s)<0$ somewhere. This is a necessary condition, not a sufficient criterion. For $U=\tanh z$, $U_s=0$ and

$$
U''(U-U_s)=-2\tanh^2z\,\operatorname{sech}^2z<0\quad(z\ne0).
$$

The possibility of instability is therefore consistent with [Fjørtoft's theorem](../../../../../fjortoft-theorem.md).

For the piecewise-linear approximation, $U''=0$ within each of the three regions. The decaying solutions outside and the two independent interior solutions can be written

$$
\phi=\begin{cases}A_-e^{k(z+1)},&z<-1,\\Ce^{kz}+Ee^{-kz},&-1<z<1,\\A_+e^{-k(z-1)},&z>1.\end{cases}
$$

At each corner, the normal [velocity](../../../../../velocity.md) is continuous, so $\phi$ is continuous. [Pressure matching at a piecewise-linear shear interface](../../../../../pressure-matching-at-a-piecewise-linear-shear-interface.md) additionally gives $[(U-c)\phi'-U'\phi]=0$, hence $(U-c)[\phi']=[U']\phi$. At $z=1$ the slope jumps from $1$ to $0$; at $z=-1$ it jumps from $0$ to $1$. Substituting the decaying outer solutions gives

$$
\begin{pmatrix}1-2k+2kc&e^{-2k}\\e^{-2k}&1-2k-2kc\end{pmatrix}\begin{pmatrix}C\\E\end{pmatrix}=0.
$$

Thus the [inviscid instability of a piecewise-linear mixing layer](../../../../../inviscid-instability-of-a-piecewise-linear-mixing-layer.md) has [dispersion relation](../../../../../dispersion-relation.md)

$$
\boxed{4k^2c^2=(2k-1)^2-e^{-4k}.}
$$

At $k=1/2$, $c=\pm i/e$, so the root with positive imaginary part is an explicitly growing mode, with **growth rate $1/(2e)$**. More generally the unstable interval is $0<k<k_c$, where the unique $k_c>1/2$ solves $2k_c-1=e^{-2k_c}$. This direct calculation establishes instability of the approximation; passing a necessary inflection test alone would not have established it.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
