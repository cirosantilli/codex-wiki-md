<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a period-$n$ orbit of $g(x)=\mu-x^2$ that avoids zero, the [chain rule](../../../../../../chain-rule.md) gives its [multiplier of a periodic orbit of an iteration](../../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) as

$$
(g^n)'(\hat x)=\prod_{k=1}^n g'(x_k)=(-2)^n\prod_{k=1}^n x_k.
$$

The sign of $g'$ is positive on the negative half-axis and negative on the positive half-axis, exactly as the parabola sketch shows. Consequently

$$
\boxed{\operatorname{sgn}((g^n)'(\hat x))=(-1)^n\prod_{k=1}^n\operatorname{sgn}(x_k).}
$$

This product is independent of the chosen starting point because changing $\hat x$ only cyclically reorders the factors. If the orbit contains zero, the derivative product is zero and its orientation is undefined. One must then use the actual zero [periodic-orbit multiplier](../../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md), rather than infer a positive or negative orientation from the special assignment $\operatorname{sgn}(0)=1$. The nonzero-[periodic-orbit multiplier](../../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) cases needed in part (d) avoid this exception automatically.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
