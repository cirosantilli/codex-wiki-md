<h1 id="12a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the total remaining rocket [mass](../../../../../../mass.md) as $\mathcal M=M+m(t)$, with $\dot m=-\alpha$. Over an interval $dt$, an exhaust [mass](../../../../../../mass.md) $dm_e=\alpha\,dt$ is expelled backwards with inertial [velocity](../../../../../../velocity.md) $v-u$ to first order. Applying [momentum conservation](../../../../../../momentum-conservation.md) to the rocket and this exhaust gives

$$
\mathcal M v=(\mathcal M-dm_e)(v+dv)+dm_e(v-u)+o(dt).
$$

Cancellation and division by $dt$ give the [rocket equation](../../../../../../rocket-equation.md)

$$
\boxed{(M+m)\frac{dv}{dt}=\alpha u.}
$$

With $M>0$, $m(t)=m_0-\alpha t$, and $0\le t\le m_0/\alpha$, integration gives

$$
v(t)-v_0=u\log\frac{M+m_0}{M+m(t)}.
$$

At burnout,

$$
\boxed{v_{\rm final}=v_0+u\log\left(1+\frac{m_0}{M}\right).}
$$

The logarithm depends on the [mass](../../../../../../mass.md) ratio, not on the burn rate. This follows from [momentum conservation](../../../../../../momentum-conservation.md) of the complete rocket–exhaust system; applying a constant-mass equation directly to the rocket alone would omit the momentum carried away.

## ↑ Ancestors (11)

1. [A](../a.md)
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
