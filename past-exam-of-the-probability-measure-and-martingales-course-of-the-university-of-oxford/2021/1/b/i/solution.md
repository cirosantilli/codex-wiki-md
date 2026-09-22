<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For every $n$, $\mathcal F_n$ is a [sigma-algebra](../../../../../sigma-algebra.md) contained in $\mathcal F$, and including one more [random variable](../../../../../random-variable-split.md) among its generators can only enlarge it. Hence $\mathcal F_n\subseteq\mathcal F_{n+1}$; the trivial $\mathcal F_0$ is contained in every [sigma-algebra](../../../../../sigma-algebra.md). These are exactly the requirements for a [filtration](../../../../../filtration-probability-theory.md).

The constant $X_0=x$ is $\mathcal F_0$-[measurable](../../../../../measurability.md). Suppose $X_n$ is $\mathcal F_n$-[measurable](../../../../../measurability.md). The pair $(X_n,U_{n+1})$ is then $\mathcal F_{n+1}$-[measurable](../../../../../measurability.md), and the [event](../../../../../event.md) $\{U_{n+1}\leq X_n\}$ is $\mathcal F_{n+1}$-[measurable](../../../../../measurability.md) because comparison of two real coordinates defines a [Borel set](../../../../../borel-set.md). Define its [indicator function](../../../../../indicator-function.md) by $B_{n+1}$. The recursion becomes

$$
X_{n+1}=\frac{X_n+B_{n+1}}2.
$$

It is a [measurable function](../../../../../measurable-function.md) of that pair. [Mathematical induction](../../../../../mathematical-induction.md) proves $X_n$ is $\mathcal F_n$-[measurable](../../../../../measurability.md) for every $n$, so **$(X_n)$ is an adapted process**. The same recursion also proves $0<X_n<1$ at every finite time, a useful bound for the later [integrability](../../../../../integrability.md) arguments.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
