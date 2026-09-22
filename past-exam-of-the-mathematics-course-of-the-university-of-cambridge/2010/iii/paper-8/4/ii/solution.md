<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The precise conclusion is that finite one-sided limits must agree, so a [jump discontinuity](../../../../../../jump-discontinuity.md) is impossible. We prove this using explicit kernels and derive every conjugate-series identity used. The distinction from a [removable discontinuity](../../../../../../removable-discontinuity.md) is addressed at the end.

Write the [Fourier coefficients](../../../../../../fourier-coefficient.md) as

$$
\widehat f(n)=\frac1{2\pi}\int_{-\pi}^{\pi}f(t)e^{-int}\,dt.
$$

Translation multiplies each coefficient by a unimodular factor and preserves the hypothesis, so place the proposed discontinuity at zero. Suppose the finite limits are $A=f(0^-)$ and $B=f(0^+)$. For $0<r<1$, geometric summation gives the [Poisson kernel on the circle](../../../../../../poisson-kernel-on-the-circle.md) and the [conjugate Poisson kernel on the circle](../../../../../../conjugate-poisson-kernel-on-the-circle.md):

$$
\begin{aligned}
P_r(t)&=1+2\sum_{n\ge1}r^n\cos(nt)
=\frac{1-r^2}{1-2r\cos t+r^2},\\
Q_r(t)&=2\sum_{n\ge1}r^n\sin(nt)
=\frac{2r\sin t}{1-2r\cos t+r^2}.
\end{aligned}
$$

These series converge uniformly and absolutely for each $r<1$. Therefore they may be integrated term by term against the [Lebesgue integrable function](../../../../../../lebesgue-integrable-function.md) $f$. With normalized [convolution](../../../../../../convolution.md), $P_r$ has multiplier $r^{|n|}$, while $Q_r$ has multiplier $-i\operatorname{sgn}(n)r^{|n|}$ for $n\ne0$ and zero at $n=0$. More explicitly, at zero,

$$
\begin{aligned}
(P_r*f)(0)&=\widehat f(0)+\sum_{n\ge1}r^n[\widehat f(n)+\widehat f(-n)],\\
(Q_r*f)(0)&=-i\sum_{n\ge1}r^n[\widehat f(n)-\widehat f(-n)].
\end{aligned}
$$

The assumed vanishing of negative [Fourier coefficients](../../../../../../fourier-coefficient.md) thus proves, rather than presupposes, the conjugate relation

$$
\boxed{(Q_r*f)(0)=-i\bigl((P_r*f)(0)-\widehat f(0)\bigr)}.
$$

We next show that the right-hand side is bounded as $r\uparrow1$. The kernel $P_r$ is positive and even, and its normalized integral is one by its series. Its mass outside any fixed $(-\delta,\delta)$ tends to zero; in fact its supremum there is $O_\delta(1-r)$. On $(-\delta,0)$, $f$ is uniformly close to $A$ for sufficiently small $\delta$, and on $(0,\delta)$ it is uniformly close to $B$. Evenness places asymptotically half the mass on each side. The outside contribution tends to zero because $f$ is integrable and the outside kernel tends uniformly to zero. Bounding the inside errors by the one-sided approximation errors gives

$$
(P_r*f)(0)\longrightarrow\frac{A+B}{2}.
$$

Hence $(Q_r*f)(0)$ is bounded by the proved conjugate relation.

On the other hand, oddness of $Q_r$ gives

$$
(Q_r*f)(0)=\frac1{2\pi}\int_0^\pi Q_r(t)\,[f(-t)-f(t)]\,dt.
$$

For $0<\delta<\pi$, differentiating $1-2r\cos t+r^2$ proves the exact identity

$$
\int_0^\delta Q_r(t)\,dt
=\log\frac{1-2r\cos\delta+r^2}{(1-r)^2}
=2\log\frac1{1-r}+O_\delta(1).
$$

Also $Q_r\ge0$ on $(0,\pi)$ and is uniformly bounded on $[\delta,\pi]$ as $r\uparrow1$. Write $f(-t)-f(t)=A-B+e(t)$ with $e(t)\to0$ as $t\downarrow0$. The integral over $[\delta,\pi]$ is $O_\delta(1)$ by integrability. Given any $\eta>0$, choose $\delta$ so that $|e(t)|\le\eta$ on $(0,\delta)$. Positivity and the preceding identity show that the near-zero error, divided by $\log(1/(1-r))$, has limiting upper bound at most $\eta/\pi$. Letting $\eta\downarrow0$ proves

$$
\boxed{\frac{(Q_r*f)(0)}{\log(1/(1-r))}\longrightarrow\frac{A-B}{\pi}}.
$$

Boundedness of the numerator makes the left side tend to zero. Therefore $A=B$. This proves [one-sided Fourier spectrum excludes jumps](../../../../../../one-sided-fourier-spectrum-excludes-jumps.md), and supplies the required conjugate-sum argument in full.

There is a point-value qualification to the phrase “first kind.” If it means finite unequal one-sided limits, the proof establishes exactly the stated result. If the definition also includes removable discontinuities, the literal statement is false for an arbitrary integrable representative: the function that equals zero everywhere except $f(0)=1$ has every [Fourier coefficient](../../../../../../fourier-coefficient.md) zero but a removable discontinuity at zero. Integral hypotheses cannot detect a change at one point. Thus **no jump is possible; equal one-sided limits need not equal an arbitrarily assigned point value**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
