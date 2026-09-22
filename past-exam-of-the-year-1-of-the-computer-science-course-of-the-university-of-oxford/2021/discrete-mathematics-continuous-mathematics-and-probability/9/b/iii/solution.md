<h1 id="9/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $h_i=\mathbb E_i[J]=i/k$ and $v_i=\mathbb E_i[JX]$. Since $0\leq JX\leq X$, the latter [expected value](../../../../../../expected-value-split.md) is finite. Conditional on the first move to $i-1$ or $i+1$, total time is one plus the remaining time, while the terminal success [indicator random variable](../../../../../../indicator-random-variable.md) is unchanged. The [Markov property](../../../../../../markov-property.md) and [linearity of expectation](../../../../../../linearity-of-expectation.md) give

$$
v_i=\tfrac12(v_{i-1}+h_{i-1})+\tfrac12(v_{i+1}+h_{i+1})
=\tfrac12v_{i-1}+\tfrac12v_{i+1}+\frac ik.
$$

At either absorbing boundary the remaining time is zero, so $v_0=v_k=0$.

Let $w_i=i(k^2-i^2)/(3k)$. The linear term has zero second difference and $i^3$ has second difference $6i$. Consequently

$$
w_{i+1}-2w_i+w_{i-1}=-\frac{2i}{k},
$$

which is exactly the required recurrence, and $w_0=w_k=0$. Uniqueness follows as before: the difference of two solutions has zero second difference and zero endpoint values. Hence

$$
\boxed{\mathbb E_i[Y]=v_i=\frac{i(k^2-i^2)}{3k}.}
$$

This is the success-weighted duration underlying the [duration of gambler's ruin conditioned on a chosen boundary](../../../../../../duration-of-gambler-s-ruin-conditioned-on-a-chosen-boundary.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
