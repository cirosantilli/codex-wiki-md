<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Compare future premium differences, since the current premium is already fixed. From the highest discount, making no claim keeps all future premiums at $c(1-\beta)$. One submitted claim raises next year's premium to $c(1-\alpha)$; if there are no further events, the year after returns to $c(1-\beta)$. The extra premium is therefore $c(\beta-\alpha)$. Claiming saves payment of the loss itself, so the first claim is advantageous precisely when $L_1>c(\beta-\alpha)$. For the unit-rate [exponential distribution](../../../../../../exponential-distribution.md) loss,

$$
\boxed{\mathbb P(\text{claim for }L_1)=e^{-c(\beta-\alpha)}.}
$$

Now condition on the first claim already having been submitted. If the second loss is not claimed, next year's discount is $\alpha$ and the following year's is $\beta$. Claiming the second loss instead makes these two discounts $0$ and $\alpha$, after which both paths are back at $\beta$. Thus the additional premium caused by this second claim is

$$
c\alpha+c(\beta-\alpha)=c\beta.
$$

This is the [incremental second-claim threshold at the highest discount level](../../../../../../incremental-second-claim-threshold-at-the-highest-discount-level.md): compare the second decision to the already-chosen one-claim path, not to a no-claim path. The second claim is advantageous exactly when $L_2>c\beta$. The losses are independent, so conditioning on the first claim does not change the [exponential distribution](../../../../../../exponential-distribution.md) of $L_2$. Hence

$$
\boxed{\mathbb P(\text{claim for }L_2\mid\text{claimed for }L_1)=e^{-c\beta}.}
$$

Equality at a threshold has probability zero. The infinitely many premiums common to both paths cancel; all nonzero differences occur in the next two years, so no divergent sum is used. These thresholds use the undiscounted comparison in the question, with no interest rate or deductible introduced.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
