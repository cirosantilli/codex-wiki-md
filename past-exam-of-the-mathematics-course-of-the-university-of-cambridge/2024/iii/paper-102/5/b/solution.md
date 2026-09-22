<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a dominant integral weight $\lambda$, the [Weyl character formula](../../../../../../weyl-character-formula.md) is

$$
\operatorname{ch}V(\lambda)=
\frac{\sum_{w\in W}(-1)^{\ell(w)}e^{w(\lambda+\rho)}}
{\sum_{w\in W}(-1)^{\ell(w)}e^{w\rho}},
$$

where $W$ is the [Weyl group](../../../../../../weyl-group.md), $\ell$ is [Coxeter length](../../../../../../coxeter-length.md), and $\rho$ is the [half-sum of positive roots](../../../../../../half-sum-of-positive-roots.md). The [Weyl denominator formula](../../../../../../weyl-denominator-formula.md) is

$$
\sum_{w\in W}(-1)^{\ell(w)}e^{w\rho}
=e^\rho\prod_{\alpha\in\Phi^+}(1-e^{-\alpha}).
$$

Set $\lambda=k\rho$. Apply the denominator identity after replacing every formal exponential $e^\mu$ by $e^{(k+1)\mu}$:

$$
\sum_w(-1)^{\ell(w)}e^{w((k+1)\rho)}
=e^{(k+1)\rho}
\prod_{\alpha\in\Phi^+}(1-e^{-(k+1)\alpha}).
$$

Dividing this by the ordinary denominator gives

$$
\begin{aligned}
\operatorname{ch}V(k\rho)
&=e^{k\rho}\prod_{\alpha\in\Phi^+}
\frac{1-e^{-(k+1)\alpha}}{1-e^{-\alpha}}\\
&=\boxed{e^{k\rho}\prod_{\alpha\in\Phi^+}
(1+e^{-\alpha}+\cdots+e^{-k\alpha})}.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
