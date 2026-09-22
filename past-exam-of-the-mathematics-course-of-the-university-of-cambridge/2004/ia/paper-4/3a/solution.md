<h1 id="3a/solution">Solution</h1>

↑ **Parent:** [3A](../3a.md)

Choose the positive direction along the incoming car's [velocity](../../../../../velocity.md). Treat each car as a translating body, take $m_1,m_2>0$, and neglect external impulse, rotation and [energy](../../../../../energy.md) losses during the short [elastic collision](../../../../../elastic-collision.md). If $v_1,v_2$ are the final signed [velocities](../../../../../velocity.md), [conservation of momentum](../../../../../momentum-conservation.md) and [conservation of energy](../../../../../conservation-of-energy.md) give

$$
m_1U_1=m_1v_1+m_2v_2,\qquad
m_1U_1^2=m_1v_1^2+m_2v_2^2.
$$

Factoring the second relation and using the first gives $U_1+v_1=v_2$ on the collision branch. The other algebraic branch, $v_1=U_1,v_2=0$, describes no impulse and cannot describe separating bodies after contact. Solving the collision branch yields

$$
\boxed{v_1=\frac{R-1}{R+1}U_1,\qquad v_2=\frac{2R}{R+1}U_1,\qquad R=\frac{m_1}{m_2}.}
$$

For $0<R<1$ the first car rebounds and the second moves forwards. At $R=1$ the first stops and the second takes its original [velocity](../../../../../velocity.md). For $R>1$ both move forwards, with $v_2-v_1=U_1>0$, so they separate. In the limits $R\to0$ and $R\to\infty$, the first car's [velocity](../../../../../velocity.md) approaches $-U_1$ and $U_1$, respectively.

For the deformable car, take $y=0$ at first contact. The resisting [force](../../../../../force.md) does negative [work](../../../../../work.md). The [work-energy theorem](../../../../../work-energy-theorem.md) therefore gives

$$
\frac12Mv(y)^2=\frac12MV^2-\int_0^y\frac{ds}{\sqrt{L-s}}
=\frac12MV^2-2\bigl(\sqrt L-\sqrt{L-y}\bigr).
$$

At the first stop $v=0$, whence $\sqrt{L-y}=\sqrt L-MV^2/4$. The [speed](../../../../../speed.md) bound ensures that this right-hand side is positive, so squaring introduces no extraneous solution. The stopping compression is

$$
\boxed{y=L-\left(\sqrt L-\frac{MV^2}{4}\right)^2
=\frac{MV^2\sqrt L}{2}-\frac{M^2V^4}{16}.}
$$

For $0<V<2L^{1/4}/M^{1/2}$ this lies strictly between $0$ and $L$, as required before complete crushing. The coefficient in the stipulated [force](../../../../../force.md) law is taken in its stated normalization.

## ↑ Ancestors (10)

1. [3A](../3a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
