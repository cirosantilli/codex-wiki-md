<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We prove [finite propagation speed](../../../../../../finite-propagation-speed.md) using a [shrinking cone energy argument](../../../../../../shrinking-cone-energy-argument.md). Fix $T>0$ and $x_*$, and suppose the [Cauchy data](../../../../../../cauchy-data.md) vanish on $B(x_*,T)$. For $0\leq s<T$, define the local [wave energy](../../../../../../wave-energy.md)

$$
e=\frac12\bigl(\phi_t^2+|\nabla\phi|^2\bigr),\qquad
E(s)=\int_{B(x_*,T-s)}e(s,x)\,dx.
$$

The homogeneous [wave equation](../../../../../../wave-equation-split.md) gives the local [conservation law](../../../../../../conservation-law.md)

$$
\partial_t e=\nabla\cdot(\phi_t\nabla\phi).
$$

Differentiate the integral over the moving ball. Its boundary moves inward with speed one, so the [divergence theorem](../../../../../../divergence-theorem.md) gives

$$
E'(s)=\int_{\partial B(x_*,T-s)}\bigl(\phi_t\partial_n\phi-e\bigr)\,dS
=-\frac12\int_{\partial B(x_*,T-s)}
\left((\phi_t-\partial_n\phi)^2+|\nabla_{\mathrm{tan}}\phi|^2\right)\,dS\leq0.
$$

Here $n$ is the outward [unit normal](../../../../../../unit-normal.md), $\partial_n$ the [normal derivative](../../../../../../normal-derivative.md), and $\nabla_{\mathrm{tan}}$ the component of the [gradient](../../../../../../gradient.md) tangent to the boundary. Since $E(0)=0$ and $e\geq0$, we have $E(s)=0$. Hence both $\phi_t$ and $\nabla\phi$ vanish inside the backward [light cone](../../../../../../light-cone.md). Integrating $\phi_t(s,x_*)=0$ from the zero initial displacement gives $\phi(s,x_*)=0$; [continuity](../../../../../../continuous-function.md) then gives $\phi(T,x_*)=0$.

Applying the same [energy estimate](../../../../../../energy-estimate.md) to the difference of two solutions proves the [domain of dependence](../../../../../../domain-of-dependence.md) assertion. If $\operatorname{dist}(x_*,K)>T$, the initial ball misses $K$, and the preceding argument proves the stated [support](../../../../../../support.md) bound. **No disturbance propagates faster than one.**

## ↑ Ancestors (11)

1. [2](../2.md)
2. [1](../../1.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
