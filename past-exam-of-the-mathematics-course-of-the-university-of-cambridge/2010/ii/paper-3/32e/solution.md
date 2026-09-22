<h1 id="32e/solution">Solution</h1>

↑ **Parent:** [32E](../32e.md)

Integrating the vector-field equations gives the one-parameter transformations

$$
\boxed{(x,t,v)\longmapsto(e^{\alpha s}x,e^{\beta s}t,e^{\gamma s}v).}
$$

Under this scaling, $v_t,v^2v_x,v_{xxx}$ have weights $\gamma-\beta,3\gamma-\alpha,\gamma-3\alpha$. Equality of all three weights gives

$$
\boxed{\beta=3\alpha,\qquad\gamma=-\alpha.}
$$

Thus the nontrivial [Lie point symmetry](../../../../../lie-point-symmetry.md) generator can be normalized to $x\partial_x+3t\partial_t-v\partial_v$.

For the [Miura transformation](../../../../../miura-transformation.md) $u=v^2+v_x$, direct [differentiation](../../../../../differentiation.md) gives the operator identity

$$
u_t-6uu_x+u_{xxx}
=(\partial_x+2v)(v_t-6v^2v_x+v_{xxx}).
$$

For example $u_x=2vv_x+v_{xx}$ and $u_{xxx}=6v_xv_{xx}+2vv_{xxx}+v_{xxxx}$; inserting them makes the $v_xv_{xx}$ terms cancel and leaves the right side. Hence **$u$ solves $u_t-6uu_x+u_{xxx}=0$** whenever $v$ solves the [mKdV equation](../../../../../modified-korteweg-de-vries-equation.md). Both $v^2$ and $v_x$ have weight $-2\alpha$, so the corresponding [Korteweg-De Vries equation](../../../../../korteweg-de-vries-equation.md) symmetry is

$$
\boxed{(x,t,u)\mapsto(e^s x,e^{3s}t,e^{-2s}u),\qquad
x\partial_x+3t\partial_t-2u\partial_u.}
$$

## ↑ Ancestors (10)

1. [32E](../32e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
