<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $s=\delta Z>0$. For the [Fay solution](../../../../../../../fay-solution.md), $1/\sinh(ns)=2e^{-ns}[1+O(e^{-2ns})]$. At $s\gg1$ the first harmonic therefore gives

$$
\boxed{q=4\delta e^{-s}\sin\theta+O(\delta e^{-2s}),}
$$

which agrees with the late-time limit in (i).

For the opposite limit, expand the reciprocal [hyperbolic sine](../../../../../../../hyperbolic-sine.md) as a [geometric series](../../../../../../../geometric-series.md) and interchange absolutely convergent sums at every $s>0$:

$$
\begin{aligned}
q&=4\delta\sum_{j=0}^{\infty}\sum_{n=1}^{\infty}e^{-(2j+1)ns}\sin n\theta\\
&=4\delta\sum_{j=0}^{\infty}\frac{e^{-(2j+1)s}\sin\theta}{1-2e^{-(2j+1)s}\cos\theta+e^{-2(2j+1)s}}\\
&=2\delta\sin\theta\sum_{j=0}^{\infty}\frac1{\cosh((2j+1)s)-\cos\theta}.
\end{aligned}
$$

This exact positive-denominator form is useful near the shock. For small $s$ and $|\theta|$, expand the denominator of the terms with small $(2j+1)s$ and use $\sin\theta\sim\theta$. The leading sum is

$$
q\sim\frac{4\delta\theta}{s^2}\sum_{j=0}^{\infty}\frac1{(2j+1)^2+(\theta/s)^2}.
$$

For the shock-layer scaling $\theta=s\eta$, the passage to this sum follows from dominated convergence: $\cosh z-1\ge z^2/2$ and $1-\cos\theta\ge c\theta^2$ for small $|\theta|$ provide a summable bound proportional to $[(2j+1)^2+\eta^2]^{-1}$. The same leading expression matches the outer small-angle range $s\ll|\theta|\ll1$. More generally, split the exact sum at $(2j+1)s=b$ with $\max(s,|\theta|)\ll b\ll1$: the low terms have vanishing relative Taylor error, while the discarded exact and approximate tails are smaller than the leading expression by $O(\max(s,|\theta|)/b)$.

Now apply the partial-fraction identity for the [hyperbolic tangent](../../../../../../../hyperbolic-tangent.md) with $\eta=\theta/s$:

$$
\sum_{j=0}^{\infty}\frac1{(2j+1)^2+\eta^2}=\frac{\pi}{4\eta}\tanh(\pi\eta/2).
$$

The [Fay shock-layer asymptotics](../../../../../../../fay-shock-layer-asymptotics.md) are therefore

$$
\boxed{q(\theta,Z)\sim\frac\pi Z\tanh\!\left(\frac{\pi\theta}{2\delta Z}\right),\qquad |\theta|\ll1,\ \delta Z\ll1.}
$$

The angular shock thickness is $O(\delta Z)$, and its matched states are $\pm\pi/Z$. At $\theta=0$, both formulas vanish; the limiting slopes agree. The denominator throughout this derivation is $\sinh(n\delta Z)$ as printed in the PDF, not the erroneous $\sin(n\delta Z)$ in the converted TeX.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 82](../../../../paper-82-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
