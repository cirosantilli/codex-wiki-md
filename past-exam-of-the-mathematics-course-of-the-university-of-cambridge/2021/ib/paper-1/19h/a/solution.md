<h1 id="19h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A random time $T$ is a [stopping time](../../../../../../stopping-time.md) when the event $\{T\leq n\}$ is determined by $X_0,\ldots,X_n$. The [Strong Markov property](../../../../../../strong-markov-property.md) says that, conditionally on $T<\infty$ and $X_T=x$, the process $(X_{T+k})_{k\geq0}$ is a fresh Markov chain started at $x$, independent of the history before $T$.

Use the state space $\{1,2,4\}\times\mathbb Z_{\geq0}$, with $(2,0)$ absorbing. Observe the chain only when it is at square 2. From $(2,k)$, the change $Y$ in wealth by the next return to square 2 has distribution

$$
\Pr(Y=-1)=\frac12,\qquad
\Pr(Y=1)=\frac18,\qquad
\Pr(Y=2)=\frac38.
$$

Indeed, heads lands on square 3 and returns to square 2 after losing £1. After tails reaches square 4, the remaining two or three moves give the other cases.

For $r=2/3$,

$$
\mathbb E[r^Y]
=\frac12r^{-1}+\frac18r+\frac38r^2=1.
$$

Thus $r^{M_j}$ is a [martingale](../../../../../../martingale-split.md) for the embedded wealth random walk $M_j$. Stopping when it first reaches $m-1$ or a large upper level and then letting that level tend to infinity gives

$$
\Pr_{(2,m)}(\text{ever hit }(2,m-1))=r=\boxed{\frac23}.
$$

The upper-bound contribution vanishes because $0<r<1$; equivalently, this is the smaller probability solution of the first-step equation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
