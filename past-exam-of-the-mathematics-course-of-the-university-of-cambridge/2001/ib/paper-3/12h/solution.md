<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

Assume $0<a<b<l$ for the interior pulse; endpoint variants use the same coefficient formula. Orthogonality of the [Fourier sine basis](../../../../../fourier-sine-basis.md) gives

$$
b_n=\frac2l\int_a^b\sin\frac{n\pi x}{l}\,dx=\frac{2}{n\pi}\left(\cos\frac{n\pi a}{l}-\cos\frac{n\pi b}{l}\right),\qquad
f(x)\sim\sum_{n\ge1}b_n\sin\frac{n\pi x}{l}.
$$

The [Fourier sine series](../../../../../fourier-sine-series.md) equals $f$ at its interior continuity points and takes value $1/2$ at the jumps $a,b$; the sine series is zero at both endpoints. Thus it does not retain an arbitrarily assigned value at a jump.

For the string, write $y(x,t)=\sum_{n\ge1}q_n(t)\sin(n\pi x/l)$. The [wave equation on a string](../../../../../wave-equation-on-a-string.md) gives

$$
q_n''+\left(\frac{n\pi c}{l}\right)^2q_n=0,\qquad q_n(0)=0,\qquad q_n'(0)=\frac2l\sin\frac{n\pi}{4}.
$$

The last equality is the [Fourier sine series](../../../../../fourier-sine-series.md) of the [Dirac delta](../../../../../dirac-delta-function.md) at $l/4$. Solving the modal [ordinary differential equations](../../../../../ordinary-differential-equation.md) gives

$$
\boxed{y(x,t)=\frac{2}{\pi c}\sum_{n=1}^{\infty}\frac{\sin(n\pi/4)\sin(n\pi x/l)\sin(n\pi ct/l)}n.}
$$

This [impulsively struck fixed-end string](../../../../../impulsively-struck-fixed-end-string.md) is understood as a [distributional weak solution](../../../../../weak-solution.md); the initial velocity is a distribution, not a classical continuous function.

To evaluate the requested time, take the odd $2l$-periodic extension $v$ of $\delta(x-l/4)$ and use the [D'Alembert formula](../../../../../d-alembert-s-formula.md) $y=(2c)^{-1}\int_{x-ct}^{x+ct}v(s)\,ds$. At $ct=l/2$, the interval contains the positive impulse at $l/4$. For $x<l/4$, it also contains the negative reflected impulse at $-l/4$, so the contributions cancel. For $l/4<x<3l/4$ only the positive impulse contributes. For $x>3l/4$ neither contributes. Thus the midpoint-valued [Fourier series](../../../../../fourier-series-split.md) gives

$$
\boxed{y\left(x,\frac{l}{2c}\right)=\begin{cases}0,&0\le x<l/4\text{ or }3l/4<x\le l,\\1/(2c),&l/4<x<3l/4,\\1/(4c),&x=l/4\text{ or }x=3l/4.\end{cases}}
$$

The discontinuity values are a convention for the Fourier representative and do not affect the distribution. The sketch shows the reflected negative front cancelling the left portion of the initially generated plateau.

<a id="12h/image-fixed-end-string-at-time-l-divided-by-2c-showing-the-plateau-and-midpoint-values-at-the-two-jump-fronts"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3-struck-string.png)

**[Figure 1](#12h/image-fixed-end-string-at-time-l-divided-by-2c-showing-the-plateau-and-midpoint-values-at-the-two-jump-fronts). Fixed-end string at time l divided by 2c, showing the plateau and midpoint values at the two jump fronts**.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
