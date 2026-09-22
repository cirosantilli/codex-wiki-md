<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [Fourier stability analysis](../../../../../../fourier-stability-analysis.md), take spatial modes $e^{im\theta}$ and put

$$
D(\theta)=ae^{-i\theta}+b+ce^{i\theta},\qquad
N(\theta)=d+ee^{i\theta},\qquad G(\theta)=N(\theta)/D(\theta).
$$

A bounded implicit step requires $D$ to stay away from zero, and [von Neumann stability analysis](../../../../../../von-neumann-stability-analysis.md) requires $|G|\leq1$ for every frequency. Expanding the squared moduli and using $\cos2\theta=2\cos^2\theta-1$ gives

$$
\begin{aligned}
|D|^2&=a^2+b^2+c^2+2b(a+c)\cos\theta+2ac\cos2\theta,\\
|N|^2&=d^2+e^2+2de\cos\theta,\\
\boxed{|D|^2-|N|^2}&=\boxed{\mu(\mu-2)(\mu-1)(\mu+1)(1-\cos\theta)^2.}
\end{aligned}
$$

Consequently, apart from denominator invertibility, the necessary and sufficient sign condition is

$$
\mu(\mu-2)(\mu-1)(\mu+1)\geq0.
$$

Its real solution set is $(-\infty,-1]\cup[0,1]\cup[2,\infty)$.

To check the denominator rather than assume it, note

$$
\operatorname{Im}D=(1-2\mu)\sin\theta,\qquad
D(0)=3,\qquad D(\pi)=1+2\mu-2\mu^2.
$$

If $\mu\ne1/2$, a zero can occur only at zero or the Nyquist frequency. The zero-frequency value is nonzero, and the Nyquist zeros occur only at $\mu=(1\pm\sqrt3)/2$, both outside the proposed stable intervals. At $\mu=1/2$, $D=9/4+(3/4)\cos\theta\geq3/2$, also nonzero. Continuity on the frequency circle now gives a positive lower bound on $|D|$ for each allowed $\mu$.

The implicit convolution operator is therefore boundedly invertible on the square-summable grid sequences. By the [Plancherel theorem](../../../../../../plancherel-theorem.md), $|G|\leq1$ gives

$$
\boxed{\|u^{n+1}\|_{\ell^2_h}\leq\|u^n\|_{\ell^2_h},\qquad
\mu\in(-\infty,-1]\cup[0,1]\cup[2,\infty).}
$$

Outside these intervals the modulus difference is negative at every nonzero frequency where $D$ is nonzero. There is an interval on which $|G|>1$, giving arbitrarily large growth of powers of the step operator, so the method is unstable; a zero of $D$ additionally makes the step ill posed.

For the physical choice $k,h>0$, the stable range is **$0<\mu\leq1$ or $\mu\geq2$**; zero is the limiting zero-step case. The exact-shift values have unit gain and are included.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
