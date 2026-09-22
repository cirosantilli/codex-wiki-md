<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\eta(A)=\int_A X_\infty\,d\lambda$. This is a finite positive [measure](../../../../../../../measure.md). For $A\in\mathcal F_n$, the [conditional expectation](../../../../../../../conditional-expectation.md) inequality gives

$$
\eta(A)=\int_A\mathbb E[X_\infty\mid\mathcal F_n],d\lambda\leq\int_A X_n\,d\lambda=\mu(A).
$$

The union $\mathcal A=\bigcup_n\mathcal F_n$ is an algebra of sets generating $\mathcal B([0,1))$, since half-open [dyadic intervals](../../../../../../../dyadic-interval.md) generate all open sets and hence all Borel sets. The class $\{A:\eta(A)\leq\mu(A)\}$ is closed under increasing and decreasing limits, by continuity of these finite [measures](../../../../../../../measure.md). The [Monotone class theorem](../../../../../../../monotone-class-theorem.md) extends the inequality from $\mathcal A$ to every Borel set. Approximation by nonnegative simple functions and [monotone convergence](../../../../../../../monotone-convergence-theorem.md) then give

$$
\boxed{\mu(f)\geq\int fX_\infty\,d\lambda\quad\text{for every nonnegative measurable }f.}
$$

The difference $\nu=\mu-\eta$ is therefore a finite nonnegative [measure](../../../../../../../measure.md), not merely a signed [measure](../../../../../../../measure.md). For $A\in\mathcal F_n$,

$$
\nu(A)=\int_A\left(X_n-\mathbb E[X_\infty\mid\mathcal F_n]\right)d\lambda.
$$

Consequently its restricted [Radon-Nikodym derivative](../../../../../../../radon-nikodym-derivative.md) is

$$
\boxed{Y_n=X_n-\mathbb E[X_\infty\mid\mathcal F_n].}
$$

Choose the cell-average versions of all the [conditional expectations](../../../../../../../conditional-expectation.md). Then $Y_n$ is constant on each level-$n$ cell and equals $2^n\nu(D_k^n)$ there, so these versions are nonnegative at every point.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
