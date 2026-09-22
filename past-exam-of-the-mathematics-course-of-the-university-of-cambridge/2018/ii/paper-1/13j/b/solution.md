<h1 id="13j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
\Lambda(t)=\int_0^t\lambda(s)\,ds
$$

be the baseline [cumulative hazard](../../../../../../cumulative-hazard-function.md). Under the [proportional hazards model](../../../../../../proportional-hazards-model.md),

$$
h_i(t)=\lambda(t)e^{\beta^Tx_i},
\qquad
S_i(t)=\exp[-e^{\beta^Tx_i}\Lambda(t)].
$$

Thus

$$
f_i(Y_i)=h_i(Y_i)S_i(Y_i)
=\lambda(Y_i)e^{\beta^Tx_i}
\exp[-e^{\beta^Tx_i}\Lambda(Y_i)].
$$

Independence makes the log likelihood

$$
\boxed{\
\ell(\beta)=\sum_{i=1}^n
\left[
\log\lambda(Y_i)+\beta^Tx_i
-e^{\beta^Tx_i}\Lambda(Y_i)
\right]\
}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [13J](../../13j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
