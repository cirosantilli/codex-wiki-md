<h1 id="12a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0\le k<1$, the first burn reduces the total [mass](../../../../../../mass.md) from $M+m_0$ to $M+(1-k)m_0$. The [rocket equation](../../../../../../rocket-equation.md) therefore gives

$$
v_1=u\log\frac{M+m_0}{M+(1-k)m_0}.
$$

Detachment exerts negligible impulse, so the surviving second stage keeps [velocity](../../../../../../velocity.md) $v_1$. Its initial and final [masses](../../../../../../mass.md) are $(1-k)(M+m_0)$ and $(1-k)M$, respectively. A second application of the [rocket equation](../../../../../../rocket-equation.md) gives

$$
\boxed{v_2=u\log\frac{M+m_0}{M+(1-k)m_0}+u\log\left(1+\frac{m_0}{M}\right).}
$$

For the single-stage comparison from rest, $v_{\rm single}=u\log(1+m_0/M)$. Hence

$$
\boxed{v_2-v_{\rm single}=u\log\frac{M+m_0}{M+(1-k)m_0}\ge0.}
$$

Equality holds at $k=0$; for positive fuel and exhaust speed it is strict when $0<k<1$. This [two-stage rocket with proportional fuel and body masses](../../../../../../two-stage-rocket-with-proportional-fuel-and-body-masses.md) gains speed by discarding inert body [mass](../../../../../../mass.md) before the last burn.

As $k\to1^-$ the expression tends to $2u\log(1+m_0/M)$, but the surviving second-stage [mass](../../../../../../mass.md) also tends to zero. At exactly $k=1$ there is no second stage, so its final [speed](../../../../../../speed.md) is undefined and that limiting formula cannot be assigned to it. The first stage alone reaches the single-stage burnout [speed](../../../../../../speed.md) before detachment. If $m_0=0$, neither design gains speed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12A](../../12a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
