<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Commutation of the two [local flows](../../../../../../local-flow.md) means $\phi_t\psi_s=\psi_s\phi_t$ for all sufficiently small independent parameters $s,t$, on their common local domains. Differentiate this identity in $s$ at zero. The [chain rule](../../../../../../chain-rule.md) gives

$$
d\phi_t|_p(Y_p)=Y_{\phi_t(p)}.
$$

In a [coordinate chart](../../../../../../manifold-chart.md), differentiating again in $t$ at zero gives $DX_pY_p=DY_pX_p$. But the [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md) has coordinate expression

$$
[X,Y]_p=DY_pX_p-DX_pY_p,
$$

so commuting [local flows](../../../../../../local-flow.md) imply $[X,Y]=0$.

For the converse, suppose the [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md) vanishes. Write $u(t)=\phi_t(p)$ in a [coordinate chart](../../../../../../manifold-chart.md), and put $J(t)=d\phi_t|_p$. Differentiating the [local flow](../../../../../../local-flow.md) equation with respect to the initial point gives the variational [ordinary differential equation](../../../../../../ordinary-differential-equation.md)

$$
\dot J(t)=DX_{u(t)}J(t),\qquad J(0)=I.
$$

Consequently $W(t)=Y_{u(t)}-J(t)Y_p$ satisfies

$$
\dot W(t)=DY_{u(t)}X_{u(t)}-DX_{u(t)}J(t)Y_p
=DX_{u(t)}W(t),\qquad W(0)=0,
$$

where the zero [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md) was used in the second equality. Uniqueness for this linear [ordinary differential equation](../../../../../../ordinary-differential-equation.md) gives $W=0$. This is a local argument and can be continued through successive [coordinate charts](../../../../../../manifold-chart.md), proving $d\phi_t(Y)=Y\circ\phi_t$ wherever the [local flow](../../../../../../local-flow.md) is defined.

For fixed $t$, the curve $s\mapsto\phi_t(\psi_s(p))$ therefore has derivative $Y$ at its current point and starts at $\phi_t(p)$. Uniqueness of the [integral curve of a vector field](../../../../../../integral-curve-of-a-vector-field.md) $Y$ identifies it with $s\mapsto\psi_s(\phi_t(p))$. Hence **$\boxed{\phi_t\psi_s=\psi_s\phi_t\ \Longleftrightarrow\ [X,Y]=0}$ locally**. No [complete vector field](../../../../../../complete-vector-field.md) hypothesis is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
