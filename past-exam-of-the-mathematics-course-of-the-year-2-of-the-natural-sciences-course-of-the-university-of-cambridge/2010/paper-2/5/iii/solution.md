<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [convolution theorem](../../../../../convolution-theorem.md) turns the product $e^{-k^2t}\widetilde\theta(k,0)$ into a spatial [convolution](../../../../../convolution.md). Its kernel is

$$
G(z,t)=\frac1{2\pi}\int_{\mathbb R}e^{-tk^2+ikz}dk,\qquad t>0.
$$

Complete the square:

$$
-tk^2+ikz=-t\left(k-\frac{iz}{2t}\right)^2-\frac{z^2}{4t}.
$$

After rescaling the variable, the supplied translated [Gaussian integral](../../../../../gaussian-integral.md) gives

$$
\boxed{G(z,t)=\frac1{\sqrt{4\pi t}}e^{-z^2/(4t)},\qquad
\theta(x,t)=\frac1{\sqrt{4\pi t}}\int_{\mathbb R}\theta(y,0)e^{-(x-y)^2/(4t)}dy.}
$$

This is the [heat-kernel solution](../../../../../heat-kernel-solution.md) for diffusivity one. Its kernel integrates to one, preserving the total temperature integral, and approaches a [Dirac delta function](../../../../../dirac-delta-function.md) as $t\downarrow0$. Its variance is $2t$; the factor is appropriate to $\theta_t=\theta_{xx}$, rather than the alternative convention with diffusivity $1/2$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
