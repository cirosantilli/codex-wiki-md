<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\alpha=3$, let $F_n$ denote the time factor normalized by $F_n(0)=0$, $F_n'(0)=1$. By [superposition](../../../../../../superposition-principle.md) the [Fourier sine series](../../../../../../fourier-sine-series.md) solution is

$$
y(x,t)=e^{-3t}\sum_{n=1}^\infty b_nF_n(t)\sin(nx),\qquad
F_n(t)=\begin{cases}
\dfrac{\sinh(\sqrt{9-n^2}\,t)}{\sqrt{9-n^2}},&n<3,\\
t,&n=3,\\
\dfrac{\sin(\sqrt{n^2-9}\,t)}{\sqrt{n^2-9}},&n>3.
\end{cases}
$$

At $t=0$, its [initial velocity](../../../../../../initial-velocity.md) is $\sum_{n\geq1}b_n\sin(nx)=\sin^2x$. Multiply by $\sin(mx)$, integrate on $[0,\pi]$, and use the permitted interchange and [Fourier orthogonality](../../../../../../fourier-orthogonality.md). This yields the requested [integral](../../../../../../integral-split.md) expression

$$
\boxed{b_n=\frac2\pi\int_0^\pi\sin^2x\sin(nx)\,dx.}
$$

Under $x\mapsto\pi-x$, $\sin^2x$ is unchanged and $\sin(n(\pi-x))=(-1)^{n+1}\sin(nx)$. Hence every even-index [Fourier coefficient](../../../../../../fourier-coefficient.md) is zero, including $b_2$.

For odd $n$, use $\sin^2x=(1-\cos2x)/2$ and the [product-to-sum formula](../../../../../../product-to-sum-formula.md):

$$
\begin{aligned}
\int_0^\pi\sin^2x\sin(nx)\,dx
&=\frac1n-\frac12\left(\frac1{n+2}+\frac1{n-2}\right)\\
&=-\frac4{n(n^2-4)}.
\end{aligned}
$$

Thus

$$
\boxed{b_n=\begin{cases}-\dfrac8{\pi n(n^2-4)},&n\text{ odd},\\0,&n\text{ even}.\end{cases}}
$$

In particular $b_1=8/(3\pi)$ and $b_3=-8/(15\pi)$. An explicit version of the [solution of a differential equation](../../../../../../solution-of-a-differential-equation.md) is

$$
\boxed{y(x,t)=e^{-3t}\left[
\frac8{3\pi}\frac{\sinh(\sqrt8\,t)}{\sqrt8}\sin x
-\frac8{15\pi}t\sin3x
-\frac8\pi\sum_{\substack{n\geq5\\n\text{ odd}}}
\frac{\sin(\sqrt{n^2-9}\,t)\sin(nx)}{n(n^2-4)\sqrt{n^2-9}}
\right].}
$$

Only the first, [overdamped](../../../../../../overdamping.md) [normal mode](../../../../../../normal-mode.md), the third, [critically damped](../../../../../../critical-damping.md) [normal mode](../../../../../../normal-mode.md), and the odd [underdamped](../../../../../../underdamping.md) [normal modes](../../../../../../normal-mode.md) of index at least five occur. No odd-index [Fourier coefficient](../../../../../../fourier-coefficient.md) vanishes.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
