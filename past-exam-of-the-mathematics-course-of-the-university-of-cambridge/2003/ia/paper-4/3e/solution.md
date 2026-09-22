<h1 id="3e/solution">Solution</h1>

↑ **Parent:** [3E](../3e.md)

Let $s=m_0/T$ be the constant fuel [mass](../../../../../mass.md) rate, and let $q(t)=M+m_0-st$ be the remaining rocket [mass](../../../../../mass.md). Take positive motion opposite to the exhaust direction. Over a short interval $dt$, [momentum conservation](../../../../../momentum-conservation.md) including the [mass](../../../../../mass.md) $s\,dt$ expelled at [velocity](../../../../../velocity.md) $v-u$ gives

$$
qv-\mu qg\,dt=(q-s\,dt)(v+dv)+s\,dt(v-u)+o(dt).
$$

Consequently, while the rocket slides forward,

$$
q\dot v=su-\mu qg,\qquad \dot v=\frac{su}{M+m_0-st}-\mu g.
$$

This is the [constant-burn rocket with ground friction](../../../../../constant-burn-rocket-with-ground-friction.md). Assuming forward sliding begins immediately and persists, integration from rest gives

$$
v(t)=u\log\frac{M+m_0}{M+m_0-st}-\mu gt,
$$

and hence

$$
\boxed{v(T)=u\log\frac{M+m_0}{M}-\mu gT}.
$$

A necessary physical assumption is missing from the printed request. With a common [static friction](../../../../../static-friction.md) and [kinetic friction](../../../../../kinetic-friction.md) coefficient $\mu>0$, immediate motion requires $su\geq\mu g(M+m_0)$; equality allows motion as soon as fuel loss lowers the normal force. Then the acceleration is nonnegative initially and increases thereafter, so forward sliding is consistent. Without this assumption the displayed expression need not be the final [speed](../../../../../speed.md) and can even be negative.

For completeness, the physical rest/sliding solution with these equal coefficients is as follows. If $su\leq\mu gM$, the rocket never starts before burnout and its final [speed](../../../../../speed.md) is zero. If $\mu gM<su<\mu g(M+m_0)$, [static friction](../../../../../static-friction.md) initially balances the thrust and release occurs at

$$
t_s=\frac{M+m_0-su/(\mu g)}s,\qquad q_s=\frac{su}{\mu g}.
$$

Integrating only the sliding interval yields

$$
\boxed{v(T)=u\log(q_s/M)-\mu g(T-t_s)}.
$$

This [speed](../../../../../speed.md) is positive because, with $y=q_s/M>1$, it equals $u[\log y-1+1/y]$, whose derivative with respect to $y$ is $(y-1)/y^2>0$. The $\mu=0$ case recovers the frictionless [rocket equation](../../../../../rocket-equation.md). If static and kinetic coefficients differ, the release condition uses the static coefficient and the subsequent integral uses the kinetic coefficient; the prompt supplies no second coefficient.

## ↑ Ancestors (10)

1. [3E](../3e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
