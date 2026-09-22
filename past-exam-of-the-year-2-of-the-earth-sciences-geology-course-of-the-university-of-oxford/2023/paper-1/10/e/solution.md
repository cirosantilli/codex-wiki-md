<h1 id="10/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

After [bath cooling followed by insulated equilibration](../../../../../bath-cooling-followed-by-insulated-equilibration.md), the remaining mean [temperature](../../../../../temperature-split.md) is conserved: integrating the insulated [heat equation](../../../../../heat-equation.md) gives

$$
\frac{d}{d\tau}\int_0^L U(x,\tau)\,dx=\kappa[U_x(L,\tau)-U_x(0,\tau)]=0.
$$

For constant [density](../../../../../density.md), specific [heat capacity](../../../../../heat-capacity.md) and cross-section, this is [conservation of energy](../../../../../conservation-of-energy.md). Its [Fourier cosine series](../../../../../fourier-cosine-series.md) has a constant mode equal to the initial [integral average](../../../../../integral-average.md); every nonconstant mode decays. Therefore the eventual uniform [temperature](../../../../../temperature-split.md) is

$$
T_f=\frac1L\int_0^LT(x,t_f)\,dx.
$$

For each mode with an [odd integer](../../../../../odd-integer.md) index in part (c), $L^{-1}\int_0^L\sin((2j+1)\pi x/L)dx=2/[(2j+1)\pi]$. Integrating the bath-cooled series yields

$$
\boxed{T_f=\frac{8T_0}{\pi^2}\sum_{j=0}^{\infty}\frac{1}{(2j+1)^2}\exp\left[-\frac{(2j+1)^2\pi^2\kappa t_f}{L^2}\right]}.
$$

For $t_f>0$, [uniform convergence](../../../../../uniform-convergence.md) justifies termwise [integration](../../../../../integral-split.md); the $t_f=0$ result also follows by dominated convergence of the summable positive coefficients. As a check, $\sum_{j\geq0}(2j+1)^{-2}=\pi^2/8$ gives $T_f=T_0$ for zero bath time, and $T_f\to0$ as $t_f\to\infty$. More bath time strictly lowers the retained average [temperature](../../../../../temperature-split.md) when $T_0>0$ and $\kappa>0$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
