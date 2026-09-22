<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a regular one-parameter [sampling distribution](../../../../../../sampling-distribution.md), the [Fisher information](../../../../../../fisher-information-matrix.md) and [Jeffreys prior](../../../../../../jeffreys-prior.md) are

$$
I(\theta)=\mathbb E_\theta\left[\left(\frac{\partial}{\partial\theta}\log p_Y(Y\mid\theta)\right)^2\right],
\qquad \boxed{\pi_J(\theta)\propto\sqrt{I(\theta)}}.
$$

Under the usual differentiation and integrability conditions, $I(\theta)=-\mathbb E_\theta[\partial_\theta^2\log p_Y(Y\mid\theta)]$. This [prior distribution](../../../../../../prior-probability.md) transforms as a density under smooth one-to-one reparameterizations, so the rule is coordinate invariant. Its integral need not be finite; [posterior propriety](../../../../../../posterior-propriety.md) must still be established if it is an [improper prior](../../../../../../improper-prior.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
