<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [sl2 Lie algebra](../../../../../sl2-lie-algebra.md) relations $[H,X]=2X$, $[H,Y]=-2Y$ and $[X,Y]=H$. A [highest-weight vector](../../../../../highest-weight-vector.md) satisfies $Xv=0$ and $Hv=mv$, and $HY^jv=(m-2j)Y^jv$. For $k=0$, $XYv=YXv+Hv=mv$. Assuming the formula at $k-1$, one gets

$$
XY^{k+1}v=(YX+H)Y^kv=\bigl[k(m-k+1)+m-2k\bigr]Y^kv=(k+1)(m-k)Y^kv.
$$

Thus the [sl2 highest-weight lowering formula](../../../../../sl2-highest-weight-lowering-formula.md) is

$$
\boxed{XY^{k+1}v=(k+1)(m-k)Y^kv\qquad(k\geq0).}
$$

In particular a finite-dimensional [Irreducible Lie algebra representation](../../../../../irreducible-lie-algebra-representation.md) has highest weight $m\in\mathbb Z_{\geq0}$ and [weight vectors](../../../../../weight-vector.md) $v,Yv,\ldots,Y^mv$, as in the [classification of finite-dimensional sl2 representations](../../../../../classification-of-finite-dimensional-sl2-representations.md).

Let $V_\lambda$ be a finite-dimensional [Irreducible Lie algebra representation](../../../../../irreducible-lie-algebra-representation.md) of a complex [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md), with [highest weight](../../../../../highest-weight-of-a-representation.md) $\lambda$. Write $m_\lambda(\mu)=\dim(V_\lambda)_\mu$, taking it to be zero when $\mu$ is not a weight, and let $\rho$ be the [half-sum of positive roots](../../../../../half-sum-of-positive-roots.md). The [Killing form](../../../../../killing-form.md) induces an [inner product](../../../../../inner-product.md) on the real span of weights. [Freudenthal multiplicity formula](../../../../../freudenthal-multiplicity-formula.md) states

$$
\boxed{\bigl((\lambda+\rho,\lambda+\rho)-(\mu+\rho,\mu+\rho)\bigr)m_\lambda(\mu)=2\sum_{\alpha>0}\sum_{j\geq1}(\mu+j\alpha,\alpha)m_\lambda(\mu+j\alpha).}
$$

The sums are finite. For a weight $\mu\ne\lambda$, the coefficient on the left is positive: move $\mu$ into the dominant [Weyl chamber](../../../../../fundamental-chamber-of-a-root-system.md), use that a [weight](../../../../../weight-representation-theory.md) is below $\lambda$ in [dominance order](../../../../../dominance-order.md), and note that $(\mu,\rho)$ does not increase on moving back out of that chamber. The resulting recursion starts from $m_\lambda(\lambda)=1$.

Here is a proof using the allowed [Casimir operator](../../../../../casimir-element.md). Choose [root vectors](../../../../../root-vector.md) $E_\alpha,F_\alpha$ for positive and negative roots, normalized by $B(E_\alpha,F_\alpha)=1$, and let $t_\alpha\in\mathfrak h$ satisfy $B(t_\alpha,h)=\alpha(h)$. [Invariance of a bilinear form on a Lie algebra](../../../../../invariance-of-a-bilinear-form-on-a-lie-algebra.md) gives $[E_\alpha,F_\alpha]=t_\alpha$. If $h_i,h^i$ are [dual bases](../../../../../dual-basis.md) of the [Cartan subalgebra](../../../../../cartan-subalgebra.md) under $B$, the [Casimir operator](../../../../../casimir-element.md) is

$$
C=\sum_i h_ih^i+\sum_{\alpha>0}(E_\alpha F_\alpha+F_\alpha E_\alpha).
$$

On the [weight space](../../../../../weight-space.md) of $\mu$, the first sum acts by $(\mu,\mu)$. Replacing $E_\alpha F_\alpha$ with $F_\alpha E_\alpha+t_\alpha$ gives

$$
C\big|_{(V_\lambda)_\mu}=(\mu,\mu+2\rho)I+2\sum_{\alpha>0}F_\alpha E_\alpha\big|_{(V_\lambda)_\mu}.
$$

Define $T_\alpha(\mu)=\operatorname{tr}(F_\alpha E_\alpha\big|_{(V_\lambda)_\mu})$. The [cyclic trace identity between adjacent weight spaces](../../../../../cyclic-trace-identity-between-adjacent-weight-spaces.md) and the commutator relation yield

$$
T_\alpha(\mu)=\operatorname{tr}(E_\alpha F_\alpha\big|_{(V_\lambda)_{\mu+\alpha}})=T_\alpha(\mu+\alpha)+(\mu+\alpha,\alpha)m_\lambda(\mu+\alpha).
$$

Iterate upwards until the [weight spaces](../../../../../weight-space.md) vanish to obtain $T_\alpha(\mu)=\sum_{j\geq1}(\mu+j\alpha,\alpha)m_\lambda(\mu+j\alpha)$. Finally take the [trace](../../../../../matrix-trace.md) of the displayed restriction of $C$. Its [Casimir eigenvalue](../../../../../casimir-eigenvalue.md) is $(\lambda,\lambda+2\rho)$, so subtracting $(\mu,\mu+2\rho)m_\lambda(\mu)$ proves the formula. This trace argument handles [weight multiplicities](../../../../../weight-multiplicity.md) greater than one without choosing a separate [sl2 Lie algebra](../../../../../sl2-lie-algebra.md) string through each vector.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
