<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the constant limit as $c$. First, [convergence in distribution to a constant implies convergence in probability](../../../../../../convergence-in-distribution-to-a-constant-implies-convergence-in-probability.md): the [Portmanteau theorem](../../../../../../portmanteau-theorem.md) applied to the closed set $\{y:|y-c|\geq\varepsilon\}$ gives

$$
\limsup_{n\to\infty}\mathbb P(|Y_n-c|\geq\varepsilon)\leq0.
$$

Now compare [characteristic functions](../../../../../../characteristic-function.md) without imposing [independence](../../../../../../independent-random-variables.md). For fixed $t\in\mathbb R$,

$$
\begin{aligned}
\left|\mathbb Ee^{it(X_n+Y_n)}-e^{itc}\mathbb Ee^{itX_n}\right|
&\leq\mathbb E|e^{itY_n}-e^{itc}|\\
&\leq |t|\varepsilon+2\mathbb P(|Y_n-c|>\varepsilon).
\end{aligned}
$$

The second bound uses $|e^{iu}-e^{iv}|\leq\min\{2,|u-v|\}$. By [convergence in probability](../../../../../../convergence-in-probability.md), the limiting upper bound is $|t|\varepsilon$; then let $\varepsilon\downarrow0$. Meanwhile $X_n$ has [weak convergence of random variables](../../../../../../convergence-in-distribution.md) to $X$, so $\mathbb Ee^{itX_n}\to\mathbb Ee^{itX}$. Thus the [characteristic function](../../../../../../characteristic-function.md) of the sum tends to $e^{itc}\mathbb Ee^{itX}$, the [characteristic function](../../../../../../characteristic-function.md) of $X+c$, which is [continuous](../../../../../../continuous-function.md) at zero. The [Lévy continuity theorem](../../../../../../levy-continuity-theorem.md) proves

$$
\boxed{X_n+Y_n\ \Longrightarrow\ X+c.}
$$

This is the additive case of the [Slutsky theorem](../../../../../../slutsky-theorem.md), with its proof supplied. The constant limiting marginal removes the dependence obstruction in part (b).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
