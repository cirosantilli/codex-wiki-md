<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $N=|R^+|$ and identify the real weight and Cartan spaces using a [Weyl group](../../../../../../weyl-group.md)-invariant positive [inner product](../../../../../../inner-product.md). For a regular $H$, meaning $(\alpha,H)\ne0$ for every root, specialize $e^\mu$ to $e^{t(\mu,H)}$. Then the value of the [formal character](../../../../../../formal-character-of-a-weight-module.md) at $t=0$ is $\dim L(\lambda)$, but both [Weyl alternants](../../../../../../weyl-alternant.md) in the [Weyl character formula](../../../../../../weyl-character-formula.md) vanish there. We compute their leading terms instead of substituting into that zero-over-zero expression.

Expand

$$
A_\nu(tH)=\sum_{m\ge0}t^m P_m(\nu,H),\qquad
P_m(\nu,H)=\frac1{m!}\sum_{w\in W}\det(w)(w\nu,H)^m.
$$

For every root reflection $s$, replacing $\nu$ by $s\nu$ changes the sign of $P_m$, by replacing $w$ with $ws$ in the sum. Replacing $H$ by $sH$ also changes its sign, by replacing $w$ with $sw$. Thus the polynomial vanishes whenever $\nu$ or $H$ lies on any reflecting hyperplane. It is divisible by $\prod_{\alpha>0}(\nu,\alpha)$ in its first variables and by $\prod_{\alpha>0}(H,\alpha)$ in its second variables. Distinct positive roots give distinct linear factors; each product has degree $N$.

The polynomial $P_m$ has degree $m$ in each group of variables. Therefore $P_m=0$ for $m<N$, and for $m=N$ it has the form

$$
P_N(\nu,H)=C\prod_{\alpha>0}(\nu,\alpha)\prod_{\alpha>0}(H,\alpha)
$$

with a constant $C$ independent of both variables. At $\nu=\rho$, the [Weyl denominator formula](../../../../../../weyl-denominator-formula.md) gives

$$
A_\rho(tH)=e^{t(\rho,H)}\prod_{\alpha>0}(1-e^{-t(\alpha,H)})
=t^N\prod_{\alpha>0}(\alpha,H)+O(t^{N+1}).
$$

Consequently $C\prod_{\alpha>0}(\rho,\alpha)=1$. For strictly dominant $\nu=\lambda+\rho$, its leading coefficient is nonzero, and the ratio of the two [Weyl alternants](../../../../../../weyl-alternant.md) tends to

$$
\boxed{\dim L(\lambda)=\prod_{\alpha>0}\frac{(\lambda+\rho,\alpha)}{(\rho,\alpha)}
=\prod_{\alpha>0}\frac{\langle\lambda+\rho,\alpha^\vee\rangle}{\langle\rho,\alpha^\vee\rangle}.}
$$

The [coroot](../../../../../../coroot.md) is $\alpha^\vee=2\alpha/(\alpha,\alpha)$, so the root-length factors cancel in each ratio. This proves the [Weyl dimension formula](../../../../../../weyl-dimension-formula.md) by the [lowest-degree alternant proof of the Weyl dimension formula](../../../../../../lowest-degree-alternant-proof-of-the-weyl-dimension-formula.md), including the limiting step.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
