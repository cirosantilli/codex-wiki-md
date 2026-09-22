<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A radial null ray obeys $c\,d\tau=dr/\sqrt{1+r^2/r_{\rm curv}^2}$. Hence

$$
c(\tau_0-\tau_*)=r_{\rm curv}\operatorname{arsinh}\frac{r_*}{r_{\rm curv}},\qquad
r_*=r_{\rm curv}\sinh\frac{c(\tau_0-\tau_*)}{r_{\rm curv}}.
$$

For the open matter solution, let $\beta=\sqrt{1-\Omega_m}$. The [Friedmann equation](../../../../../../friedmann-equations.md) gives $a'=H_0\sqrt{\Omega_m a+\beta^2a^2}$, and the age in [conformal time](../../../../../../conformal-time.md) is

$$
\tau_0=\frac1{H_0}\int_0^1\frac{da}{\sqrt{a(\Omega_m+\beta^2a)}}
=\frac2{H_0\beta}\operatorname{arsinh}\frac{\beta}{\sqrt{\Omega_m}}
=\frac2{H_0\beta}\operatorname{artanh}\beta.
$$

Thus

$$
\boxed{\tau_0=\frac1{H_0\beta}\ln\frac{1+\beta}{1-\beta},\qquad
r_*\simeq\frac{c}{H_0\beta}\sinh(2\operatorname{artanh}\beta)
=\frac{2c}{H_0\Omega_m}.}
$$

Here the stated approximation $\tau_*\ll\tau_0$ was used only in the last distance estimate. The flat limit is smooth: $\tau_0\to2/H_0$ and $r_*\to2c/H_0$. Retaining $\tau_*$ in the preceding null-ray formula gives the finite-emission-time correction.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
