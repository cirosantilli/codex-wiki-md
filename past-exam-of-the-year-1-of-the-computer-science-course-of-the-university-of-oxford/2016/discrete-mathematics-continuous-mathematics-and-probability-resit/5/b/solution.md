<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The given [square wave](../../../../../square-wave.md) agrees almost everywhere with an [odd function](../../../../../odd-function.md) on $(-\pi,\pi)$; its assigned value at the single point $0$ does not affect any [Fourier coefficient](../../../../../fourier-coefficient.md). Thus $a_0=a_n=0$, while

$$
b_n=\frac2\pi\int_0^\pi\sin(nx)\,dx
=\frac{2(1-(-1)^n)}{\pi n}
=\begin{cases}4/(\pi n),&n\text{ odd},\\0,&n\text{ even}.\end{cases}
$$

The [Fourier series](../../../../../fourier-series-split.md) is therefore

$$
\boxed{f(x)=\frac4\pi\sum_{r=0}^{\infty}\frac{\sin((2r+1)x)}{2r+1}\quad(-\pi<x<0\text{ or }0<x<\pi)}.
$$

The [Dirichlet convergence theorem for Fourier series](../../../../../dirichlet-s-theorem-on-fourier-series.md) applies because the periodic extension is piecewise smooth. It gives $f(x)$ at each continuity point and the midpoint $0$ at the jumps, including $x=0$; it does not reproduce the assigned value $f(0)=-1$ there.

At the continuity point $x=\pi/2$, $\sin((2r+1)\pi/2)=(-1)^r$ and $f(\pi/2)=1$. Thus

$$
\boxed{1-\frac13+\frac15-\frac17+\cdots=\frac\pi4}.
$$

No evaluation at a discontinuity or rearrangement of the conditionally convergent series is involved.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics and probability (resit)](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
