<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Since $0<f_\alpha\leq1$, its [regular distribution](../../../../../regular-distribution.md) satisfies

$$
|\langle f_\alpha,\phi\rangle|\leq\|\phi\|_1
\leq\pi\bigl(p_{0,0}(\phi)+p_{2,0}(\phi)\bigr),
$$

so $f_\alpha$ is a [tempered distribution](../../../../../tempered-distribution.md) for every $\alpha>0$.

Put $a=\alpha/2$. The defining [integral](../../../../../integral-split.md) of the [gamma function](../../../../../gamma-function.md), with $r=(1+x^2)t$, gives

$$
f_\alpha(x)=\frac1{\Gamma(a)}\int_0^\infty t^{a-1}e^{-t}e^{-tx^2}\,dt.
$$

The [Fourier transform of a Gaussian](../../../../../fourier-transform-of-a-gaussian.md) suggests the following representative for the [Fourier transform of an inverse power of one plus x squared](../../../../../fourier-transform-of-an-inverse-power-of-one-plus-x-squared.md):

$$
\boxed{h_\alpha(\xi)=\frac{\sqrt\pi}{\Gamma(a)}\int_0^\infty t^{a-3/2}e^{-t-\xi^2/(4t)}\,dt\quad(\xi\ne0).}
$$

All factors are positive. [Tonelli's theorem](../../../../../tonelli-theorem.md) evaluates its total [integral](../../../../../integral-split.md), allowing an infinite value at the single point zero:

$$
\begin{aligned}
\int_{\mathbb R}h_\alpha(\xi)\,d\xi
&=\frac{\sqrt\pi}{\Gamma(a)}\int_0^\infty t^{a-3/2}e^{-t}
\left(\int_{\mathbb R}e^{-\xi^2/(4t)}\,d\xi\right)dt\\
&=\frac{2\pi}{\Gamma(a)}\int_0^\infty t^{a-1}e^{-t}\,dt=2\pi.
\end{aligned}
$$

Assign any finite value at zero if necessary. This gives an [integrable function](../../../../../lebesgue-integrable-function.md) with $\|h_\alpha\|_1=2\pi$.

To verify equality as [tempered distributions](../../../../../tempered-distribution.md), take any [Schwartz function](../../../../../schwartz-function.md) $\phi$. Substituting the mixture into $\langle f_\alpha,\widehat\phi\rangle$ is justified by

$$
\frac1{\Gamma(a)}\int_0^\infty t^{a-1}e^{-t}\int e^{-tx^2}|\widehat\phi(x)|\,dx\,dt
\leq\|\widehat\phi\|_1.
$$

For each $t>0$, [Fubini's theorem](../../../../../fubini-s-theorem.md) and the [Fourier transform of a Gaussian](../../../../../fourier-transform-of-a-gaussian.md) identify the inner pairing with $\int\sqrt{\pi/t}\,e^{-\xi^2/(4t)}\phi(\xi)\,d\xi$. Interchanging the resulting [integrals](../../../../../integral-split.md) is valid because their absolute value is bounded by $2\pi\|\phi\|_\infty$ after integrating the positive kernel. Therefore

$$
\langle\widehat{f_\alpha},\phi\rangle=\int h_\alpha(\xi)\phi(\xi)\,d\xi.
$$

Finally, on a [compact set](../../../../../compact-space.md) with $|\xi|\geq\delta>0$, the mixture [integrand](../../../../../integrand.md) is bounded by $t^{a-3/2}e^{-t-\delta^2/(4t)}$, which is integrable both at zero and at infinity. [Dominated convergence](../../../../../dominated-convergence-theorem.md) proves continuity there. Hence $\boxed{\widehat{f_\alpha}=h_\alpha\in L^1(\mathbb R),\ h_\alpha(\xi)>0\text{ and continuous for }\xi\ne0}$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
