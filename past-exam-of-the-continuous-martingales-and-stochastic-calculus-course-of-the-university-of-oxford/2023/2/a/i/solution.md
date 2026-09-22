<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $0=t_0<t_1<\cdots<t_m<\infty$ and let $\xi_j$ be bounded $\mathcal F_{t_j}$-[measurable](../../../../../measurability.md) [random variables](../../../../../random-variable-split.md). For the bounded [simple predictable process](../../../../../simple-predictable-process.md)

$$
H_s=\sum_{j=0}^{m-1}\xi_j\mathbf1_{(t_j,t_{j+1}]}(s),
$$

the [Itô integral](../../../../../ito-integral.md) against a [continuous martingale](../../../../../continuous-martingale.md) $M\in\mathcal H^{2,c}$ is defined by the increment sum

$$
\boxed{(H\mathbin\cdot M)_t=\int_0^tH_s\,dM_s
:=\sum_{j=0}^{m-1}\xi_j\bigl(M_{t\wedge t_{j+1}}-M_{t\wedge t_j}\bigr).}
$$

The same definition applies to [elementary predictable processes with stopping-time intervals](../../../../../elementary-predictable-process-with-stopping-time-intervals.md), replacing $t_j$ by ordered [stopping times](../../../../../stopping-time.md) $T_j$ and taking bounded $\mathcal F_{T_j}$-[measurable](../../../../../measurability.md) coefficients. Refinement of the intervals leaves the increment sum unchanged. The initial value of the [integral](../../../../../integral-split.md) is zero, and its [martingale](../../../../../martingale-split.md) property follows from the [conditional expectation](../../../../../conditional-expectation.md) identity for subsequent increments of $M$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
