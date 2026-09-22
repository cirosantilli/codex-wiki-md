<h1 id="31c/solution">Solution</h1>

↑ **Parent:** [31C](../31c.md)

For the [WKB approximation](../../../../../wkb-approximation.md), put $Q(x)=|x|-E$. Away from the [turning points](../../../../../turning-point.md) $x=\pm E$, the forbidden-region solutions have the form $Q^{-1/4}\exp(\pm\int\sqrt Q\,dx)$; in the allowed region put $k(x)=\sqrt{E-|x|}$ and use $k^{-1/2}\exp(\pm i\int k\,dx)$. The decaying tails selected by the [boundary conditions](../../../../../boundary-condition.md) are

$$
y\sim C_+(x-E)^{-1/4}e^{-\frac23(x-E)^{3/2}}\ (x>E),\qquad
y\sim C_-(-x-E)^{-1/4}e^{-\frac23(-x-E)^{3/2}}\ (x<-E).
$$

The simple-turning-point Airy connection formula matches these to

$$
2C_+k(x)^{-1/2}\sin\left(\int_x^E k(s)ds+\frac\pi4\right),\qquad
2C_-k(x)^{-1/2}\sin\left(\int_{-E}^x k(s)ds+\frac\pi4\right).
$$

Compatibility requires the [Bohr-Sommerfeld quantization](../../../../../bohr-sommerfeld-quantization.md) condition

$$
\int_{-E}^E\sqrt{E-|x|}\,dx=\frac43E^{3/2}\sim\pi(n+1/2),
$$

with levels indexed from $n=0$. Therefore

$$
\boxed{E_n\sim\left[\frac{3\pi}{4}(n+1/2)\right]^{2/3},\qquad E_n=O(n^{2/3}).}
$$

The cusp at zero does not alter the leading high-energy count. An exact matching check is available: on $x\ge0$ the decaying solution is $\operatorname{Ai}(x-E)$, and parity at zero imposes $\operatorname{Ai}'(-E)=0$ for even states or $\operatorname{Ai}(-E)=0$ for odd states. Their interlacing large negative zeros give the same combined leading quantization. Reindexing from one changes only the constant phase shift, not the requested growth law.

## ↑ Ancestors (10)

1. [31C](../31c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
