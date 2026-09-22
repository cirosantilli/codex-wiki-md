<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a path $\Gamma$,

$$
\{f(x)-f(y)\}^2
\leq|\Gamma|\sum_{e\in\Gamma}\{\nabla_ef\}^2
$$

by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Average over $\nu_{xy}$, multiply by $\widetilde Q(x,y)$, and sum. Reversing the order of summation in the definition of the two [Dirichlet forms](../../../../../../dirichlet-form-of-a-markov-chain.md) gives

$$
\mathcal E_{\widetilde P}(f,f)\leq B\mathcal E_P(f,f).
$$

Let $M=\max_x\pi(x)/\widetilde\pi(x)$. The variational formula for variance gives

$$
\operatorname{Var}_\pi f
=\min_c\sum_x\pi(x)(f(x)-c)^2
\leq M\operatorname{Var}_{\widetilde\pi}f.
$$

Take a nonconstant eigenfunction attaining the Rayleigh quotient $\gamma$ for $P$. Then

$$
\widetilde\gamma
\leq\frac{\mathcal E_{\widetilde P}(f,f)}
{\operatorname{Var}_{\widetilde\pi}f}
\leq MB\frac{\mathcal E_P(f,f)}{\operatorname{Var}_\pi f}
=\boxed{MB\gamma}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
