<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The upward jump at $-1/2$ creates a [rarefaction wave](../../../../rarefaction-wave.md) with $u=(x+1/2)/t$, bounded by the characteristic lines $x=-1/2$ and $x=t-1/2$. The downward jump at zero joins the states $1,0$, so part (a) gives the shock position $s(t)=t/2$. The intervening plateau exists exactly while $t-1/2<t/2$, or $t<1$. The fan satisfies the [Inviscid Burgers equation](../../../../inviscid-burgers-equation.md) classically and matches the constant branches continuously; the shock satisfies the [Rankine-Hugoniot condition](../../../../rankine-hugoniot-conditions.md) and is causal because $1>1/2>0$. Its initial trace is the prescribed pulse.

At $t=1$, the fan reaches the shock at $x=1/2$. Subsequently the states immediately to its left and right are $(s(t)+1/2)/t$ and zero, so

$$
\dot s=\frac{s+1/2}{2t},\qquad s(1)=\frac12.
$$

Solving gives $s(t)+1/2=\sqrt t$. Thus the continuation is

$$
\boxed{u(x,t)=\begin{cases}(x+1/2)/t,&-1/2<x<\sqrt t-1/2,\\0,&\text{otherwise},\end{cases}\qquad t\geq1,\qquad s(t)=\sqrt t-\frac12}.
$$

Values assigned precisely at the shock do not affect the [weak solution](../../../../weak-solution.md). Its speed $1/(2\sqrt t)$ lies strictly between the left state $1/\sqrt t$ and zero, so it remains a causal [entropy shock](../../../../entropy-shock.md). The area under the triangular profile is $\tfrac12(\sqrt t)(1/\sqrt t)=1/2$, checking conservation of the initial mass. This is the [rectangular pulse solution of the inviscid Burgers equation](../../../../rectangular-pulse-solution-of-the-inviscid-burgers-equation.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the applied partial differential equations course of the University of Oxford](../../../split.md)
5. [Applied partial differential equations course of the University of Oxford](../../../../applied-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
