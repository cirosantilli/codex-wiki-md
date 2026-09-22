<h1 id="9b/solution">Solution</h1>

↑ **Parent:** [9B](../9b.md)

During ejection, the remaining [mass](../../../../../mass.md) is $m(t)=m_o+m_w-Qt$, and the water is exhausted at $t_c=m_w/Q$. Consider the [momentum](../../../../../momentum.md) of the octopus and the small portion of water expelled during $dt$. Initially it is $mu$. At the end of this interval, the remaining body has [mass](../../../../../mass.md) $m-Q\,dt$ and [velocity](../../../../../velocity.md) $u+du$, while the expelled [mass](../../../../../mass.md) $Q\,dt$ has laboratory [velocity](../../../../../velocity.md) $u-V$, to first order. Hence the total final [momentum](../../../../../momentum.md) is

$$
(m-Q\,dt)(u+du)+Q\,dt(u-V)=mu+m\,du-QV\,dt+o(dt).
$$

The external [impulse](../../../../../impulse.md) from [quadratic drag](../../../../../quadratic-drag.md) is $-\alpha u^2dt$. Equating this to the change in total [momentum](../../../../../momentum.md), and dividing by $dt$, proves the [equation of motion](../../../../../equation-of-motion.md)

$$
\boxed{m\frac{du}{dt}=QV-\alpha u^2.}
$$

The outgoing water's [momentum](../../../../../momentum.md) flux is essential: applying $d(mu)/dt$ to the remaining body alone would omit it.

For [dimensional analysis](../../../../../dimensional-analysis.md), the independent physical inputs are $m_o,m_w,Q,V,\alpha$, with dimensions

$$
[m_o]=[m_w]=\mathsf M,\quad[Q]=\mathsf M\mathsf T^{-1},\quad[V]=\mathsf L\mathsf T^{-1},\quad[\alpha]=\mathsf M\mathsf L^{-1}.
$$

The scales $m_o$, $m_o/Q$ and $Vm_o/Q$ fix units of [mass](../../../../../mass.md), time and length. In these units, the only remaining independent [dimensionless variables](../../../../../dimensionless-variable.md) are

$$
\boxed{\lambda=\frac{m_w}{m_o},\qquad\mu=\frac{\alpha V}{Q}.}
$$

For example, with $s=Qt/m_o$ and $w=u/V$, the [equation of motion](../../../../../equation-of-motion.md) becomes $(1+\lambda-s)\,dw/ds=1-\mu w^2$, with $w(0)=0$ and ejection ending at $s=\lambda$. Thus the dimensionless terminal value depends only on $\lambda,\mu$, proving $u_c=Vf(\lambda,\mu)$.

For its explicit value, put $m_0=m_o+m_w$ and $U=\sqrt{QV/\alpha}$. The initially stationary solution stays below $U$, since the [acceleration](../../../../../acceleration.md) vanishes at $U$ and is positive below it. [Separation of variables](../../../../../separation-of-variables.md) gives

$$
\int_0^{u(t)}\frac{dv}{QV-\alpha v^2}=\int_0^t\frac{d\tau}{m_0-Q\tau}.
$$

The two integrals yield

$$
\frac{1}{\sqrt{\alpha QV}}\operatorname{artanh}\frac{u(t)}U=\frac1Q\log\frac{m_0}{m_0-Qt}.
$$

This is [constant mass-loss propulsion with quadratic drag](../../../../../constant-mass-loss-propulsion-with-quadratic-drag.md). At $t_c$, the remaining [mass](../../../../../mass.md) is $m_o$, giving

$$
\boxed{u_c=\sqrt{\frac{QV}{\alpha}}\tanh\left(\sqrt{\frac{\alpha V}{Q}}\log\frac{m_o+m_w}{m_o}\right)
=\frac{V}{\sqrt\mu}\tanh\bigl(\sqrt\mu\log(1+\lambda)\bigr).}
$$

Thus $f(\lambda,\mu)=\mu^{-1/2}\tanh(\sqrt\mu\log(1+\lambda))$, verifying the required dimensional form. The limit as drag tends to zero is $V\log(1+\lambda)$, the ordinary [rocket equation](../../../../../rocket-equation.md), while the positive-drag answer is below the [terminal velocity](../../../../../terminal-velocity.md) $U$.

## ↑ Ancestors (10)

1. [9B](../9b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
