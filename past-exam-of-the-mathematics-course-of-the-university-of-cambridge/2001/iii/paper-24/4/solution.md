<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

First stop the solution on leaving $[-n,n]$, at $\tau_n$, and set $F_n(t)=\mathbb E\sup_{u\leq t}|X_{u\wedge\tau_n}|^2$. The [stochastic integral](../../../../../stochastic-integral.md) representation, the [Doob L2 maximal inequality](../../../../../doob-l2-maximal-inequality.md) and the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) give, for $0\leq t\leq1$,

$$
\begin{aligned}
F_n(t)&\leq 2\mathbb E\sup_{u\leq t}\left|\int_0^{u\wedge\tau_n}\sigma(X_s)\,dB_s\right|^2
+2\mathbb E\sup_{u\leq t}\left|\int_0^{u\wedge\tau_n}b(X_s)\,ds\right|^2\\
&\leq 8\mathbb E\int_0^{t\wedge\tau_n}\sigma(X_s)^2\,ds
+2t\mathbb E\int_0^{t\wedge\tau_n}b(X_s)^2\,ds\\
&\leq8A\int_0^t(1+F_n(s))\,ds.
\end{aligned}
$$

Here stopping ensures square integrability before the calculation, and $8\sigma^2+2t b^2\leq8(\sigma^2+b^2)$ explains the constant. The [Gronwall inequality](../../../../../gronwall-inequality.md) gives $F_n(t)\leq e^{8At}-1$. For globally [Lipschitz functions](../../../../../lipschitz-continuity.md) as coefficients, the [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../../../global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients.md) supplies a nonexplosive solution. Letting $n$ increase and using [Fatou's lemma](../../../../../fatou-s-lemma.md) proves the slightly stronger [maximal second-moment bound under linear growth](../../../../../maximal-second-moment-bound-under-linear-growth.md):

$$
\boxed{\mathbb E\sup_{t\leq1}|X_t|^2\leq e^{8A}-1\leq e^{8A}.}
$$

For coefficients that are only [locally Lipschitz functions](../../../../../locally-lipschitz-function.md), let $\pi_n(x)=\max(-n,\min(x,n))$ and replace the coefficients by $\sigma(\pi_n(x))$ and $b(\pi_n(x))$. These are globally [Lipschitz functions](../../../../../lipschitz-continuity.md), agree with the originals on $[-n,n]$, and obey the same [linear growth condition for an SDE](../../../../../linear-growth-condition-for-an-sde.md), since $|\pi_n(x)|\leq|x|$. The globally defined solutions agree until their common exits from $[-n,n]$ by [pathwise uniqueness](../../../../../pathwise-uniqueness.md). The uniform preceding estimate and [Markov's inequality](../../../../../markov-inequality.md) imply

$$
\mathbb P(\tau_n\leq1)\leq\frac{e^{8A}-1}{n^2}\longrightarrow0.
$$

Patch the solutions before their increasing exit times. Their limiting lifetime exceeds $1$ almost surely by this bound. **Thus a pathwise unique strong solution exists throughout $[0,1]$ even for locally Lipschitz coefficients.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
