<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Z=(Z_n)_{n\geq0}$ be a [Markov chain](../../../../markov-chain-split.md) with [transition kernel](../../../../markov-kernel.md) $K$, and let $N$ be an independent [Poisson process](../../../../poisson-process-split.md) of constant rate $r>0$. A [Pseudo-Poisson process](../../../../pseudo-poisson-process.md) is $X_t=Z_{N_t}$. On the [Banach space](../../../../banach-space-split.md) $B_b(E)$ of bounded [Borel measurable functions](../../../../borel-measurable-function.md), with the [supremum norm](../../../../supremum-norm.md), write

$$
(Kf)(x)=\int_E f(y)K(x,dy),\qquad K^0=I.
$$

Its [infinitesimal generator](../../../../infinitesimal-generator-stochastic-processes.md), [transition semigroup](../../../../markov-semigroup.md), and [resolvent operator](../../../../resolvent-of-an-operator.md) are respectively

$$
\boxed{L=r(K-I),\qquad D(L)=B_b(E),}
$$



$$
\boxed{P_t=e^{tL}=e^{-rt}\sum_{n=0}^{\infty}\frac{(rt)^n}{n!}K^n,}
$$

and, for $\lambda>0$,

$$
\boxed{R_\lambda=\int_0^\infty e^{-\lambda t}P_t\,dt
=\frac1{\lambda+r}\sum_{n=0}^{\infty}\left(\frac r{\lambda+r}\right)^nK^n
=(\lambda I-L)^{-1}.}
$$

The [transition semigroup](../../../../markov-semigroup.md) averages $K^n$ against the [Poisson distribution](../../../../poisson-distribution.md) of the number of updates. Since $K$ is a [Markov operator](../../../../markov-operator.md), $\|K\|\leq1$; both series converge in [operator norm](../../../../operator-norm.md). Updates with $Z_{n+1}=Z_n$ are allowed and do not count as changes of the observed state. The degenerate rate $r=0$ gives $L=0$, $P_t=I$, and $R_\lambda=I/\lambda$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the stochastic analysis and partial differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic analysis and partial differential equations course of the University of Oxford](../../../../stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
