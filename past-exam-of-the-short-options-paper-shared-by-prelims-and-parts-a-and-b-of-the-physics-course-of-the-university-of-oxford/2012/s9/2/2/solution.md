<h1 id="s9/2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The series is predictable in a statistical sense beyond linear return autocorrelation. For example, the observed past feature $Z_t=X_{t-1}X_{t-2}$ satisfies $\mathbb E[X_tZ_t]=1$ and $\mathbb EZ_t^2=4$, so its least-squares predictor within the family $bZ_t$ is $\boxed{\widehat X_t=Z_t/4}$. This is a predictor based on observed increments, not an assumption that the hidden driving signs are directly visible; it need not equal the full conditional expectation.

A finite bound on ordinary peak-to-trough [financial drawdown](../../../../../drawdown-economics.md) does **not** follow. Choose a long alternating sequence of driving signs, $a_t=(-1)^t$. It produces $X_t=-1+(-1)^t$, alternating $-2$ and $0$. The price never recovers during that episode and its cumulative loss grows without bound as the episode length grows. Every finite such driving sequence has positive [probability](../../../../../probability.md). Thus $\boxed{\text{no finite worst drawdown magnitude or duration exists without a horizon bound}.}$

More precisely, over an $N$-month window and over admissible starting histories, the maximum possible drawdown is

$$
\boxed{D_{\max}(N)=2\lfloor N/2\rfloor+2\quad(N\ge1).}
$$

One derivation keeps the last two signs as a four-state dynamic program. Let $d_n(a,b)$ be the smallest cumulative increment after $n$ steps ending with signs $(a,b)$, with $d_0(a,b)=0$ for each permitted initial pair. Then $d_{n+1}(b,c)=\min_{a=\pm1}[d_n(a,b)+ab+c]$. Induction gives the negative of the displayed minimum. The bound is attained by increments $(-2,0)^k,-2$ for $N=2k+1$, or $(-2,0)^{k-1},-2,-2$ for $N=2k$, so it is also an attained peak-to-trough loss over $N$ months, not only an algebraic net displacement bound.

For comparison, the index with increments $a_t=\pm1$ has $D_{\max}(N)=N$, attained by $N$ successive negative signs; it too has no finite horizon-free bound. If “drawdown” were intended to mean a **strictly decreasing consecutive run**, the first model permits at most two successive $-2$ increments, for a loss of four over two months, whereas the simple walk permits arbitrarily long such runs. That different run statistic must not be substituted for the usual drawdown definition: zero increments can separate continuing losses without any recovery.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [2](../../2.md)
3. [S9](../../../s9.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
