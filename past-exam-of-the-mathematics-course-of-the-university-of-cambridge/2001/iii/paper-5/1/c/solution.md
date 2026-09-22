<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the [Weyl character formula](../../../../../../weyl-character-formula.md) with $\lambda=\rho$. In the [Weyl denominator formula](../../../../../../weyl-denominator-formula.md), replace every formal exponential $e^\mu$ by $e^{2\mu}$. This gives

$$
A_{2\rho}=e^{2\rho}\prod_{\alpha>0}(1-e^{-2\alpha}).
$$

Dividing by $A_\rho=e^\rho\prod_{\alpha>0}(1-e^{-\alpha})$ and cancelling each factor yields

$$
\boxed{\operatorname{ch}L(\rho)=e^\rho\prod_{\alpha>0}(1+e^{-\alpha})
=\prod_{\alpha>0}(e^{\alpha/2}+e^{-\alpha/2}).}
$$

The last expression is a compact way of writing the same character; individual half-root exponentials may need a larger formal lattice, but their full product lies in the group ring of the [weight lattice](../../../../../../weight-lattice.md). Expanding the first expression, a subset $S\subseteq R^+$ contributes the [weight](../../../../../../weight-representation-theory.md) $\rho-\sum_{\alpha\in S}\alpha$. Different subsets with the same sum give that weight's multiplicity. In particular $\dim L(\rho)=2^{|R^+|}$, consistent with the [Weyl dimension formula](../../../../../../weyl-dimension-formula.md). This is the case $k=1$ of the [character of a Weyl-vector multiple](../../../../../../character-of-a-weyl-vector-multiple.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
