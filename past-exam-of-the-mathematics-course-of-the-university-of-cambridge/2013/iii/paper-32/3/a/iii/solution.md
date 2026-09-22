<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Wald statistic](../../../../../../../wald-test.md) has law $Z_1=\widehat\delta_1\sqrt{I_1}\sim N(\delta\sqrt{I_1},1)$. Write $C=\{Z_1\geq f_1\}$ for continuation. By the normal cumulative distribution function,

$$
\Pr_\delta(C)=1-\Phi(f_1-\delta\sqrt{I_1})
=\Phi(\delta\sqrt{I_1}-f_1).
$$

The final [sample size](../../../../../../../sample-size.md) per arm is $N=n_1+n_2^*\mathbf1_C$, so

$$
\boxed{\mathbb E_\delta N
=n_1+n_2^*\Phi(\delta\sqrt{I_1}-f_1).}
$$

It lies between $n_1$ and $n_2=n_1+n_2^*$, increasing with the treatment effect: a more promising treatment is more likely to reach full enrollment. Total expected recruitment over both arms is twice this expression. Equality at the [futility boundary](../../../../../../../futility-boundary.md) has [probability](../../../../../../../probability.md) zero under the normal model.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 32](../../../../paper-32-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
