<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A smooth [vector field](../../../../../vector-field.md) is a smooth [section of a vector bundle](../../../../../section-of-a-vector-bundle.md) $X:M\to TM$ of the [tangent bundle](../../../../../tangent-bundle.md), so $X_p\in T_pM$. In a [manifold chart](../../../../../manifold-chart.md), $X=X^i\partial_i$ with smooth coefficients. It acts on a [smooth function](../../../../../smooth-function.md) by $Xf=X^i\partial_i f$. For a [diffeomorphism](../../../../../diffeomorphism.md) $\alpha:M\to N$, the [pushforward of a vector field](../../../../../pushforward-of-a-vector-field.md) is

$$
(\alpha_*X)_q=d\alpha_{\alpha^{-1}(q)}X_{\alpha^{-1}(q)}.
$$

The [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md) is the commutator of their actions on [smooth functions](../../../../../smooth-function.md):

$$
[X,Y]f=X(Yf)-Y(Xf),\qquad [X,Y]^j=X^i\partial_iY^j-Y^i\partial_iX^j.
$$

The second derivatives of $f$ cancel, so this is again a [vector field](../../../../../vector-field.md). The corresponding [Jacobi identity](../../../../../jacobi-identity.md) is $[X,[Y,Z]]+[Y,[Z,X]]+[Z,[X,Y]]=0$.

A [local flow](../../../../../local-flow.md) of $X$ is a smooth map $(t,p)\mapsto\phi_t(p)$ on an open neighbourhood of $\{0\}\times M$ satisfying $\phi_0(p)=p$ and $\partial_t\phi_t(p)=X_{\phi_t(p)}$. On a sufficiently small neighbourhood and time interval, each $\phi_t$ is a [diffeomorphism](../../../../../diffeomorphism.md) onto its image, with inverse $\phi_{-t}$. Uniqueness of [integral curves of a vector field](../../../../../integral-curve-of-a-vector-field.md) gives $\phi_{s+t}=\phi_s\circ\phi_t$ wherever both sides are defined. These are local statements; no assumption of a [complete vector field](../../../../../complete-vector-field.md) is required.

A smooth [tensor field](../../../../../tensor-field.md) of type $(r,s)$ is a smooth section of $(TM)^{\otimes r}\otimes(T^*M)^{\otimes s}$, where the factors are the [tangent bundle](../../../../../tangent-bundle.md) and [cotangent bundle](../../../../../cotangent-bundle.md). The [flow definition of the Lie derivative of a tensor field](../../../../../flow-definition-of-the-lie-derivative-of-a-tensor-field.md) is

$$
\mathcal L_XT=\left.\frac d{dt}\right|_{t=0}\phi_t^*T.
$$

Here pullback applies $d\phi_t^{-1}$ to each vector factor and the dual of $d\phi_t$ to each covector factor, evaluating $T$ at $\phi_t(p)$. Thus all tensors being differentiated lie in the same fibre over $p$.

For a [smooth function](../../../../../smooth-function.md), $\phi_t^*f=f\circ\phi_t$, and the [chain rule](../../../../../chain-rule.md) gives

$$
\boxed{\mathcal L_Xf=df(X)=Xf}.
$$

For a [vector field](../../../../../vector-field.md) $Y$, in local coordinates the expansions $\phi_t(x)=x+tX(x)+O(t^2)$ and $d\phi_t(x)=I+t\,dX_x+O(t^2)$ give

$$
\phi_t^*Y(x)=d\phi_t(x)^{-1}Y(\phi_t(x))
=Y(x)+t\bigl(dY_xX(x)-dX_xY(x)\bigr)+O(t^2).
$$

Consequently

$$
\boxed{\mathcal L_XY=[X,Y]}.
$$

Pullback preserves [tensor products](../../../../../tensor-product.md) and [tensor contractions](../../../../../tensor-contraction.md), so differentiation makes this definition a [tensor derivation](../../../../../tensor-derivation.md). It therefore agrees on every [tensor field](../../../../../tensor-field.md) with the [Lie derivative of a tensor field](../../../../../lie-derivative-of-a-tensor-field.md) determined by these two formulas.

Now put $\psi_t=\alpha\circ\phi_t\circ\alpha^{-1}$. The [chain rule](../../../../../chain-rule.md) gives

$$
\partial_t\psi_t(q)=d\alpha_{\phi_t(\alpha^{-1}q)}X_{\phi_t(\alpha^{-1}q)}
=(\alpha_*X)_{\psi_t(q)},\qquad \psi_0(q)=q.
$$

Thus $\psi_t$ is the [local flow](../../../../../local-flow.md) of $\alpha_*X$. In the case $M=N$, if $\alpha_*X=X$, uniqueness of [integral curves of a vector field](../../../../../integral-curve-of-a-vector-field.md) makes $\psi_t=\phi_t$ on their common domains, or $\alpha\circ\phi_t=\phi_t\circ\alpha$. Conversely, differentiating this commuting identity at zero gives $d\alpha_pX_p=X_{\alpha(p)}$, hence $\alpha_*X=X$. This proves that [diffeomorphism invariance of a vector field is equivalent to commuting with its local flow](../../../../../diffeomorphism-invariance-of-a-vector-field-is-equivalent-to-commuting-with-its-local-flow.md), with every identity understood on the domain where its compositions exist.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 115](../../paper-115-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
