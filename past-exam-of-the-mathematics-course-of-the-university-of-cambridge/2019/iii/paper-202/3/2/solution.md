<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Since $B_{T_a}=0$, applying [Itô formula](../../../../../../ito-s-lemma.md) to $B_t^3$ after $T_a$ gives

$$
dX_t=3B_t\,dt+3B_t^2\,dB_t
=3\operatorname{sign}(X_t)|X_t|^{1/3}dt+3|X_t|^{2/3}dB_t.
$$

Before $T_a$, both sides vanish. Since $T_a$ is a stopping time determined by $B$, this is a [strong solution of a stochastic differential equation](../../../../../../strong-solution-of-a-stochastic-differential-equation.md).

Taking $a=0$ gives $X_t=B_t^3$, whereas any $a>0$ gives a solution that remains zero until $T_a$; these differ with positive probability while using the same Brownian motion and initial value. Therefore **pathwise uniqueness fails**.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
