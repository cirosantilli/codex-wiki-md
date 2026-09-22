<h1 id="m/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Condition on the intermediate state at time $m$. The [Markov property](../../../../../markov-property.md) and time homogeneity give

$$
p_{ij}(m+n)=\sum_k\Pr(X_m=k\mid X_0=i)\Pr(X_{m+n}=j\mid X_m=k)=\sum_kp_{ik}(m)p_{kj}(n).
$$

These nonnegative sums are valid on a countable state space. Starting from $P(0)=I$, $P(1)=P$, [induction](../../../../../mathematical-induction.md) gives $\boxed{P(n)=P^n}$. Conditioning on the initial state now yields $\boxed{\Pr(X_n=i)=(\mu P^n)_i}$. If $\mu P=\mu$, [induction](../../../../../mathematical-induction.md) gives $\mu P^n=\mu$ for every $n$, so all one-time distributions equal the stationary initial distribution.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [M](../../../m.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
