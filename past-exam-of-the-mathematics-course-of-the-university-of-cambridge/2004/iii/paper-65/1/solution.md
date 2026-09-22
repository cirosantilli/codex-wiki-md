<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Consider the complex field before taking its real part. Put $p=\hat z\times k=(-k_y,k_x,0)$ and $b=Rp+S\hat z$. Both components are perpendicular to $k$, so the [solenoidal magnetic-field constraint](../../../../../solenoidal-magnetic-field-constraint.md) holds. The time-dependent phase obeys

$$
(\partial_t+u\cdot\nabla)e^{ik(t)\cdot x}=i(\dot k\cdot x+u\cdot k)e^{ik\cdot x}=0,
$$

because $\dot k_y=-k_0/T$ and $u\cdot k=k_0y/T$. Moreover $\dot p=(k_0/T,0,0)$, and magnetic stretching is $b\cdot\nabla u=(Rk_0/T,0,0)=R\dot p$. Thus the changing basis exactly supplies the shear-stretching term. Finally,

$$
k\times p=k^2\hat z,\qquad k\times\hat z=-p,\qquad
\nabla\times(be^{ik\cdot x})=i(k^2R\hat z-Sp)e^{ik\cdot x},
$$

and $\nabla^2$ acts as $-k^2$. Equating coefficients verifies

$$
\boxed{\dot R=-i\alpha S-\eta k^2R,\qquad \dot S=i\alpha k^2R-\eta k^2S.}
$$

Take $k_0,T>0$ and first $\alpha\ne0$. Remove [magnetic diffusion](../../../../../magnetic-diffusion.md) by writing $R=e^{-D}G$, $S=e^{-D}H$, where

$$
D(t)=\eta\int_0^tk^2(s)ds=\eta k_0^2\left(t+\frac{t^3}{3T^2}\right).
$$

Then $\dot G=-i\alpha H$, $\dot H=i\alpha k^2G$, and $\ddot G=\alpha^2k^2G$. Equivalently, rescaling time by $|\alpha|$ and replacing $H$ by $\operatorname{sgn}(\alpha)H$ gives the pair used in the question. Its growing [WKB approximation](../../../../../wkb-approximation.md) is

$$
G\sim Ck^{-1/2}\exp\left(|\alpha|\int_0^tk(s)ds\right),\qquad
H\sim i\operatorname{sgn}(\alpha)kG.
$$

The complex relative phase follows directly from $H=i\dot G/\alpha$; the printed $H\sim kG$ is sufficient for magnitudes but omits that phase.

The phase-averaged [magnetic energy](../../../../../magnetic-energy.md) is $(k^2|R|^2+|S|^2)/(4\mu_0)$, hence for a nonzero growing-mode component

$$
E\sim C_1k\exp\left[2|\alpha|\int_0^tk(s)ds-2\eta\int_0^tk^2(s)ds\right].
$$

At $t\gg T$, $k\sim k_0t/T$, so its leading exponential is

$$
\boxed{E\ \propto\ t\exp\left(\frac{|\alpha|k_0}{T}t^2-\frac{2\eta k_0^2}{3T^2}t^3+\text{subleading terms}\right).}
$$

The positive quadratic term permits strong amplification before the negative cubic diffusion term dominates. The leading maximum occurs near $t_{\rm peak}=|\alpha|T/(\eta k_0)$. Put $\varepsilon=\eta k_0/|\alpha|$ and $b_0=|\alpha|k_0T$. A well-separated late-time growing interval requires

$$
\boxed{\varepsilon\ll1,\qquad \varepsilon^2\ll b_0.}
$$

The first ensures $t_{\rm peak}\gg T$; the second ensures the WKB condition at the peak, since $|\dot k|/(|\alpha|k^2)\sim\varepsilon^2/b_0$. For fixed nonzero $b_0$ both follow by taking sufficiently small positive $\eta$. The peak's leading exponent is $b_0/(3\varepsilon^2)$, whereas the eventual exponent tends to minus infinity. This is [mean-field shearing-wave transient amplification](../../../../../mean-field-shearing-wave-transient-amplification.md), not sustained [dynamo action](../../../../../dynamo-action.md).

Growth from the initial instant is possible explicitly: choose $S(0)=i\operatorname{sgn}(\alpha)k_0R(0)$ with $R(0)\ne0$. The initial logarithmic energy derivative is $2(|\alpha|k_0-\eta k_0^2)>0$ when $\varepsilon<1$. Growth is not asserted for every initial polarization, for example an identically zero field. If $\alpha=0$, the amplitudes simply diffuse and the energy is proportional to $[k^2|R_0|^2+|S_0|^2]e^{-2D}$; shear can still give algebraic transient amplification of an in-plane field for small diffusivity, but a purely vertical field only decays. Positive diffusivity is essential to the final decay.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
