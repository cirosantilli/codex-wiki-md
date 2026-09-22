<h1 id="10c/solution">Solution</h1>

↑ **Parent:** [10C](../10c.md)

For a smooth map $\mathbf u$, the [Jacobian determinant](../../../../../jacobian-determinant.md) is the determinant of its [Jacobian matrix](../../../../../jacobian-matrix.md) $A_{ai}=\partial_i u_a$. In [Einstein summation convention](../../../../../einstein-notation.md),

$$
J[\mathbf u]=\det A=\frac16\epsilon_{ijk}\epsilon_{abc}(\partial_i u_a)(\partial_j u_b)(\partial_k u_c).
$$

Differentiate the supplied expression for $V_i$ by the [product rule](../../../../../product-rule.md). The term differentiating $\partial_j u_a$ vanishes because $\partial_i\partial_j u_a$ is symmetric in $i,j$, while $\epsilon_{ijk}$ is antisymmetric; the term differentiating $\partial_k u_b$ vanishes similarly. Only differentiation of $u_c$ remains:

$$
\partial_iV_i=\frac16\epsilon_{ijk}\epsilon_{abc}(\partial_j u_a)(\partial_k u_b)(\partial_i u_c)=J[\mathbf u].
$$

The last equality follows by the cyclic relabelling $(i,j,k)\mapsto(j,k,i)$, which has positive sign. This proves the [Jacobian determinant as a divergence](../../../../../jacobian-determinant-as-a-divergence.md) identity.

For a composition $\mathbf w=\mathbf u\circ\mathbf v$, the [chain rule](../../../../../chain-rule.md) gives

$$
\partial_iw_a(\mathbf x)=(\partial_bu_a)(\mathbf v(\mathbf x))\,\partial_iv_b(\mathbf x),\qquad D\mathbf w(\mathbf x)=D\mathbf u(\mathbf v(\mathbf x))D\mathbf v(\mathbf x).
$$

Taking [determinants](../../../../../determinant.md) yields

$$
\boxed{J[\mathbf w](\mathbf x)=J[\mathbf u](\mathbf v(\mathbf x))J[\mathbf v](\mathbf x).}
$$

For the first-order perturbation, use [spatial derivative control in perturbations of the identity map](../../../../../spatial-derivative-control-in-perturbations-of-the-identity-map.md): the usual smooth-family interpretation gives $D\mathbf u_t=I+tD\mathbf F+o(t)$ locally. Multilinearity of the [determinant](../../../../../determinant.md) shows that its linear term comes from choosing one column of $tD\mathbf F$ and all other columns from $I$. This gives the [trace](../../../../../matrix-trace.md):

$$
\boxed{J[\mathbf u_t]=1+t\operatorname{tr}(D\mathbf F)+o(t)=1+t\nabla\cdot\mathbf F+o(t),\qquad Q=\nabla\cdot\mathbf F.}
$$

The regularity qualification matters: a pointwise $o(t)$ remainder for maps does not by itself give an $o(t)$ remainder for spatial derivatives. For instance $(x+t^2\sin(x/t^2),y,z)$ has a uniform $o(t)$ displacement and $\mathbf F=0$, but its [Jacobian determinant](../../../../../jacobian-determinant.md) at $x=0$ is $2$ for $t\ne0$. Thus the first expansion needs the remainder in $C^1$ locally, or an equivalent smoothness assumption on the family.

Under the subsequent group law, $\mathbf u_0$ is the identity and $\mathbf u_{-t}$ is the inverse of $\mathbf u_t$. Write $j(t,\mathbf x)=J[\mathbf u_t](\mathbf x)$. Applying the composition formula to $\mathbf u_{t+h}=\mathbf u_h\circ\mathbf u_t$ and the short-time expansion gives the [Jacobian evolution of a smooth flow](../../../../../jacobian-evolution-of-a-smooth-flow.md):

$$
\partial_tj(t,\mathbf x)=(\nabla\cdot\mathbf F)(\mathbf u_t(\mathbf x))j(t,\mathbf x),\qquad j(0,\mathbf x)=1.
$$

Hence

$$
j(t,\mathbf x)=\exp\left(\int_0^t(\nabla\cdot\mathbf F)(\mathbf u_s(\mathbf x))\,ds\right).
$$

If only the pointwise generator expansion is assumed initially, the group law still gives $\partial_t\mathbf u_t(\mathbf x)=\mathbf F(\mathbf u_t(\mathbf x))$. Uniqueness and smooth dependence for this smooth [ordinary differential equation](../../../../../ordinary-differential-equation.md) make it a smooth [flow map](../../../../../flow-map.md), thereby justifying the differentiated expansion used above. Thus **a divergence-free generator has**

$$
\boxed{J[\mathbf u_t]=1\quad\text{for every }t.}
$$

By the [change of variables formula](../../../../../change-of-variables-formula.md), these maps preserve ordinary Euclidean volume and orientation. This is the Euclidean instance of a [volume-preserving vector field](../../../../../volume-preserving-vector-field.md).

## ↑ Ancestors (10)

1. [10C](../10c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
