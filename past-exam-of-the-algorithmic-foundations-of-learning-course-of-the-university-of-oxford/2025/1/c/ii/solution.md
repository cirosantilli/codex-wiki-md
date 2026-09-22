<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We give a finite [chaining](../../../../../chaining.md) argument, keeping the constants explicit. If $\delta=0$, the [metric space](../../../../../metric-space.md) has just the point $t_0$ and both sides vanish. Suppose $\delta>0$, and write

$$
\varepsilon_k=2^{-k}\delta,\qquad N_k=N(\varepsilon_k;T,d),\quad k\geq1.
$$

Choose a smallest [metric net](../../../../../metric-net.md) $T_k\subseteq T$ of radius $\varepsilon_k$, and maps $\pi_k:T\to T_k$ satisfying $d(t,\pi_k(t))\leq\varepsilon_k$. Set $T_0=\{t_0\}$ and $\pi_0(t)=t_0$. Since $T$ is finite, choose $K$ with $\varepsilon_K$ smaller than the minimum distance between distinct points; then $T_K=T$ and $\pi_K(t)=t$.

For each $k$, retain only the pairs actually occurring along these approximation paths:

$$
E_k=\{(\pi_k(t),\pi_{k-1}(t)):t\in T\},\qquad m_k=|E_k|.
$$

The [triangle inequality](../../../../../triangle-inequality.md) gives $d(u,v)\leq\varepsilon_k+\varepsilon_{k-1}=3\varepsilon_k$ for $(u,v)\in E_k$; for $k=1$ the same argument uses $d(t,t_0)\leq\delta=\varepsilon_0$. Also

$$
m_1\leq N_1,\qquad m_k\leq N_kN_{k-1}\leq N_k^2\ (k\geq2),\qquad \log m_k\leq2\log N_k.
$$

Here only monotonicity in the radius for the same space $T$ is used. No monotonicity under subsets is assumed.

For every pair in $E_k$, the increment has the [Sub-Gamma random variable in the right tail](../../../../../sub-gamma-random-variable-in-the-right-tail.md) bound with common parameters $9\nu\varepsilon_k^2$ and $3c\varepsilon_k$: for $0<s<(3c\varepsilon_k)^{-1}$,

$$
\log\mathbb E e^{s(X_u-X_v)}
\leq\frac{\nu d(u,v)^2s^2}{2(1-cd(u,v)s)}
\leq\frac{9\nu\varepsilon_k^2s^2}{2(1-3c\varepsilon_ks)}.
$$

Identical pairs give the zero increment, which obeys the same bound. Both orientations have finite [exponential moments](../../../../../exponential-moment.md), so all increments are [integrable random variables](../../../../../integrable-random-variable.md). Differentiating their two upper bounds at zero also gives $\mathbb E(X_u-X_v)=0$. Applying the maximum bound from part (b), including its $m_k=1$ case, gives

$$
\begin{aligned}
\mathbb E\max_{(u,v)\in E_k}(X_u-X_v)
&\leq3\varepsilon_k\sqrt{2\nu\log m_k}+3c\varepsilon_k\log m_k\\
&\leq6\sqrt\nu\,\varepsilon_k\sqrt{\log N_k}+6c\varepsilon_k\log N_k.
\end{aligned}
$$

The [telescoping sum](../../../../../telescoping-sum.md) along each path is exact:

$$
X_t-X_{t_0}=\sum_{k=1}^K(X_{\pi_k(t)}-X_{\pi_{k-1}(t)}).
$$

Take the [supremum](../../../../../supremum.md), bound it by the sum of the maxima, and take [expected values](../../../../../expected-value-split.md). This proves

$$
\mathbb E\sup_{t\in T}(X_t-X_{t_0})
\leq6\sqrt\nu\sum_{k=1}^K\varepsilon_k\sqrt{\log N_k}
+6c\sum_{k=1}^K\varepsilon_k\log N_k.
$$

For either $f(u)=\sqrt{\log N(u;T,d)}$ or $f(u)=\log N(u;T,d)$, the function is nonnegative and nonincreasing. Thus

$$
\int_{\varepsilon_{k+1}}^{\varepsilon_k}f(u)\,du
\geq\frac{\varepsilon_k}{2}f(\varepsilon_k),\qquad
\sum_{k=1}^K\varepsilon_k f(\varepsilon_k)
\leq2\int_0^{\delta/2}f(u)\,du.
$$

Combining the estimates yields the required [metric entropy](../../../../../metric-entropy.md) bound:

$$
\boxed{\mathbb E\left[\sup_{t\in T}X_t-X_{t_0}\right]
\leq12\sqrt\nu\int_0^{\delta/2}\sqrt{\log N(u;T,d)}\,du
+12c\int_0^{\delta/2}\log N(u;T,d)\,du.}
$$

In particular, **$C=12$ and $C'=12$ work**. The square-root and linear [metric entropy](../../../../../metric-entropy.md) terms arise respectively from the two terms in the sub-Gamma maximum bound. Because the chain ends exactly at $T$, no limiting sample-path regularity assumption is needed.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the algorithmic foundations of learning course of the University of Oxford](../../../../split.md)
6. [Algorithmic foundations of learning course of the University of Oxford](../../../../../algorithmic-foundations-of-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
