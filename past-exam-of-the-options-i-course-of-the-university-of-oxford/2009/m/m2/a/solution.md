<h1 id="m/m2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $n=0$, the conditional transition probabilities are $\delta_{ij}$, the entries of $P^0=I$; for $n=1$ the assertion is the definition of $P$. For the induction step, condition on the state at time $n$ and use the [Markov property](../../../../../markov-property.md) and [time-homogeneity](../../../../../time-homogeneous-markov-property.md):

$$
\mathbb P(X_{n+1}=j\mid X_0=i)
=\sum_k\mathbb P(X_n=k\mid X_0=i)p_{kj}
=\sum_k(P^n)_{ik}p_{kj}=(P^{n+1})_{ij}.
$$

The countable sum is justified by the [law of total probability](../../../../../law-of-total-probability.md); all terms are nonnegative. Thus the formula follows for every $n$ by induction. It is the [Chapman-Kolmogorov equation](../../../../../chapman-kolmogorov-equation.md) for repeated one-step transitions.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [M2](../../m2.md)
3. [M](../../../m.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
