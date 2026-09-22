<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the continuous [adapted process](../../../../../../adapted-process.md) $X$, the supremum on each compact time interval is attained. Let $D_t=(\mathbb Q\cap[0,t])\cup\{t\}$. Continuity gives $\sup_{s\leq t}X_s=\sup_{r\in D_t}X_r$, and hence

$$
\{T\leq t\}=\{X_t^*\geq\lambda\}
=\bigcap_{m=1}^\infty\bigcup_{r\in D_t}\{X_r>\lambda-1/m\}\in\mathcal F_t.
$$

Each event inside the union is in $\mathcal F_r\subseteq\mathcal F_t$, so this proves carefully that $T$ is a [stopping time](../../../../../../stopping-time.md). Merely checking rational times for $X_r\geq\lambda$ would miss a path that touches the level at an isolated irrational time; the approximation from below avoids this issue. This is the [closed-level hitting times of continuous adapted processes](../../../../../../closed-level-hitting-times-of-continuous-adapted-processes.md) criterion. For $\lambda=0$, nonnegativity makes $T=0$ and the later inequality is immediate.

For $\lambda>0$, put $A=\{T\leq t\}$ and $\tau=T\wedge t$. On $A$, continuity implies $X_\tau\geq\lambda$. To justify the [optional sampling](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) step without extra filtration assumptions, round $\tau$ upwards to a finite dyadic grid in $[0,t]$, obtaining stopping times $\tau_n\downarrow\tau$. The event $A$ belongs to $\mathcal F_\tau$, and hence to $\mathcal F_{\tau_n}$: directly, $A\cap\{\tau\leq u\}=\{T\leq u\}$ for $u<t$, while for $u\geq t$ it is $A$. Discrete [optional sampling](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) for the sampled [submartingale](../../../../../../submartingale.md) gives

$$
\mathbb E(X_t\mathbf1_A)\geq\mathbb E(X_{\tau_n}\mathbf1_A).
$$

As $n\to\infty$, continuity gives $X_{\tau_n}\to X_\tau$. Nonnegativity and the [Fatou lemma](../../../../../../fatou-s-lemma.md) therefore yield

$$
\mathbb E(X_t\mathbf1_A)\geq\mathbb E(X_\tau\mathbf1_A)\geq\lambda\mathbb P(A).
$$

Consequently the [Doob maximal inequality for a nonnegative submartingale](../../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) takes the precise form

$$
\boxed{\lambda\mathbb P(X_t^*\geq\lambda)\leq\mathbb E\bigl(X_t\mathbf1_{\{X_t^*\geq\lambda\}}\bigr).}
$$

For the second-moment bound, suppose first that $\mathbb E X_t^2<\infty$; otherwise the inequality with an infinite right side is automatic. Set $M_R=X_t^*\wedge R$. The [layer cake representation](../../../../../../layer-cake-representation.md) and the preceding tail estimate give

$$
\begin{aligned}
\mathbb E M_R^2
&=2\int_0^R\lambda\mathbb P(X_t^*\geq\lambda)\,d\lambda\\
&\leq2\int_0^R\mathbb E\bigl(X_t\mathbf1_{\{X_t^*\geq\lambda\}}\bigr)d\lambda
=2\mathbb E(X_tM_R)\\
&\leq2\|X_t\|_2\|M_R\|_2.
\end{aligned}
$$

The integrands are nonnegative, so the interchange is justified by the [Tonelli theorem](../../../../../../tonelli-theorem.md). Since $M_R$ is bounded, division is legitimate when its norm is nonzero, giving $\|M_R\|_2\leq2\|X_t\|_2$; the zero-norm case is immediate. Finally, [monotone convergence](../../../../../../monotone-convergence-theorem.md) as $R\to\infty$ gives

$$
\boxed{\|X_t^*\|_2\leq2\|X_t\|_2.}
$$

This [truncated layer-cake proof of the L2 maximal inequality](../../../../../../truncated-layer-cake-proof-of-the-l2-maximal-inequality.md) proves square integrability of the maximum rather than assuming it during the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) step.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
