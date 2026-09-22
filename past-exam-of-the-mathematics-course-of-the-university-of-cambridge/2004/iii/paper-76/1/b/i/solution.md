<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take the usual [Heaviside step function](../../../../../../../heaviside-step-function.md), $H(x)=1$ for $x>0$ and $0$ for $x<0$. Its [Fourier transform](../../../../../../../fourier-transform.md) must be interpreted as a [tempered distribution](../../../../../../../tempered-distribution.md). For $a>0$, exponential damping gives an ordinary integral:

$$
\widehat{e^{-ax}H(x)}(k)=\int_0^\infty e^{-(a+ik)x}\,dx
=\frac1{a+ik}=\frac a{a^2+k^2}-i\frac{k}{a^2+k^2}.
$$

Against any [Schwartz function](../../../../../../../schwartz-function.md) $\varphi$, the first term is an [approximate identity](../../../../../../../approximate-identity.md) of total mass $\pi$: changing variables $k=au$ gives the limit $\pi\varphi(0)$. For the second term, pair positive and negative $k$ near zero. The difference $\varphi(k)-\varphi(-k)=O(k)$ removes the singularity and gives the [Cauchy principal value](../../../../../../../cauchy-principal-value.md) of $1/k$. The tails converge by [dominated convergence](../../../../../../../dominated-convergence-theorem.md). Since the damped functions also approach $H$ as [tempered distributions](../../../../../../../tempered-distribution.md), continuity of the [Fourier transform](../../../../../../../fourier-transform.md) yields the [Fourier transform of the Heaviside step function](../../../../../../../fourier-transform-of-the-heaviside-step-function.md):

$$
\boxed{\widehat H(k)=\pi\delta(k)-i\operatorname{PV}\frac1k}.
$$

**The printed plus sign is inconsistent with the printed $e^{-ikx}$ convention for this $H$.** In fact $H'=\delta$ requires $ik\widehat H=1$; the printed expression would give $-1$. Its plus sign would instead be correct for $H(-x)$.

To find the [Fourier transform of a principal-value reciprocal](../../../../../../../principal-value-fourier-transform-of-a-real-pole.md), exponential damping of its odd part gives

$$
\widehat{e^{-a|x|}\operatorname{PV}(1/x)}(k)
=-2i\int_0^\infty e^{-ax}\frac{\sin(kx)}x\,dx.
$$

The integral vanishes at $k=0$ and its $k$-derivative is $a/(a^2+k^2)$, so it equals $\arctan(k/a)$. Taking the [distributional convergence](../../../../../../../weak-convergence-of-distributions.md) limit gives

$$
\boxed{\mathcal F\!\left(\operatorname{PV}\frac1x\right)(k)=-i\pi\operatorname{sgn}k}.
$$

An ordinary improper integral of $1/x$ across zero is not a substitute for the specified [Cauchy principal value](../../../../../../../cauchy-principal-value.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 76](../../../../paper-76-split.md)
5. [Iii](../../../../split.md)
6. [2004](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
