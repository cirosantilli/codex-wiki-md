<h1 id="n/n1/solution">Solution</h1>

↑ **Parent:** [N1](../n1.md)

Condition on the state after $m$ steps and use the [Markov property](../../../../markov-property.md) and [time-homogeneous Markov property](../../../../time-homogeneous-markov-property.md):

$$
p_{ij}^{(m+n)}=\sum_{k\in S}\mathbb P(X_{m+n}=j\mid X_m=k,X_0=i)
\mathbb P(X_m=k\mid X_0=i)=\boxed{\sum_kp_{ik}^{(m)}p_{kj}^{(n)}}.
$$

This is the [Chapman-Kolmogorov equation](../../../../chapman-kolmogorov-equation.md), or $P^{m+n}=P^mP^n$. A [stationary distribution](../../../../stationary-distribution.md) is a [probability](../../../../probability.md) row vector with nonnegative entries summing to one and $\boxed{\pi P=\pi}$. Inductively $\pi P^n=\pi$, so a chain started with that distribution retains it at every time.

For the given [matrix](../../../../matrix.md), its first stationary equation is $\pi_1=\pi_1/2+(\pi_2+\pi_3)/3$. Normalization gives $\pi_1=2/5$. The third equation gives $\pi_3=2\pi_2/3+\pi_3/3$, hence $\pi_3=\pi_2$. Therefore

$$
\boxed{\pi=(2/5,3/10,3/10).}
$$

Direct multiplication verifies the second equation as well. The finite chain is irreducible, so this stationary [probability](../../../../probability.md) distribution is unique.

## ↑ Ancestors (12)

1. [N1](../n1.md)
2. [N](../../n.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
