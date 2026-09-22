<h1 id="b/5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Orient the smooth contour so the plus side is to its left. Assume the density is Hölder continuous near the observation point and the integrals converge at any other endpoints. The [Cauchy principal value](../../../../../cauchy-principal-value.md) is

$$
\operatorname{PV}\int_\Gamma\frac{f(\zeta)}{\zeta-t}d\zeta
=\lim_{\eta\downarrow0}\int_{\Gamma\setminus B_\eta(t)}\frac{f(\zeta)}{\zeta-t}d\zeta.
$$

Subtract $f(t)$ from the numerator. The resulting quotient is locally integrable, so its limits from the two sides coincide. For the remaining constant density, straightening the contour gives a half-circle contribution $\pm i\pi f(t)$. Division by $2\pi i$ yields the [Sokhotski–Plemelj formula](../../../../../sokhotski-plemelj-theorem.md)

$$
\boxed{w_\pm(t)=\pm\tfrac12f(t)+\frac1{2\pi i}\operatorname{PV}\int_\Gamma\frac{f(\zeta)}{\zeta-t}d\zeta.}
$$

For the requested real integral assume $0<\alpha<1$ and $-1<x<1$, ensuring integrable endpoints and an interior principal-value [pole](../../../../../pole.md). Put $W(t)=(1-t)^{\alpha-1}/(1+t)^\alpha$. Choose $w(z)=(z-1)^{\alpha-1}/(z+1)^\alpha$ analytic off $[-1,1]$, positive for $z>1$, and $w(z)\sim1/z$ at infinity. Its two boundary values are $w_\pm(t)=-e^{\pm i\pi\alpha}W(t)$.

The jump is $-2i\sin(\pi\alpha)W(t)$. The Cauchy representation for this decaying analytic function is therefore $w(z)=-\sin(\pi\alpha)\int_{-1}^1W(t)/(t-z)dt\,/\pi$. Taking the mean of its two boundary values removes the half-[residue](../../../../../residue.md) terms and gives

$$
\boxed{\operatorname{PV}\int_{-1}^1\frac{(1-t)^{\alpha-1}}{(1+t)^\alpha(t-x)}dt
=\pi\cot(\pi\alpha)\frac{(1-x)^{\alpha-1}}{(1+x)^\alpha}.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
