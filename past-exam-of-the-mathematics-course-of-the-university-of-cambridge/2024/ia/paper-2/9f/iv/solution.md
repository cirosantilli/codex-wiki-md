<h1 id="9f/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Conditioning on $N$ and using the [moment-generating function](../../../../../../moment-generating-function.md) of a unit exponential variable,

$$
\begin{aligned}
\mathbb E(e^{\theta Y})
&=\sum_{n=1}^\infty p(1-p)^{n-1}
  \left(\frac1{1-\theta}\right)^n\\
&=\frac{p}{1-\theta}
  \sum_{m=0}^\infty
  \left(\frac{1-p}{1-\theta}\right)^m
=\boxed{\frac{p}{p-\theta}},
\end{aligned}
$$

where the geometric [series](../../../../../../series-mathematics.md) converges precisely when $\theta<p$. This is the moment-generating [function](../../../../../../function-split.md) of an exponential variable of rate $p$, so the [geometric sum of exponential variables](../../../../../../geometric-sum-of-exponential-variables.md) satisfies

$$
\boxed{Y\sim\operatorname{Exp}(p)}.
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
