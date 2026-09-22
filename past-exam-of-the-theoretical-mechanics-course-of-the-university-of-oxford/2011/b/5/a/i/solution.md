<h1 id="b/5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take the nondegenerate [stationary point](../../../../../../stationary-point.md) in the interior of the integration interval. Choose a smooth cutoff equal to one near $k_\star$. Away from its support, $\psi'$ is bounded away from zero. [Integration by parts](../../../../../../integration-by-parts.md) using $e^{it\psi}=(it\psi')^{-1}\partial_ke^{it\psi}$ makes that nonstationary contribution $O(t^{-1})$, under the usual smooth-phase assumptions.

Near the [stationary point](../../../../../../stationary-point.md) use the signed coordinate

$$
s=\operatorname{sgn}(k-k_\star)\sqrt{2(\psi(k)-\psi(k_\star))}.
$$

Since $\psi''(k_\star)>0$, this is locally invertible, with $ds/dk=\sqrt{\psi''(k_\star)}$ at the point. The local [integral](../../../../../../integral-split.md) becomes

$$
e^{it\psi(k_\star)}\int a(s)e^{its^2/2}\,ds,\qquad a(0)=\frac{f(k_\star)}{\sqrt{\psi''(k_\star)}}.
$$

Scale $s=\sqrt{2/t}\,r$. The supplied [Fresnel integral](../../../../../../fresnel-integral.md) gives $\int_{-\infty}^{\infty}e^{ir^2}dr=e^{i\pi/4}\sqrt\pi$. Approximating the smooth [amplitude](../../../../../../wave-amplitude.md) by its value at zero, with a cutoff and a nonstationary estimate for the tails, therefore gives

$$
\boxed{I(t)=f(k_\star)e^{it\psi(k_\star)+i\pi/4}\sqrt{\frac{2\pi}{t\psi''(k_\star)}}+o(t^{-1/2}).}
$$

If $f(k_\star)\ne0$, this is the requested asymptotic equivalence. The phase shift $\pi/4$ comes from the positive quadratic curvature. A [stationary point](../../../../../../stationary-point.md) at an integration endpoint instead needs a one-sided formula.

The printed auxiliary estimate asserting an $O(\gamma^{-1})$ Fourier [integral](../../../../../../integral-split.md) for every continuous [amplitude](../../../../../../wave-amplitude.md) is too strong without extra regularity. The argument here uses [integration by parts](../../../../../../integration-by-parts.md) only for the actual smooth, cutoff nonstationary amplitudes, where that estimate is justified; continuity alone generally guarantees convergence to zero, not this rate.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../../split.md)
7. [Theoretical mechanics course of the University of Oxford](../../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
