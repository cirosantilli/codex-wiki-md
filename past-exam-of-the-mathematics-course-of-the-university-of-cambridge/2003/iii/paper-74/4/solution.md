<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use [mass conservation](../../../../../mass-conservation.md) and conservative [momentum conservation](../../../../../momentum-conservation.md), with [viscous stress](../../../../../viscous-stress-tensor.md) $\sigma_{ij}$ defined so that its divergence is the viscous force:

$$
\rho_t+\partial_i(\rho u_i)=0,\qquad
(\rho u_i)_t+\partial_j(\rho u_i u_j)=-\partial_i p+\partial_j\sigma_{ij}.
$$

Differentiate the first equation in time and eliminate the momentum time derivative using the second. This gives

$$
\rho_{tt}=\partial_i\partial_j(\rho u_i u_j)+\nabla^2p-\partial_i\partial_j\sigma_{ij}.
$$

Set $\rho'=\rho-\rho_0$ and $p'=p-p_0$, where the reference values and $c_0$ are constant. Subtract $c_0^2\nabla^2\rho'$ to obtain the exact [Lighthill acoustic analogy](../../../../../lighthill-acoustic-analogy.md)

$$
\boxed{(\partial_t^2-c_0^2\nabla^2)\rho'=\partial_i\partial_jT_{ij},\qquad
T_{ij}=\rho u_i u_j+(p'-c_0^2\rho')\delta_{ij}-\sigma_{ij}}.
$$

The [Lighthill stress tensor](../../../../../lighthill-stress-tensor.md) includes nonlinear momentum transport, departure from the reference linear pressure-density relation, and [viscous stress](../../../../../viscous-stress-tensor.md). For an inviscid fluid the last term is absent. The derivation is an exact rearrangement of the conservation equations; treating the tensor as a known localized source is a subsequent approximation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
