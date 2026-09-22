<h1 id="3h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [derivative](../../../../../../derivative.md) is $f'(x)=-4x^3e^{-x^4}$. Its absolute value is [continuous](../../../../../../continuous-function.md) and tends to zero as $x\to\pm\infty$, so it is bounded. More explicitly,

$$
\sup_{x\in\mathbb R}|f'(x)|=4\left(\frac34\right)^{3/4}e^{-3/4}=:M,
$$

obtained by differentiating $4t^3e^{-t^4}$ for $t\geq0$. The [mean value theorem](../../../../../../mean-value-theorem.md) gives $|f(x)-f(y)|\leq M|x-y|$ for every $x,y$. Thus $f$ is [Lipschitz continuous](../../../../../../lipschitz-continuity.md), and choosing $\delta=\varepsilon/M$ proves **$e^{-x^4}$ is uniformly continuous on $\mathbb R$**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3H](../../3h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
