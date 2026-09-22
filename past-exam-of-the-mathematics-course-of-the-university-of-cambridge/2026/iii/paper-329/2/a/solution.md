<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret the stated ansatz as

$$
a(z,t)=f(t)+\sqrt2\,g(t)\sin(kz).
$$

Multiplying the pressure relation by $a$ gives $2\mu a_t=Pa-\gamma$. Equating its constant and sinusoidal parts yields

$$
f'=\frac{Pf-\gamma}{2\mu},
\qquad
g'=\frac{Pg}{2\mu}.
$$

The volume per wavelength is proportional to the mean of $a^2$, namely $f^2+g^2$. Hence

$$
\boxed{\alpha_0=f(0)^2+g(0)^2=f(t)^2+g(t)^2}.
$$

Choosing

$$
P=\frac{\gamma f}{\alpha_0}
$$

then gives exactly

$$
\boxed{f'=-\frac\gamma{2\mu}\frac{g^2}{\alpha_0}},
\qquad
\boxed{g'=\frac\gamma{2\mu}\frac{fg}{\alpha_0}}.
$$

For $g\ll f\simeq a_0$, the disturbance amplitude obeys

$$
g'\simeq\frac\gamma{2\mu a_0}g,
$$

so its long-wave linear growth rate is

$$
\boxed{s=\frac\gamma{2\mu a_0}}.
$$

The minimum radius is $a_{\min}=f-\sqrt2g$, and

$$
\frac{d a_{\min}}{dt}
=-\frac\gamma{2\mu\alpha_0}(g^2+\sqrt2fg)<0.
$$

Since the trajectory follows the circle $f^2+g^2=\alpha_0$ toward increasing $g$, it reaches $f=\sqrt2g$ and hence $a_{\min}=0$. Thus the nonlinear disturbance narrows monotonically to pinch-off within this approximation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
