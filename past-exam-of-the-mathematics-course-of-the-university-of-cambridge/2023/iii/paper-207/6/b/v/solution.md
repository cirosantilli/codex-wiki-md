<h1 id="6/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Ignoring factors that do not depend on $\theta$, each observed side-effect contributes $\theta e^{-\theta x_i}$ and each censored observation contributes $e^{-\theta x_i}$. Thus

$$
L(\theta)\propto\theta^{v_+}e^{-\theta x_+},
\qquad
\ell(\theta)=v_+\log\theta-\theta x_++\text{constant}.
$$

The [score equation](../../../../../../../score-equation.md) $v_+/\theta-x_+=0$ gives

$$
\widehat\theta=\frac{v_+}{x_+}.
$$

This event-count divided by person-time estimator is the sample analogue of the expectation ratio in part iv.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
