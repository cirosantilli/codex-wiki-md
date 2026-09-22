<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Within month two, each individual contributes only the time spent at risk between times one and two. There are $104-6-1=97$ complete one-month contributions. The six event contributions are $0.08,0.16,0.22,0.50,0.63,0.72$, and the censored contribution is $0.69$. Consequently

$$
T_2=97+(0.08+0.16+0.22+0.50+0.63+0.72)+0.69
=100\text{ person-months}.
$$

The month-specific [likelihood](../../../../../../likelihood-function.md) factor in a [piecewise-exponential survival model](../../../../../../piecewise-exponential-survival-model.md) is $\theta_2^6e^{-\theta_2T_2}$, giving

$$
\boxed{\widehat\theta_2=\frac6{100}=0.06\text{ per month}.}
$$

The eight individuals no longer at risk at time one contribute no month-two exposure. Using either all 112 individuals or all 104 as full-month observations would give the wrong denominator.

## ↑ Ancestors (11)

1. [B](../b.md)
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
