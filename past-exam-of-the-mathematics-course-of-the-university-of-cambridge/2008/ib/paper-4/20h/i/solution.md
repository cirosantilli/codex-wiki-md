<h1 id="20h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For fixed $b$, put $\mathcal L_b(x)=f(x)+\lambda(b)^T(b-g(x))$. Feasibility gives $\mathcal L_b(\bar x(b))=f(\bar x(b))=\phi(b)$. The assumed [Lagrangian duality](../../../../../../lagrangian-duality.md) representation says this value is the unrestricted supremum of $\mathcal L_b$, so $\bar x(b)$ is also an unconstrained global maximizer of this continuously differentiable function. Its first derivative vanishes:

$$
\nabla f(\bar x)=Dg(\bar x)^T\lambda(b).
$$

Differentiate the identity $g(\bar x(b))=b$ using the assumed smooth dependence of the optimizer:

$$
Dg(\bar x)D_b\bar x=I_m.
$$

The [chain rule](../../../../../../chain-rule.md) now gives the [envelope theorem](../../../../../../envelope-theorem.md)

$$
D_b\phi=\nabla f(\bar x)^TD_b\bar x=\lambda(b)^TDg(\bar x)D_b\bar x=\lambda(b)^T.
$$

Thus

$$
\boxed{\frac{\partial\phi}{\partial b_i}(b)=\lambda_i(b),\qquad i=1,\ldots,m.}
$$

Each [Lagrange multiplier](../../../../../../lagrange-multiplier.md) is the marginal change in optimal value per unit relaxation of its constraint. The proof only uses the resulting stationarity and smooth feasibility identities; it does not require differentiating the maximizer explicitly or differentiating the multiplier.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [20H](../../20h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
