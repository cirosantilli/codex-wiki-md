<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Separate $L$ into a [diffusion generator](../../../../../diffusion-generator.md) and the constant killing term $-1/2$. The appropriate [stochastic differential equation](../../../../../stochastic-differential-equation.md) and its explicit [geometric Brownian motion](../../../../../geometric-brownian-motion.md) solution are

$$
dX_s=X_s\,dB_s+\frac12X_s\,ds,\qquad X_0=x,
\qquad \boxed{X_s=xe^{B_s}.}
$$

The second-order term in the [Itô formula](../../../../../ito-s-lemma.md) cancels the drift of $\log|X|$ when $x\ne0$; if $x=0$, the solution stays zero.

Fix a terminal time $t$. Apply the [Itô formula](../../../../../ito-s-lemma.md) to $e^{-s/2}u(t-s,X_s)$ for $0\leq s\leq t$. Its drift is

$$
e^{-s/2}\left(-u_t+\frac{X_s^2}{2}u_{xx}+\frac{X_s}{2}u_x-\frac12u\right)(t-s,X_s)\,ds=0.
$$

After localization this is a [local martingale](../../../../../local-martingale.md), and it is bounded because $u$ is bounded. It is therefore a true [martingale](../../../../../martingale-split.md). Taking [expectations](../../../../../expected-value.md) at its endpoints gives the [Feynman-Kac formula](../../../../../feynman-kac-formula.md)

$$
\boxed{u(t,x)=e^{-t/2}\mathbb E[g(xe^{B_t})].}
$$

For $t>0$ and $x\ne0$, the change of variable $y=xe^z$ in the [normal density](../../../../../normal-density.md) produces the [killed geometric Brownian heat kernel](../../../../../killed-geometric-brownian-heat-kernel.md) with respect to [Lebesgue measure](../../../../../lebesgue-measure.md):

$$
\boxed{p(t,x,y)=
\begin{cases}
\displaystyle\frac{e^{-t/2}}{|y|\sqrt{2\pi t}}\exp\left[-\frac{\log^2(|y/x|)}{2t}\right],&xy>0,\\
0,&xy\leq0.
\end{cases}}
$$

For $xy>0$, an equivalent form is

$$
p(t,x,y)=\frac1{|x|\sqrt{2\pi t}}\exp\left[-\frac{(\log|y/x|+t)^2}{2t}\right].
$$

In particular,

$$
\boxed{p(t,1,y)=\frac1{\sqrt{2\pi t}}\exp\left[-\frac{(\log y+t)^2}{2t}\right]\quad(y>0).}
$$

The apparent missing $1/y$ in this last expression is absorbed into the completed square, together with the killing factor; it is not a transcription error. The total mass is $e^{-t/2}$, as expected for killing at rate $1/2$. At $x=0$ the fundamental kernel is instead the [measure](../../../../../measure.md) $e^{-t/2}\delta_0(dy)$; it has no [Radon-Nikodym derivative](../../../../../radon-nikodym-derivative.md) with respect to [Lebesgue measure](../../../../../lebesgue-measure.md). Thus $u(t,0)=e^{-t/2}g(0)$. At $t=0$ the kernel is $\delta_x$, and continuity of bounded $g$ gives the initial condition. This also specifies the fundamental solution at the degenerate point omitted by a density-only formula.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
