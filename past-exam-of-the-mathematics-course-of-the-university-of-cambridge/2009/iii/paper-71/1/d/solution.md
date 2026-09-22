<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix $T>t$. In the representation from (c), the [finite-horizon extension of a boundary transform](../../../../../../finite-horizon-extension-of-a-boundary-transform.md) allows $G_0(k,t)$ to be replaced by $G_0(k,T)$. To see this directly, their difference contributes

$$
\int_{\partial D_+}e^{ikx}(1-3k^2)\int_t^T e^{\omega(k)(s-t)}g_0(s)\,ds\,dk.
$$

It has an [holomorphic](../../../../../../complex-differentiability-at-a-point.md) [integrand](../../../../../../integrand.md) inside $D_+$; there $\operatorname{Re}\omega<0$, and the factors $e^{\omega(s-t)}$ and $e^{ikx}$ allow the [contour](../../../../../../complex-integration-contour.md) to be closed. Its [integral](../../../../../../integral.md) is zero for $x>0$. This replacement puts the observation-time dependence entirely in $e^{ikx-\omega t}$.

Every such exponential satisfies the [linear dispersive Stokes equation](../../../../../../linear-dispersive-stokes-equation.md), because

$$
\bigl(\partial_t+\partial_x+\partial_x^3\bigr)e^{ikx-\omega(k)t}
=\bigl[-\omega(k)+ik+(ik)^3\bigr]e^{ikx-\omega(k)t}=0.
$$

Consequently the representation satisfies the [partial differential equation](../../../../../../partial-differential-equation-split.md). The stipulated smoothness and decay justify the differentiated oscillatory [integrals](../../../../../../integral.md), or equivalently their regularized limits. The fixed horizon is useful here: no artificial source term arises from differentiating the endpoint of a time transform.

At $t=0$, use the original $G_0(k,0)=0$ version. The $F$ [integral](../../../../../../integral.md) vanishes after closing inside $D_+$, since $F$ is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) there and $x>0$. [Fourier inversion](../../../../../../fourier-inversion-theorem.md) of the initial half-line transform therefore gives

$$
\boxed{q(x,0)=q_0(x)\quad(x>0).}
$$

For the boundary trace use the fixed-horizon version, with $0<t<T$. First consider the initial-data terms at $x=0$. Differentiating $\nu_j^2+k\nu_j+k^2-1=0$ gives

$$
\nu_1'=-A_1,\qquad\nu_2'=-A_2.
$$

Thus changing variables separately in the two pieces of the $F$ [integral](../../../../../../integral.md) gives

$$
\int_{\mathbb R}e^{-\omega t}\widehat q_0\,dk
-\int_{\partial D_+}e^{-\omega t}F\,dk
=\int_{\Gamma_-}e^{-\omega(k)t}\widehat q_0(k)\,dk,
$$

where $\Gamma_-$ goes from lower-left infinity to $-1/\sqrt3$, across to $1/\sqrt3$, and then to lower-right infinity along $\operatorname{Re}\omega=0$. For completeness, on the upper-right curved edge one root maps onto the real ray $(-\infty,-2/\sqrt3]$ and the other onto the lower-right curved edge. On the upper-left edge the corresponding images are $[2/\sqrt3,\infty)$ and the lower-left edge. The middle segment maps to the remaining real intervals $[1/\sqrt3,2/\sqrt3]$ and $[-2/\sqrt3,-1/\sqrt3]$. These real images cancel the outer pieces of the original real-axis [integral](../../../../../../integral.md), leaving exactly $\Gamma_-$ with the stated orientation.

This [contour](../../../../../../complex-integration-contour.md) bounds the lower-central region $\operatorname{Im}k<0$, $\operatorname{Re}\omega>0$. The spatial transform is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) there and $e^{-\omega t}$ decays on its closing arcs for $t>0$. Its [integral](../../../../../../integral.md) is therefore zero by the [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md). The initial-data part of the boundary trace vanishes.

In the remaining boundary [integral](../../../../../../integral.md), use $d\omega=i(1-3k^2)\,dk$. Along the oriented $\partial D_+$, $\omega$ traverses the imaginary axis once from $-i\infty$ to $i\infty$. On its real segment, the imaginary part runs from $-2/(3\sqrt3)$ to $2/(3\sqrt3)$; the two curved edges supply the complementary intervals. It follows that

$$
q(0,t)=\frac1{2\pi i}\int_{-i\infty}^{i\infty}e^{-\omega t}
\left[\int_0^T e^{\omega s}g_0(s)\,ds\right]d\omega=g_0(t).
$$

The last equality is ordinary temporal [Fourier inversion](../../../../../../fourier-inversion-theorem.md), after $\omega=i\xi$. Because $t$ is strictly inside $(0,T)$ it gives the full value, not a truncated-transform endpoint half-value. Thus

$$
\boxed{q(0,t)=g_0(t)\quad(t>0).}
$$

Compatibility $q_0(0)=g_0(0)$ makes the two traces agree at the corner. Spatial decay follows from the upper-[contour](../../../../../../complex-integration-contour.md) exponential and nonstationary oscillatory estimates on the real [integral](../../../../../../integral.md) as $x\to\infty$, under the assumed data decay.

The decaying smooth solution is also unique. For a zero-data difference $w$, [integration by parts](../../../../../../integration-by-parts.md) in the [linear dispersive Stokes equation](../../../../../../linear-dispersive-stokes-equation.md) gives

$$
\frac d{dt}\frac12\int_0^\infty|w|^2\,dx=-\frac12|w_x(0,t)|^2\leq0,
$$

using $w(0,t)=0$ and decay at infinity. The initial norm is zero, so $w=0$. This completes verification of the initial value, boundary value and governing equation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
