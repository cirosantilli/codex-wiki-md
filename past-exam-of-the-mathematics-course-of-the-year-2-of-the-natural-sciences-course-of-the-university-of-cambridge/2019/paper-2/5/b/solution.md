<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $\lambda>0$ and $t>0$, the [positive diffusivity requirement for the forward heat kernel](../../../../../positive-diffusivity-requirement-for-the-forward-heat-kernel.md). The PDF does not explicitly specify the sign of $\lambda$; the stated real [Gaussian function](../../../../../gaussian-function.md) formula requires this assumption. For a direct calculation, initially assume sufficiently smooth and rapidly decreasing data, so that the [Fourier transform](../../../../../fourier-transform-split.md), its inverse and the following integrations are justified. The resulting [heat-kernel convolution](../../../../../heat-kernel-convolution.md) extends to wider classes of initial data.

Using the stated [Fourier transform](../../../../../fourier-transform-split.md) convention and [integration by parts](../../../../../integration-by-parts.md),

$$
\widetilde{u_{xx}}(k,t)=-k^2\widetilde u(k,t),\qquad
\partial_t\widetilde u=-\lambda k^2\widetilde u.
$$

The transformed [ordinary differential equation](../../../../../ordinary-differential-equation.md) has solution $\widetilde u(k,t)=e^{-\lambda k^2t}\widetilde u_0(k)$. [Fourier inversion](../../../../../fourier-inversion-theorem.md) then gives

$$
u(x,t)=\int_{-\infty}^{\infty}u_0(y)K_t(x-y)\,dy,\qquad
K_t(s)=\frac1{2\pi}\int_{-\infty}^{\infty}e^{-\lambda tk^2+iks}\,dk.
$$

Complete the square:

$$
-\lambda tk^2+iks
=-\lambda t\left(k-\frac{is}{2\lambda t}\right)^2-\frac{s^2}{4\lambda t}.
$$

Part (a), after scaling by $\sqrt{\lambda t}$, evaluates the remaining [Gaussian integral](../../../../../gaussian-integral.md) even though its shift is imaginary. Therefore

$$
K_t(s)=\frac{e^{-s^2/(4\lambda t)}}{\sqrt{4\pi\lambda t}},\qquad
\boxed{u(x,t)=\frac1{\sqrt{4\pi\lambda t}}\int_{-\infty}^{\infty}
e^{-(x-y)^2/(4\lambda t)}u(y,0)\,dy}.
$$

The [heat kernel](../../../../../heat-kernel.md) has integral one and is an [approximate identity](../../../../../approximate-identity.md) as $t\downarrow0$, which recovers the initial condition. Mere decay at spatial infinity does not by itself imply every Fourier integral is absolutely convergent; the regularity assumption above supplies a rigorous setting for the derivation.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
