<h1 id="5a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Away from the impulse, the [harmonic oscillator equation](../../../../../../simple-harmonic-motion.md) has a [homogeneous solution](../../../../../../homogeneous-solution.md). Before $x=\pi/2$, the [initial conditions](../../../../../../initial-condition.md) select $y=\cos x$. The [jump condition for an impulse](../../../../../../jump-condition-for-an-impulse.md) requires continuity of $y$ and a unit jump in $y'$: a jump in $y$ would produce a derivative of the [Dirac delta distribution](../../../../../../dirac-delta-function.md), which is absent from the forcing, while integrating through the impulse gives $[y']=1$.

Just before the impulse, $y=0$ and $y'=-1$. Just afterwards, $y=0$ and $y'=0$, so uniqueness for the [harmonic oscillator equation](../../../../../../simple-harmonic-motion.md) makes the subsequent solution identically zero. Equivalently the causal response is $H(x-\pi/2)\sin(x-\pi/2)$, with $H$ the [Heaviside step function](../../../../../../heaviside-step-function.md), and it cancels the original oscillation.

**The solution is**

$$
\boxed{y(x)=\cos x+H(x-\pi/2)\sin(x-\pi/2)=\begin{cases}\cos x,&0\leq x<\pi/2,\\0,&x\geq\pi/2.\end{cases}}
$$

The [impulse cancellation of a harmonic oscillator](../../../../../../impulse-cancellation-of-a-harmonic-oscillator.md) produces a continuous graph with a corner at $(\pi/2,0)$, followed by a horizontal zero line.

<a id="5a/a/image-an-impulse-cancels-the-oscillator-at-zero-displacement"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2-impulse.png)

**[Figure 1](#5a/a/image-an-impulse-cancels-the-oscillator-at-zero-displacement). An impulse cancels the oscillator at zero displacement**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5A](../../5a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
