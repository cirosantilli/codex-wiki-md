<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Under the specified evolution rule, conditional on the entire history, the next event's [probability distribution](../../../../../probability-distribution-split.md) depends only on the current population size. This is the [time-homogeneous Markov property](../../../../../time-homogeneous-markov-property.md). Birth and immigration both increase the size by one, while death decreases it by one. Writing $q=1-p$, the [transition probabilities](../../../../../transition-probability.md) on $\mathbb Z_{\geq0}$ are

$$
\boxed{P(k,k+1)=u_k=\frac{kp+\theta}{k+\theta}\quad(k\geq0),\qquad P(k,k-1)=d_k=\frac{kq}{k+\theta}\quad(k\geq1),}
$$

and all other entries are zero. In particular $P(0,1)=1$ and $d_0=0$. The row sum is $[kp+\theta+kq]/(k+\theta)=1$. Every neighboring pair communicates, so this is an [irreducible Markov chain](../../../../../irreducible-markov-chain.md), specifically a [birth-death-immigration jump chain](../../../../../birth-death-immigration-jump-chain.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
