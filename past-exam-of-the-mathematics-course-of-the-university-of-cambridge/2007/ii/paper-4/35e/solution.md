<h1 id="35e/solution">Solution</h1>

↑ **Parent:** [35E](../35e.md)

Replace $\varphi$ by $\varphi+\epsilon\eta$, with $\eta$ vanishing on the boundary, and differentiate the action at zero. Integrate the derivative of $\eta$ by parts:

$$
\delta S=\int\left[\frac{\partial\mathcal L}{\partial\varphi}\eta+
\frac{\partial\mathcal L}{\partial\varphi_{,a}}\partial_a\eta\right]d^4x
=\int\left[\frac{\partial\mathcal L}{\partial\varphi}
-\partial_a\frac{\partial\mathcal L}{\partial\varphi_{,a}}\right]\eta\,d^4x.
$$

The coefficient of $\eta$ is the [functional derivative](../../../../../functional-derivative.md) $\delta S/\delta\varphi$.

For the electromagnetic action, $\delta F_{ab}=\partial_a\delta A_b-\partial_b\delta A_a$. Antisymmetry combines these terms and integration by parts gives

$$
\delta S=\int\left[\mu_0^{-1}\partial_aF^{ab}-J^b\right]\delta A_b\,d^4x.
$$

Thus the inhomogeneous [Maxwell equations](../../../../../maxwell-equations.md) are $\partial_aF^{ab}=\mu_0J^b$. The definition of $F$ also gives the homogeneous equations $\partial_{[a}F_{bc]}=0$, equivalently $\partial_a\widetilde F^{ab}=0$. These are the two four-vector Maxwell systems.

Unrestricted variation of the alternative component-gradient action instead gives $\Box A^b=\mu_0J^b$. This is equivalent to the first Maxwell system only when supplemented by the [Lorenz gauge](../../../../../lorenz-gauge-condition.md) $\partial_aA^a=0$, because

$$
\partial_aF^{ab}=\Box A^b-\partial^b(\partial_aA^a).
$$

The alternative action is not by itself gauge-invariant; the additional condition must be supplied consistently, not silently omitted.

Expand the tensor square: $F^{ab}F_{ab}=2[\partial^bA^a\partial_bA_a-\partial^bA^a\partial_aA_b]$. Hence

$$
S-\widehat S=\frac1{2\mu_0}\int\partial^bA^a\partial_aA_b\,d^4x.
$$

Integrating this cross term by parts twice expresses its integral as a boundary term plus $\int(\partial_aA^a)^2\,d^4x$. Under Lorenz gauge it is therefore purely a boundary term. With fixed or vanishing boundary contributions, **the two actions have the same variational equations once the additional gauge condition is included**. This is the [Lorenz-gauge reduction of the electromagnetic action](../../../../../lorenz-gauge-reduction-of-the-electromagnetic-action.md).

## ↑ Ancestors (10)

1. [35E](../35e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
