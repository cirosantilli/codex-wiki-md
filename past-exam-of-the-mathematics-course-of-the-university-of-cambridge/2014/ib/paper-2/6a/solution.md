<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

Use compatible orientations for the loop and spanning surface. The relevant [Maxwell equations](../../../../../maxwell-equations.md) are

$$
\nabla\cdot\mathbf B=0,\qquad
\nabla\times\mathbf E=-\partial_t\mathbf B.
$$

The [magnetic flux transport for a moving circuit](../../../../../magnetic-flux-transport-for-a-moving-circuit.md) separates the change of the field from the motion of its boundary. To see the boundary term, freeze $\mathbf B$ at time $t$. Orient the closed swept surface as $S(t+\delta t)-S(t)+S'$. Its side element is

$$
d\mathbf S'=-\delta t\,\mathbf v\times d\mathbf r,
$$

to first order. Hence its flux is $-\delta t\oint_C\mathbf B\cdot(\mathbf v\times d\mathbf r)$. By the [divergence theorem](../../../../../divergence-theorem.md) and $\nabla\cdot\mathbf B=0$, the sum of the three fluxes is zero, giving the purely geometric change

$$
\delta\Phi_{\rm shape}
=\delta t\oint_C\mathbf B\cdot(\mathbf v\times d\mathbf r)
=-\delta t\oint_C(\mathbf v\times\mathbf B)\cdot d\mathbf r.
$$

Adding the temporal field change and applying [Stokes theorem](../../../../../stokes-theorem.md) yields

$$
\frac{d\Phi}{dt}
=\int_{S(t)}\partial_t\mathbf B\cdot d\mathbf S
-\oint_C(\mathbf v\times\mathbf B)\cdot d\mathbf r
=-\oint_C(\mathbf E+\mathbf v\times\mathbf B)\cdot d\mathbf r.
$$

Thus

$$
\boxed{\frac{d\Phi}{dt}=-\mathcal E.}
$$

The boundary contribution is the [motional electromotive force](../../../../../motional-electromotive-force.md); the field contribution is [Faraday's law](../../../../../faraday-s-law-of-induction.md).

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
