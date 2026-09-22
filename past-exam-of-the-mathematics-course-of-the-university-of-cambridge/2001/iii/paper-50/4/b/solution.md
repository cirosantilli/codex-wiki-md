<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Integrate the initial [Cole-Hopf transformation](../../../../../../cole-hopf-transformation.md) and choose a continuous positive normalization:

$$
\psi(\theta,0)=\begin{cases}1,&\theta<0,\\e^{U\theta/(2\epsilon)},&\theta>0.\end{cases}
$$

Split the [heat kernel](../../../../../../heat-kernel.md) convolution at zero, and complete the square in the positive half-line contribution. Define

$$
I_-=\int_\theta^\infty e^{-s^2/(4\epsilon Z)}\,ds,\qquad I_+=\int_{-(\theta+UZ)}^\infty e^{-s^2/(4\epsilon Z)}\,ds,\qquad E=e^{U(\theta+UZ/2)/(2\epsilon)}.
$$

The resulting [heat equation](../../../../../../heat-equation.md) solution is

$$
\psi=(4\pi\epsilon Z)^{-1/2}(I_-+EI_+).
$$

Differentiating the moving endpoints gives $\partial_\theta I_-=-e^{-\theta^2/(4\epsilon Z)}$ and $E\partial_\theta I_+=e^{-\theta^2/(4\epsilon Z)}$. These terms cancel. Hence $\psi_\theta=(4\pi\epsilon Z)^{-1/2}UEI_+/(2\epsilon)$, and the [viscous Burgers step solution with negative flux](../../../../../../viscous-burgers-step-solution-with-negative-flux.md) is

$$
\boxed{q=\frac{U}{1+\alpha e^{-U(\theta+UZ/2)/(2\epsilon)}},\qquad \alpha=\frac{I_-}{I_+}.}
$$

The lower limit of $I_-$ is $\theta$, as printed in the original PDF. The converted TeX's $-\theta$ does not give the correct convolution or endpoint cancellation.

For the [vanishing-viscosity limit](../../../../../../vanishing-viscosity-limit.md), the conservative flux is $F(q)=-q^2/2$ and the [characteristic speed](../../../../../../characteristic-speed.md) is $F'(q)=-q$. If $U>0$, the characteristics from the right move left and collide with those on the left. The [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md) gives shock speed $[F]/[q]=-U/2$. Thus

$$
q\longrightarrow\begin{cases}0,&\theta<-UZ/2,\\U,&\theta>-UZ/2.\end{cases}
$$

The viscous transition has width $O(\epsilon/U)$, and its centre value is exactly $U/2$ by the [midpoint symmetry of a viscous Burgers step](../../../../../../midpoint-symmetry-of-a-viscous-burgers-step.md).

If $U<0$, the right characteristics move right and separate from the left ones. The limit is a [rarefaction wave](../../../../../../rarefaction-wave.md),

$$
\boxed{q(\theta,Z)\longrightarrow\begin{cases}0,&\theta\leq0,\\-\theta/Z,&0<\theta<-UZ,\\U,&\theta\geq-UZ.\end{cases}}
$$

This follows either from the [Burgers Riemann problem with negative flux](../../../../../../burgers-riemann-problem-with-negative-flux.md) or the large-argument Gaussian-tail asymptotics of the exact formula. The two signs therefore give a shock and a spreading rarefaction respectively, not two shocks.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
