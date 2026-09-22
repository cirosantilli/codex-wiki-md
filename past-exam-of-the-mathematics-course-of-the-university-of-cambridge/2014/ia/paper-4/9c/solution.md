<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

First apply [momentum conservation](../../../../../momentum-conservation.md) to the rocket and the infinitesimal amount of expelled gas. During $dt$, the exhaust [mass](../../../../../mass.md) is $\alpha\,dt$ and its inertial [velocity](../../../../../velocity.md), to first order, is $v-u$. With no dust, the momentum balance is

$$
mv=(m-\alpha\,dt)(v+dv)+\alpha\,dt(v-u)+o(dt).
$$

It gives the [rocket equation](../../../../../rocket-equation.md) **$\boxed{m\dot v=\alpha u}$**, while $\dot m=-\alpha$.

For a [dust-collecting rocket](../../../../../dust-collecting-rocket.md), the incoming dust [mass](../../../../../mass.md) is $\beta v\,dt$ with zero initial [momentum](../../../../../momentum.md). The same balance has rocket [mass](../../../../../mass.md) $m+(\beta v-\alpha)dt$ after the interval, so

$$
mv=\bigl(m+(\beta v-\alpha)dt\bigr)(v+dv)+\alpha\,dt(v-u)+o(dt).
$$

Consequently

$$
\boxed{\dot m=\beta v-\alpha,\qquad m\dot v=\alpha u-\beta v^2.}
$$

The second term in the [acceleration](../../../../../acceleration.md) equation accounts for the [momentum](../../../../../momentum.md) required to bring collected dust up to rocket [speed](../../../../../speed.md).

Set $\lambda=\sqrt{\alpha/(\beta u)}$ and $V=\lambda u$, so $\alpha u=\beta V^2$. As long as the engines operate and $0\leq v<V$, the [velocity](../../../../../velocity.md) increases and time can be eliminated:

$$
\frac{d\log m}{dv}=\frac{v-\lambda^2u}{V^2-v^2}
=-\frac{\lambda-1}{2(V-v)}-\frac{\lambda+1}{2(V+v)}.
$$

Integrating from $v=0$, $m=m_0$, gives

$$
\log\frac m{m_0}=\frac{\lambda-1}{2}\log\frac{V-v}{V}-\frac{\lambda+1}{2}\log\frac{V+v}{V}.
$$

Thus the required [mass](../../../../../mass.md)–[velocity](../../../../../velocity.md) relation is

$$
\boxed{m=\lambda m_0u\sqrt{\frac{(\lambda u-v)^{\lambda-1}}{(\lambda u+v)^{\lambda+1}}}.}
$$

If $\lambda>1$, this formula would give $m\to0$ as $v\to V^-$. In this interval, $\dot m=\beta(v-\lambda^2u)<0$. A real rocket retains positive body [mass](../../../../../mass.md) even after its fuel is gone, and collected dust only increases that residual [mass](../../../../../mass.md). It therefore cannot follow this branch all the way to zero [mass](../../../../../mass.md): **its fuel must run out while $v<\lambda u$**. Indeed the hypothetical time integral $dt/dv=m/[\beta(V^2-v^2)]$ is integrable at $V$ when $\lambda>1$, so even the formal zero-mass endpoint would occur at finite time.

If $0<\lambda<1$, the same relation instead gives $m\to\infty$ as $v\to V^-$. The [mass](../../../../../mass.md) first decreases, reaches its minimum at $v=\lambda^2u$, and then increases because dust arrives faster than fuel is expelled. The time integral now diverges at $V$: under indefinitely maintained thrust, **$v$ approaches $\lambda u$ asymptotically while stored dust grows without bound**. At that limiting [speed](../../../../../speed.md), thrust $\alpha u$ balances the dust-loading term $\beta v^2$, and $\dot m\to\beta u\lambda(1-\lambda)>0$. This is the physical reason the total rocket [mass](../../../../../mass.md) no longer signals fuel exhaustion. A rocket with a finite initial fuel supply still runs out at finite time $t=M_{\rm fuel}/\alpha$ and before reaching $V$; increasing total [mass](../../../../../mass.md) does not create new fuel.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
