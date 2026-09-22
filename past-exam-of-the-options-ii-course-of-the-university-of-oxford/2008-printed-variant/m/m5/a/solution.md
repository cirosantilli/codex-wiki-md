<h1 id="m/m5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Condition on $X_m=k$ and apply the [Markov property](../../../../../markov-property.md) and time homogeneity:

$$
p_{ij}(m+n)=\sum_{k\in S}\mathbb P_i(X_m=k)\mathbb P(X_{m+n}=j\mid X_m=k)
=\sum_{k\in S}p_{ik}(m)p_{kj}(n).
$$

Thus the transition matrices satisfy $P(m+n)=P(m)P(n)$; since $P(1)=P$ and $P(0)=I$, induction gives $P(n)=P^n$. Averaging over the initial state gives

$$
\boxed{\mathbb P(X_n=i)=(\mu P^n)_i}.
$$

If $\mu P=\mu$, induction gives $\mu P^n=\mu$, so this probability equals $\mu_i$ for every $n$. This is stationarity of the initial distribution.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [M5](../../m5.md)
3. [M](../../../m.md)
4. [2008 printed variant](../../../../2008-printed-variant-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
