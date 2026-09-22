<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $M=\sup_{\gamma>1}F_\gamma(H_\gamma)<\infty$. Choose $\gamma_j\to\infty$. Boundedness of the [minimizers](../../../../../../global-minimizer.md) and the [Bolzano-Weierstrass theorem](../../../../../../bolzano-weierstrass-theorem.md) yield a [subsequence](../../../../../../subsequence.md), still indexed by $j$, with $H_{\gamma_j}\to H^*\in\mathbb R^n$. Each $H_{\gamma_j}$ is deterministic, hence so is $H^*$. The first exponential term gives

$$
H_{\gamma_j}\cdot p-x\leq\frac{\log M}{\gamma_j},
$$

and passing to the limit gives $H^*\cdot p\leq x$.

To obtain the [superhedging](../../../../../../superhedging.md) inequality, suppose instead that $\mathbb P(X>H^*\cdot P)>0$. There is then an $\varepsilon>0$ such that the event $E=\{X-H^*\cdot P\geq\varepsilon\}$ has positive [probability](../../../../../../probability.md). Let $\|P\|\leq B$ [almost surely](../../../../../../almost-sure-convergence.md). For all sufficiently large $j$,

$$
|(H_{\gamma_j}-H^*)\cdot P|\leq B\|H_{\gamma_j}-H^*\|\leq\varepsilon/2.
$$

Consequently $X-H_{\gamma_j}\cdot P\geq\varepsilon/2$ on $E$, giving

$$
M\geq F_{\gamma_j}(H_{\gamma_j})
\geq\mathbb P(E)e^{\gamma_j\varepsilon/2}\longrightarrow\infty,
$$

a contradiction. **The limiting portfolio meets both constraints**:

$$
\boxed{H^*\cdot p\leq x,\qquad H^*\cdot P\geq X\quad\text{almost surely}.}
$$

Bounded $P$ is used precisely to turn convergence of deterministic holdings into a uniform bound on the payoff error.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
