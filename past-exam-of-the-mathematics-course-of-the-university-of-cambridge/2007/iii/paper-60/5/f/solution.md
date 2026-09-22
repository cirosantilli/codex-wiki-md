<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For a specified negative-feedback loop with return ratio $L(s)$, let $P$ be its number of open-right-half-plane poles. Let $N_{\mathrm{cw}}$ be the signed clockwise encirclement count of $-1$ by the standard [Nyquist stability criterion](../../../../../../nyquist-stability-criterion.md) contour. Provided the contour does not hit a singularity or the critical point, the number of right-half-plane closed-loop poles is $Z=P+N_{\mathrm{cw}}$. Thus **closed-loop stability requires $N_{\mathrm{cw}}=-P$ and no closed-loop pole on the imaginary axis**, with the usual well-posedness and absence of hidden unstable cancellations. For an already stable return ratio, there must be no encirclement of $-1$ and no passage through it.

The open cavity itself, for $\gamma>0$, has state eigenvalue and transfer-function pole $-\gamma/2$. Its initial transient decays and its impulse response is a direct-feedthrough term plus a decaying exponential. Hence **the open-loop cavity is asymptotically stable and its transfer function is BIBO stable**. The right-half-plane zero at $+\gamma/2$ does not make the open cavity unstable. On the frequency axis,

$$
G(i\omega)=\frac{\omega^2-(\gamma/2)^2+i\gamma\omega}{\omega^2+(\gamma/2)^2},\qquad |G(i\omega)|=1.
$$

Its unit-circle plot passes through $-1$ at $\omega=0$. A [Nyquist stability criterion](../../../../../../nyquist-stability-criterion.md) is a feedback criterion; this passage is not by itself a test of open-plant stability.

If the intended interpretation is a unit negative-feedback loop with $L=G$, then

$$
1+G(s)=\frac{2s}{s+\gamma/2},\qquad \frac{G(s)}{1+G(s)}=\frac{s-\gamma/2}{2s}.
$$

That loop has a pole at zero, so **unit negative feedback is marginal rather than asymptotically stable**, and the critical-point passage correctly prevents a strict Nyquist stability conclusion. Without a specified feedback interconnection, the unambiguous conclusion is the stable open cavity, not that particular closed loop.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [5](../../5.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
