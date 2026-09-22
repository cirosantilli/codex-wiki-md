<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the [SI model](../../../../../../si-model.md), one infection reduces the susceptible count by one, and the total event rate is $\lambda X(t)Y(t)/n=n\,b(X_n(t))$, where $b(u)=\lambda u(1-u)$. The [Poisson time-change representation of a Markov chain](../../../../../../poisson-time-change-representation-of-a-markov-chain.md) therefore gives

$$
X_n(t)=a-\frac1nN_n\left(n\int_0^t b(X_n(s))\,ds\right),
$$

where $N_n$ is a unit-rate [Poisson process](../../../../../../poisson-process.md). Subtracting its clock from its count gives

$$
\boxed{\varepsilon_n(t)=\frac1n\left[
N_n\left(n\int_0^t b(X_n(s))\,ds\right)
-n\int_0^t b(X_n(s))\,ds\right]}.
$$

Thus $X_n(t)=a-\int_0^t b(X_n(s))\,ds-\varepsilon_n(t)$. The clock stops when the susceptible count reaches zero, so the representation also includes the absorbing state.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
