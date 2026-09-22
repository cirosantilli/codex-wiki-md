<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Dupuit approximation](../../../../../dupuit-approximation.md): the saturated region is shallow enough that [hydrostatic pressure](../../../../../hydrostatic-pressure.md) is $p=\rho g(h-z)$ and flow is predominantly horizontal. [Darcy's law](../../../../../darcy-law.md) then gives the horizontal [Darcy velocity](../../../../../darcy-velocity.md) $u_x=-u_b(1+\beta z)h_x$, where $u_b=k_0\rho g/\mu$. Integrating through the saturated depth gives the [volume flux per unit width](../../../../../volume-flux-per-unit-width.md)

$$
q=\int_0^h u_x\,dz=-u_b\left(h+\frac\beta2h^2\right)h_x.
$$

The stored water volume per unit area is $\phi h$, so [mass conservation](../../../../../mass-conservation.md) yields the [unconfined aquifer with depth-dependent permeability](../../../../../unconfined-aquifer-with-depth-dependent-permeability.md) equation

$$
\boxed{\phi h_t=u_b\partial_x\left[\left(h+\frac\beta2h^2\right)h_x\right]+R,\qquad h(0,t)=0,\qquad q(L,t)=0.}
$$

Define the positive river discharge by $Q(t)=-q(0,t)$. A useful check on all subsequent results is the integrated [mass conservation](../../../../../mass-conservation.md) law

$$
\phi\frac d{dt}\int_0^Lh\,dx=RL-Q.
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
