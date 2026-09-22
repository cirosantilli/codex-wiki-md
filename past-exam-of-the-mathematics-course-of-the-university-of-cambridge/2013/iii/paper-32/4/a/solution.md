<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume [independent censoring](../../../../../../independent-censoring.md): the censoring mechanism contributes no factor involving the lifetime rate $\theta$. The exponential density and [survival function](../../../../../../survival-function.md) are $f_\theta(x)=\theta e^{-\theta x}$ and $S_\theta(x)=e^{-\theta x}$. An observed event contributes the density; a [right-censored](../../../../../../right-censoring.md) lifetime contributes the [probability](../../../../../../probability.md) of surviving its censoring time. Thus the [likelihood](../../../../../../likelihood-function.md) for $\theta$, up to censoring factors independent of it, is

$$
L(\theta)=\prod_{i=1}^n f_\theta(x_i)^{v_i}S_\theta(x_i)^{1-v_i}
=\theta^D e^{-\theta T},\qquad
D=\sum_i v_i,\quad T=\sum_i x_i.
$$

For $D>0$ and $T>0$, $\ell'(\theta)=D/\theta-T$ vanishes at $D/T$, and $\ell''(\theta)=-D/\theta^2<0$ proves the maximum:

$$
\boxed{\widehat\theta=\frac{\text{number of observed events}}{\text{total observed person-time}}
=\frac{\sum_i v_i}{\sum_i x_i}.}
$$

Censored individuals add follow-up time to the denominator but no event to the numerator. If $D=0$ and $T>0$, the [likelihood](../../../../../../likelihood-function.md) decreases for $\theta>0$ and has only a supremum as $\theta\downarrow0$; zero is an extended boundary estimate, not a positive-rate exponential [MLE](../../../../../../maximum-likelihood-estimator.md). The derivation is for independent individuals entering at time zero; delayed entry would require conditional survival contributions and exposure measured from entry.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
