<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\widehat u_0$ be the [Fourier transform](../../../../../fourier-transform-split.md) of the initial [temperature](../../../../../temperature-split.md). Solving the scalar [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md) gives

$$
\boxed{\widehat u(k_x,k_y,t)=\widehat u_0(k_x,k_y)e^{-\alpha(k_x^2+k_y^2)t}.}
$$

Recover $u$ using the [Fourier inversion theorem](../../../../../fourier-inversion-theorem.md), with inverse factor $(2\pi)^{-2}$ for this two-dimensional convention. Equivalently, take the [convolution](../../../../../convolution.md) of the initial data with the two-dimensional [heat kernel](../../../../../heat-kernel.md). On a periodic square, the same exponential applies to each discrete [Fourier mode](../../../../../fourier-mode.md), with $k_x=2\pi m/L_x$ and $k_y=2\pi n/L_y$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2025](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
