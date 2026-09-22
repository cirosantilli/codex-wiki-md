<h1 id="12/solution">Solution</h1>

↑ **Parent:** [12](../12.md)

Work with $t>0$ and write $u=t^{-1/2}e^{-x^2/(4t)}$. The [chain rule](../../../../chain-rule.md) gives

$$
u_x=-\frac{x}{2t}u,\qquad u_{xx}=\left(\frac{x^2}{4t^2}-\frac1{2t}\right)u,\qquad u_t=\left(\frac{x^2}{4t^2}-\frac1{2t}\right)u.
$$

Thus $u_{xx}=u_t$: it is a constant multiple of the one-dimensional [Gaussian heat kernel](../../../../gaussian-heat-kernel.md).

For the modified equation, put $f=g(t)u$. Substitution gives $g u_{xx}=g'u+gu_t-gu/t$. The heat-equation terms cancel, and $u>0$ permits division to obtain $\boxed{g'=g/t}$. Solving this [separable differential equation](../../../../separable-differential-equation.md) gives

$$
\boxed{g(t)=Ct,\qquad f(x,t)=C\sqrt t\,e^{-x^2/(4t)},\quad t>0.}
$$

The zero solution is included by $C=0$. This is the [scalar integrating factor for a reaction-diffusion equation](../../../../scalar-integrating-factor-for-a-reaction-diffusion-equation.md) with reaction coefficient $1/t$, because the modified equation is $f_t=f_{xx}+f/t$. Its sign produces growth. Indeed $\int_{\mathbb R}u\,dx=2\sqrt\pi$ is constant, while $\int_{\mathbb R}f\,dx=2C\sqrt\pi\,t$ increases linearly for $C>0$; neither profile is being assigned unit normalization here.

<a id="12/image-diffusive-spreading-with-conserved-mass-versus-the-same-spreading-with-amplitude-growth"></a>
![](../../../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-2-diffusion-and-growth.png)

**[Figure 3](#12/image-diffusive-spreading-with-conserved-mass-versus-the-same-spreading-with-amplitude-growth). Diffusive spreading with conserved mass versus the same spreading with amplitude growth**. Original profiles at $t=0.5,1,2$. The left solution is $t^{-1/2}e^{-x^2/(4t)}$; the right is $\sqrt t\,e^{-x^2/(4t)}$ with $C=1$. Their widths both grow as $\sqrt t$, but their spatial integrals are respectively constant and proportional to $t$.

## ↑ Ancestors (12)

1. [12](../12.md)
2. [Paper 2](../../paper-2-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
