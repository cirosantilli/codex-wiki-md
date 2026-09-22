<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

This is [König theorem for cardinal numbers](../../../../../konig-s-theorem-set-theory.md). Let $D=\bigsqcup_{\alpha<\beta}\kappa_\alpha$ and $P=\prod_{\alpha<\beta}\lambda_\alpha$. For any proposed map $g:D\to P$, consider the values of the $\alpha$th coordinates on the $\alpha$th summand:

$$
E_\alpha=\{g(\alpha,\xi)(\alpha):\xi<\kappa_\alpha\}.
$$

This set has [cardinality](../../../../../cardinality.md) at most $\kappa_\alpha<\lambda_\alpha$. Choose $y_\alpha\in\lambda_\alpha\setminus E_\alpha$, using the [axiom of choice](../../../../../axiom-of-choice.md), and assemble $y=(y_\alpha)\in P$. For any $(\alpha,\xi)\in D$, its image disagrees with $y$ at coordinate $\alpha$. Thus $y$ is outside the image of $g$, and no such $g$ is [surjective](../../../../../surjective-function.md).

Every $\lambda_\alpha$ is nonzero. The product is nonempty by choice; if $D$ is empty, strict inequality is immediate. Otherwise [cardinal comparability principle](../../../../../cardinal-comparability-principle.md) in ZFC says that $|P|\leq|D|$ would yield a [surjection](../../../../../surjective-function.md) from $D$ onto the nonempty $P$, which the [diagonal argument](../../../../../diagonal-argument.md) excludes. Therefore

$$
\boxed{\sum_{\alpha<\beta}\kappa_\alpha<\prod_{\alpha<\beta}\lambda_\alpha.}
$$

The diagonal coordinate is tied to the summand containing the argument; this is why a sum on the left pairs naturally with a product on the right.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
