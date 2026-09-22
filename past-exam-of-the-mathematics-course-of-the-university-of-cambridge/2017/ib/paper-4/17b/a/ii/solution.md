<h1 id="17b/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For each injection time $\tau$, let $v_\tau$ solve the homogeneous [Cauchy problem for a partial differential equation](../../../../../../../cauchy-problem.md) with initial profile $v_\tau(x,\tau)=h(x,\tau)$. Its representation by the [fundamental solution of a linear differential operator](../../../../../../../fundamental-solution-of-a-linear-differential-operator.md) is

$$
v_\tau(x,t)=\int_\mathbb R F(x-y,t-\tau)h(y,\tau)\,dy\qquad(t>\tau).
$$

The causal [Green function](../../../../../../../green-s-function.md) and [Duhamel principle](../../../../../../../duhamel-s-principle.md) give

$$
\boxed{\phi(x,t)=\int_0^t v_\tau(x,t)\,d\tau
=\int_0^t\int_\mathbb R F(x-y,t-\tau)h(y,\tau)\,dy\,d\tau}.
$$

For [smooth](../../../../../../../smooth-function.md) forcing with sufficient decay, differentiating this formula gives

$$
\phi_t=h(x,t)+\int_0^t\partial_t v_\tau\,d\tau
=h(x,t)+K\phi_{xx},\qquad \phi(x,0)=0.
$$

The boundary term uses the [Dirac delta function](../../../../../../../dirac-delta-function.md) limit of $F$, not a finite pointwise value of $F(x,0)$. The same formula extends to weaker forcing in an appropriate integrable or [distribution](../../../../../../../distribution-mathematical-analysis.md) sense. Physically, each short time interval adds $h(\cdot,\tau)d\tau$ to the temperature profile; that addition subsequently undergoes homogeneous [diffusion equation](../../../../../../../diffusion-equation-split.md). The total solution is the superposition of all such diffusing injections.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
