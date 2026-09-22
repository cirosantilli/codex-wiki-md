<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First use the usual real-valued, measurable interpretation of the transition data. The complementary squares then imply $|f|\le1$, and the compact support gives $f\in L_2$. Consider the periodization on $[-\pi,\pi]$. For $|t|<2\pi/3$, only $f(t)=1$ contributes. For $2\pi/3\le t\le\pi$, only $f(t)$ and $f(t-2\pi)$ can contribute, and their squares sum to one. For $-\pi\le t\le-2\pi/3$, apply the complementary identity at $t+2\pi$ to obtain $f(t)^2+f(t+2\pi)^2=1$. Therefore the [orthonormal translates and Fourier periodization](../../../../../../orthonormal-translates-and-fourier-periodization.md) identity holds almost everywhere.

Define a periodic [MRA low-pass filter](../../../../../../low-pass-filter-of-a-multiresolution-analysis.md) by prescribing it on $[-\pi,\pi]$:

$$
m(t)=\begin{cases}f(2t),&|t|<2\pi/3,\\0,&2\pi/3\le|t|\le\pi,\end{cases}\qquad m(t+2\pi)=m(t).
$$

In the central band, $f(t)=1$, so $f(2t)=m(t)f(t)$. In the rest of this fundamental interval, both $m(t)$ and $f(2t)$ vanish. If $\pi<|t|<4\pi/3$, reducing $t$ modulo $2\pi$ puts it in an outer band where $m=0$, and again $f(2t)=0$. For $|t|\ge4\pi/3$, both $f(t)$ and $f(2t)$ vanish. Endpoint choices affect only a null set. Thus the [complementary transition bands for a scaling function](../../../../../../complementary-transition-bands-for-a-scaling-function.md) give **both Fourier conditions**, with this explicitly constructed periodic mask.

A concrete real-valued choice, illustrating that the transition constraints are consistent, is

$$
f(t)=\begin{cases}1,&|t|\le2\pi/3,\\\cos\!\left(\dfrac\pi2\left(\dfrac{3|t|}{2\pi}-1\right)\right),&2\pi/3<|t|<4\pi/3,\\0,&|t|\ge4\pi/3.\end{cases}
$$

On the positive transition band put $u=3t/(2\pi)-1\in[0,1]$. The other translate has parameter $1-u$, so the sum is $\cos^2(\pi u/2)+\sin^2(\pi u/2)=1$.

There is a genuine qualification in the printed formulation: it uses ordinary squares without explicitly declaring $f$ real-valued. If arbitrary complex values are allowed, the claimed verification is false. Take $f=1$ for $|t|\le2\pi/3$, $f=0$ for $|t|\ge4\pi/3$, and set

$$
f(t)=i\quad(2\pi/3<t<4\pi/3),\qquad f(t)=\sqrt2\quad(-4\pi/3<t<-2\pi/3).
$$

The printed complementary-square rule holds, including its endpoints: in the interior $i^2+(\sqrt2)^2=1$, while the endpoints pair one with zero. Nevertheless, for $2\pi/3<t<\pi$,

$$
\sum_k|f(t+2\pi k)|^2=|i|^2+|\sqrt2|^2=3.
$$

This compactly supported $L_2$ function is the [Fourier transform](../../../../../../fourier-transform.md) of an $L_2$ function, so it is a counterexample within the natural complex [Hilbert space](../../../../../../hilbert-space-split.md). **The verification is valid for real-valued $f$, or with absolute squares in the transition rule; it is not valid for unrestricted complex $f$ with ordinary squares.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
