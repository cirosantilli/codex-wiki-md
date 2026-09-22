<h1 id="a/2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $H(t)=\int_0^tE(r)\,dr$. For positive [rainfall](../../../../../rainfall.md) excess it is [strictly increasing](../../../../../strictly-increasing-function.md). The [characteristic equations](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) are

$$
\frac{dh}{dt}=E(t),\qquad\frac{ds}{dt}=\frac53h^{2/3}.
$$

A [characteristic](../../../../../characteristic-of-a-field.md) starting on the initial line at position $s_0\geq0$ has $h=H(t)$ and $s=s_0+S_0(t)$, where $S_0(t)=\frac53\int_0^tH(r)^{2/3}\,dr$. It supplies the downstream region $s\geq S_0(t)$.

A [characteristic](../../../../../characteristic-of-a-field.md) emitted at the upstream boundary at time $\tau$ has

$$
\boxed{h=H(t)-H(\tau),\qquad s=\frac53\int_\tau^t[H(r)-H(\tau)]^{2/3}\,dr.}
$$

For fixed $t$, this position decreases strictly from $S_0(t)$ to zero as $\tau$ increases from zero to $t$. Thus it uniquely determines $\tau=\tau(s,t)$ in the remaining region. The complete solution is

$$
\boxed{h(s,t)=\begin{cases}H(t)-H(\tau(s,t)),&0\leq s\leq S_0(t),\\H(t),&s\geq S_0(t).\end{cases}}
$$

The formulas agree at the separator, satisfy both zero data and cannot form a [characteristic](../../../../../characteristic-of-a-field.md) crossing while $E>0$. At the upstream endpoint $\tau=t$, height is zero.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
