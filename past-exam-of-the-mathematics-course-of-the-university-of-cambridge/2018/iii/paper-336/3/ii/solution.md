<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The transition equation reduces to the [Bessel differential equation](../../../../../../bessel-differential-equation.md) because $d/dT=-Z\,d/dZ$ and $d^2/dT^2=Z^2d^2/dZ^2+Z\,d/dZ$. Thus $Y_{TT}+e^{-2T}Y=0$ becomes $Z^2Y_{ZZ}+ZY_Z+Z^2Y=0$.

The [Bessel function of the first kind](../../../../../../bessel-function-of-the-first-kind.md) has $J_0(Z)=1+O(Z^2)$ at zero, while the [Bessel function of the second kind](../../../../../../bessel-function-of-the-second-kind.md) has $Y_0(Z)=(2/\pi)(\log(Z/2)+\gamma)+O(Z^2|\log Z|)$. Since $\log Z=-T$, these yield a constant and a linear function of $T$, explaining the late-time behavior. At large positive $Z$,

$$
J_0(Z)\sim\sqrt{\frac2{\pi Z}}\cos(Z-\pi/4),\qquad
Y_0(Z)\sim\sqrt{\frac2{\pi Z}}\sin(Z-\pi/4).
$$

Matching $A_0\cos(Z-\pi/4)+B_0\sin(Z-\pi/4)$ to $\sqrt{\pi/2}\sin(\varepsilon^{-1}-Z)$ fixes $A_0=\sqrt{\pi/2}\sin\theta$ and $B_0=-\sqrt{\pi/2}\cos\theta$. The large- and small-argument [asymptotic expansions](../../../../../../asymptotic-expansion.md) thereby connect the oscillatory [WKB approximation](../../../../../../wkb-approximation.md) to the nonoscillatory late-time solution through one [Bessel transition for an exponentially decaying oscillator](../../../../../../bessel-transition-for-an-exponentially-decaying-oscillator.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
