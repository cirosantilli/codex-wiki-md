<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Insert $f_i=h_iF_i$ and $F_i=e^{-H_i}$ into the [survival likelihood](../../../../../../../survival-likelihood.md). Each individual's log contribution simplifies to

$$
v_i\log h_i(x_i;\theta)+\log F_i(x_i;\theta).
$$

Therefore

$$
\boxed{\ell(\theta)=\sum_{i=1}^n\{v_i\log h_i(x_i;\theta)-H_i(x_i;\theta)\}+\text{constant}.}
$$

Failures contribute a log [hazard function](../../../../../../../hazard-function.md) term as well as exposure, whereas both failures and censored subjects contribute the negative [cumulative hazard function](../../../../../../../cumulative-hazard-function.md) over their observed follow-up.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 29](../../../../paper-29-split.md)
5. [Iii](../../../../split.md)
6. [2001](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
