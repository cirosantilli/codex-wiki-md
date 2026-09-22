<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Subtract $M_0$, which does not affect either the integral or its [quadratic variation](../../../../../../quadratic-variation.md). Let $N=M-M_0$. Choose a [localizing sequence](../../../../../../localizing-sequence.md) $\tau_n$ for $N$. By local boundedness of the [previsible process](../../../../../../predictable-process.md) $H$, there are increasing stopping times $\rho_n\uparrow\infty$ and finite deterministic constants $K_n$ with $|H_s|\leq K_n$ on $0<s\leq\rho_n$. Put

$$
\sigma_n=\tau_n\wedge\rho_n\wedge n\wedge\inf\{t:|N_t|\geq n\text{ or }[M]_t\geq n\}.
$$

Continuity and finiteness on compact intervals imply $\sigma_n\uparrow\infty$ almost surely. The stopped process $N^{\sigma_n}$ is a bounded square-integrable martingale, its bracket is bounded by $n$, and its stopped integrand is bounded by $K_n$. The indicator $\mathbf1_{\{s\leq\sigma_n\}}$ is predictable, so the stopped stochastic integral identity is valid.

Fix $n$ and abbreviate

$$
J_t=\int_0^{t\wedge\sigma_n}H_s\,dM_s,\qquad Q_t=\int_0^{t\wedge\sigma_n}H_s^2\,d[M]_s.
$$

The [Itô isometry](../../../../../../ito-isometry.md) gives $\mathbb E J_t^2=\mathbb E Q_t\leq K_n^2n$, so $J$ is a square-integrable martingale. For $F\in\mathcal F_s$, apply the same isometry to the predictable integrand $\mathbf1_F\mathbf1_{(s,t]}H$, stopped at $\sigma_n$. This yields

$$
\mathbb E\bigl[\mathbf1_F(J_t-J_s)^2\bigr]=\mathbb E\bigl[\mathbf1_F(Q_t-Q_s)\bigr].
$$

Also $\mathbb E[J_t-J_s\mid\mathcal F_s]=0$. Expanding $J_t^2-J_s^2$ therefore proves that $J^2-Q$ is a true martingale. The process $Q$ is continuous adapted increasing and starts at zero. By the characterization of continuous martingale [quadratic variation](../../../../../../quadratic-variation.md) as its increasing square compensator, and [uniqueness of an increasing square compensator](../../../../../../uniqueness-of-an-increasing-square-compensator.md), we have $[J]=Q$.

Stochastic integration and quadratic variation commute with stopping; for the latter this follows either from squared-increment sums or from the same square-compensator characterization. Hence the desired identity holds up to every $\sigma_n$. Since these times increase to infinity, they exhaust every finite time interval almost surely, and the continuous identities patch to give

$$
\boxed{[H\mathbin\cdot M]_t=\int_0^tH_s^2\,d[M]_s.}
$$

This is the [localized isometry proof of stochastic-integral quadratic variation](../../../../../../localized-isometry-proof-of-stochastic-integral-quadratic-variation.md). No unstopped second-moment or bracket-integrability assumption has been made.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
