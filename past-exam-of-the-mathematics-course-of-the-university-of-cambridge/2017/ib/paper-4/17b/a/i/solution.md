<h1 id="17b/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $K>0$. For $t>0$, the diffusion [fundamental solution of a linear differential operator](../../../../../../../fundamental-solution-of-a-linear-differential-operator.md) $F$ satisfies $(\partial_t-K\partial_x^2)F=0$ and has initial value $\delta(x)$ in the sense of [distributions](../../../../../../../distribution-mathematical-analysis.md):

$$
\boxed{\lim_{t\downarrow0}\int_\mathbb R F(x,t)\psi(x)\,dx=\psi(0)}
$$

for every [smooth](../../../../../../../smooth-function.md) compactly supported [test function](../../../../../../../test-function.md) $\psi$. With the usual spatial decay it has unit mass. Equivalently the causal extension $\Theta(t)F(x,t)$ is a [retarded fundamental solution](../../../../../../../retarded-fundamental-solution.md) satisfying $(\partial_t-K\partial_x^2)(\Theta F)=\delta(x)\delta(t)$.

The causal [Green function](../../../../../../../green-s-function.md) is zero for $t<\tau$ and satisfies

$$
\boxed{(\partial_t-K\partial_x^2)G(x,t;y,\tau)=\delta(x-y)\delta(t-\tau)}.
$$

For $t>\tau$ it solves the homogeneous [diffusion equation](../../../../../../../diffusion-equation-split.md), and its initial jump is $G(x,\tau^+;y,\tau)=\delta(x-y)$, again distributionally. The natural spatial decay and a standard bounded or integrable solution class specify the usual kernel, avoiding unrestricted growing solutions. The PDE acts on $x,t$; $y,\tau$ label the location and time of the unit impulse. Values of the [Heaviside step function](../../../../../../../heaviside-step-function.md) exactly at the jump do not affect these [distribution](../../../../../../../distribution-mathematical-analysis.md) identities.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [17B](../../../17b.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
