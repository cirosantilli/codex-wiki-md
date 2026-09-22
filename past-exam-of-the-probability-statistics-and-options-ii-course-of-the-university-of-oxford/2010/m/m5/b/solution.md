<h1 id="m/m5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At $n=0$ the transition probability is $\delta_{ij}=(P^0)_{ij}$. If the assertion holds at $n$, condition on $X_n=k$ and use the [Markov property](../../../../../markov-property.md):

$$
P(X_{n+1}=j\mid X_0=i)=\sum_k P(X_n=k\mid X_0=i)p_{kj}=\sum_k(P^n)_{ik}p_{kj}=(P^{n+1})_{ij}.
$$

[Induction](../../../../../mathematical-induction.md) proves $\boxed{P(X_n=j\mid X_0=i)=(P^n)_{ij}}$. These countable sums contain nonnegative terms and are justified by total probability.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [M5](../../m5.md)
3. [M](../../../m.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
