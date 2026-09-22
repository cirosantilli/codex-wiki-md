<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\tau=t-t'$ and $\Omega=\sqrt{k^2+m^2-\lambda^2}>0$. First take $\lambda=e\gamma>0$. Since $|e^{-i\omega\tau}|=e^{\tau\operatorname{Im}\omega}$, close the [contour](../../../../../complex-integration-contour.md) below for $\tau>0$, and above for $\tau<0$. On the chosen semicircle the exponential is bounded and the denominator grows as $R^2$, so the arc integral tends to zero. The upper [contour](../../../../../complex-integration-contour.md) encloses no [pole](../../../../../pole.md), giving **$G=0$ for $t<t'$**. The lower [contour](../../../../../complex-integration-contour.md) is clockwise, hence the real-axis integral divided by $2\pi$ is $-i$ times the sum of [residues](../../../../../residue.md). Since $D'(\omega_+)=-2\Omega$ and $D'(\omega_-)=2\Omega$, that sum is

$$
-\frac{e^{-i(\Omega-i\lambda)\tau}}{2\Omega}+\frac{e^{-i(-\Omega-i\lambda)\tau}}{2\Omega}=i e^{-\lambda\tau}\frac{\sin(\Omega\tau)}{\Omega}.
$$

Thus

$$
\boxed{G(\mathbf k;t,t')=H(t-t')\,e^{-\lambda(t-t')}\frac{\sin[\Omega(t-t')]}{\Omega}\quad(\lambda>0).}
$$

This is the [causal Green function of a damped oscillator](../../../../../causal-green-function-of-a-damped-oscillator.md). Its value is continuous through $\tau=0$, and its derivative jumps from zero to one; integrating the [differential equation](../../../../../differential-equation-split.md) through zero verifies the delta-source normalization and the [residue](../../../../../residue.md) sign. The limits are $H(\tau)\tau e^{-\lambda\tau}$ at [critical damping](../../../../../critical-damping.md) and $H(\tau)e^{-\lambda\tau}\sinh(\kappa\tau)/\kappa$ in the overdamped regime.

For completeness, if the unspecified charge has $e<0$, the same real-axis integral instead encloses upper [poles](../../../../../pole.md) for $\tau<0$ and gives $-H(-\tau)e^{-\lambda\tau}\sin(\Omega\tau)/\Omega$, an advanced [Green function](../../../../../green-s-function-split.md). A causal growing response would require an inverse-Laplace [contour](../../../../../complex-integration-contour.md) above those [poles](../../../../../pole.md), not the stated real-axis Fourier integral. At $e=0$ the real-axis integral needs a [pole](../../../../../pole.md) prescription; shifting both [poles](../../../../../pole.md) below it gives the retarded zero-damping limit. These distinctions are necessary because $\gamma>0$ alone does not fix the sign of damping.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
