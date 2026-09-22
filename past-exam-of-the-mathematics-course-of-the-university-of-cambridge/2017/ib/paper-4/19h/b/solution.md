<h1 id="19h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under the [null hypothesis](../../../../../../null-hypothesis.md) $\theta=0$, $X$ has the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $[0,1]$. Against $\theta=1$, the [likelihood ratio](../../../../../../likelihood-ratio.md) is $2x$, increasing on that interval. The [Neyman-Pearson lemma](../../../../../../neyman-pearson-lemma.md) therefore gives

$$
\boxed{\text{Reject }H_0\text{ when }X>1-\alpha\quad(0\leq\alpha\leq1)}.
$$

The [size of a statistical test](../../../../../../size-of-a-statistical-test.md) is $\mathbb P_0(X>1-\alpha)=\alpha$, and there is no boundary randomisation issue for this [continuous probability distribution](../../../../../../continuous-probability-distribution-split.md). Its [statistical power](../../../../../../statistical-power.md) against $\theta=1$ is $\int_{1-\alpha}^1 2x\,dx=2\alpha-\alpha^2$.

For every admissible alternative $0<\theta\leq1$, the [likelihood ratio](../../../../../../likelihood-ratio.md) $1-\theta+2\theta x$ is strictly increasing. The same upper-tail rejection set has size $\alpha$ and is a [most powerful test](../../../../../../most-powerful-test.md) against each fixed such alternative, again by the [Neyman-Pearson lemma](../../../../../../neyman-pearson-lemma.md). Hence **the same test is a [uniformly most powerful test](../../../../../../uniformly-most-powerful-test.md) against $\theta>0$**, where the alternative is understood within the specified parameter range. Its full [power function](../../../../../../power-function-of-a-statistical-test.md) is

$$
\boxed{\beta(\theta)=\int_{1-\alpha}^1(1-\theta+2\theta x)\,dx
=\alpha+\theta\alpha(1-\alpha)}.
$$

For $\alpha=0$ or $1$, the never-reject or always-reject test supplies the respective endpoint case.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19H](../../19h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
