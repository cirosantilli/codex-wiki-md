<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The overshoot hypothesis as printed cannot hold for every $R>0$.** For $R\leq1$, $T_R=0$ and $M_{T_R}=1$; choosing $R<1/\tau$ contradicts $M_{T_R}\leq\tau R$. The intended and sufficient assumption is the overshoot bound for $R\geq1$, on the event $\{T_R<\infty\}$. We use those thresholds below; when $R\leq1$, the requested stopped-time bound is trivial because $T\wedge T_R=0$.

Fix $R\geq1$ and set $S=T\wedge T_R$. By part (a), the stopped [martingale](../../../../../../martingale-split.md) satisfies $0\leq M_{S\wedge n}\leq\tau R$: before stopping it is below $R$, at $T$ it is zero, and at $T_R$ the assumed overshoot bound applies. Thus the square of this stopped process is integrable. For $\Delta M_n=M_{n+1}-M_n$,

$$
X_{n+1}-X_n
=\mathbf1_{\{S>n\}}\left(2M_n\Delta M_n+(\Delta M_n)^2-\sigma^2\right).
$$

The event $\{S>n\}$ is $\mathcal F_n$-measurable and contained in $\{T>n\}$. [Conditional expectation](../../../../../../conditional-expectation.md) of the linear term is zero, while the [variance](../../../../../../variance-split.md) assumption makes the remaining [conditional expectation](../../../../../../conditional-expectation.md) nonnegative. The stopped increments here are bounded by the stopping and overshoot bounds, so all [conditional expectations](../../../../../../conditional-expectation.md) are legitimate. Consequently

$$
\boxed{(X_n)_{n\geq0}\text{ is a submartingale}.}
$$

Since $X_0=1$, we have $\sigma^2\mathbb E(S\wedge n)\leq\mathbb E M_{S\wedge n}^2-1$. Bounded-time [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) also gives $\mathbb E M_{S\wedge n}=1$, so

$$
\mathbb E M_{S\wedge n}^2\leq\tau R\,\mathbb E M_{S\wedge n}=\tau R.
$$

Apply the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) to $S\wedge n$. This proves the stronger estimate $(\tau R-1)/\sigma^2$ and hence the requested [absorption-time bound from conditional variance and overshoot](../../../../../../absorption-time-bound-from-conditional-variance-and-overshoot.md):

$$
\boxed{\mathbb E(T\wedge T_R)\leq\frac{\tau R-1}{\sigma^2}\leq\frac{\tau^2R}{\sigma^2}\qquad(R\geq1).}
$$

In particular this stopping time is finite almost surely. For $0<R\leq1$, $S=0$ and $X_n=1$ is a constant [submartingale](../../../../../../submartingale.md), while the stopping-time [expectation](../../../../../../expected-value.md) is zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
