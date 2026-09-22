<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The initial profile is $f(x)=e^{-|x|}$, with the absolute value confirmed in the original PDF. Its [Fourier transform](../../../../../fourier-transform-split.md) is

$$
\widetilde f(k)=\int_0^\infty e^{-x}(e^{-ikx}+e^{ikx})dx=\frac{2}{1+k^2}.
$$

Using $\widetilde u_t(k,0)=0$ in the regular cosine-sine form gives

$$
\widetilde u(k,t)=\frac{2e^{-\gamma t}}{1+k^2}\left[\cos(ckt)+\gamma\frac{\sin(ckt)}{ck}\right],
$$

with the quotient interpreted as $t$ when $ck=0$. Put $v_0=|c|>0$. Inverting, or applying the [D'Alembert formula](../../../../../d-alembert-s-formula.md) to $e^{\gamma t}u$, whose initial velocity is $\gamma f$, gives

$$
\boxed{u(x,t)=\frac{e^{-\gamma t}}2\left[e^{-|x-v_0t|}+e^{-|x+v_0t|}+\frac{\gamma}{v_0}\int_{x-v_0t}^{x+v_0t}e^{-|s|}ds\right].}
$$

For an explicit expression at $t\geq0$, let $r=|x|$ and $s=v_0t$. The integral is $2e^{-r}\sinh s$ for $r\geq s$ and $2(1-e^{-s}\cosh r)$ for $r\leq s$. Therefore

$$
\boxed{u(x,t)=e^{-\gamma t}\begin{cases}
e^{-r}\left[\cosh(v_0t)+\dfrac{\gamma}{v_0}\sinh(v_0t)\right],&r\geq v_0t,\\[3pt]
e^{-v_0t}\cosh r+\dfrac{\gamma}{v_0}\left[1-e^{-v_0t}\cosh r\right],&r\leq v_0t.
\end{cases}}
$$

The branches agree at $r=v_0t$. At zero time, the integral vanishes and the translated profiles coincide, recovering $f$. Their time derivatives cancel, while the integral contributes $\gamma f$, cancelling the derivative of the prefactor, so $u_t(x,0)=0$.

For $c=0$ the limiting answer is $u=(1+\gamma t)e^{-\gamma t}e^{-|x|}$. The cusp in $f$ means the solution is understood as a [weak solution](../../../../../weak-solution.md), classically smooth away from the characteristic fronts $x=\pm v_0t$; it is not globally twice differentiable. No assumption that $\gamma$ is positive is needed for this initial-value solution.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
