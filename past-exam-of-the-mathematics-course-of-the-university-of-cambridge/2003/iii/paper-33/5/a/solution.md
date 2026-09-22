<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The PDF defines multiplication by an indicator: $X_t=U\mathbf1_{\{V\geq e^{-t}\}}$. Put

$$
\boxed{T=-\log V=\inf\{t\geq0:X_t>0\}.}
$$

Then $T>0$ almost surely, $\{T\leq t\}=\{X_t>0\}\in\mathcal F_t$, and $T$ is a [stopping time](../../../../../../stopping-time.md). It has [exponential distribution](../../../../../../exponential-distribution.md) of rate one and is independent of $U$. The path stays at zero until $T$, jumps to $U$ at $T$, and remains there.

Let $p=\mathbb P(U\in B)$ and $N_t=\mathbf1_{\{T\leq t,U\in B\}}$. We verify the martingale property directly. On $\{T\leq s\}$ both increments $N_t-N_s$ and $(T\wedge t)-(T\wedge s)$ vanish. On $\{T>s\}$, every observation up to $s$ is zero, so the past reveals only that survival event. Conditional on it, $R=T-s$ is rate-one exponential by memorylessness and remains independent of the mark $U$. With $h=t-s$,

$$
\mathbb E[N_t-N_s\mid\mathcal F_s]=\mathbf1_{\{T>s\}}p(1-e^{-h}),
$$

while

$$
\mathbb E[(T\wedge t)-(T\wedge s)\mid\mathcal F_s]=\mathbf1_{\{T>s\}}\mathbb E(R\wedge h)=\mathbf1_{\{T>s\}}\int_0^he^{-r}dr.
$$

Subtracting $p$ times the second identity from the first gives zero. The process is adapted and integrable, since its absolute value is bounded by $1+pt$ on a finite horizon. Therefore

$$
\boxed{N_t-p(T\wedge t)\text{ is a martingale}.}
$$

On $\{T\leq t\}$ we have $X_t=U$, so this is exactly the requested process. This first-principles argument uses the natural filtration, which does not disclose the future mark or lifetime. It describes a [single marked exponential jump process](../../../../../../single-marked-exponential-jump-process.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
