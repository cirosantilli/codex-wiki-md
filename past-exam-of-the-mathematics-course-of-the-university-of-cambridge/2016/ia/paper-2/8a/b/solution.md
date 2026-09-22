<h1 id="8a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a constant matrix, the [matrix exponential](../../../../../../matrix-exponential.md) series and its differentiated series converge uniformly on bounded time intervals, as follows by comparison with the scalar exponential in a [operator norm](../../../../../../operator-norm.md). Termwise [derivatives](../../../../../../derivative.md) therefore give

$$
\frac{d}{dt}e^{tM}=\sum_{n=1}^{\infty}\frac{t^{n-1}M^n}{(n-1)!}=Me^{tM},\qquad e^{0M}=I.
$$

Hence $\mathbf x(t)=e^{tM}\mathbf x_0$ solves the [initial value problem](../../../../../../initial-value-problem.md). For this particular matrix, direct multiplication gives $M^2=-I$. Splitting the [matrix exponential](../../../../../../matrix-exponential.md) into its even and odd powers proves

$$
\boxed{e^{tM}=I\cos t+M\sin t=\begin{pmatrix}\cos t+2\sin t&5\sin t\\-\sin t&\cos t-2\sin t\end{pmatrix}.}
$$

This is the [matrix exponential when the square is minus the identity](../../../../../../matrix-exponential-when-the-square-is-minus-the-identity.md). If $\mathbf x_0=(x_0,y_0)^{\mathsf T}$, the [general solution](../../../../../../general-solution.md) is

$$
\boxed{x(t)=x_0\cos t+(2x_0+5y_0)\sin t,\qquad y(t)=y_0\cos t-(x_0+2y_0)\sin t.}
$$

The constants in part (a) are $\alpha=x_0/5$ and $\beta=y_0+2x_0/5$, which makes the two forms identical.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8A](../../8a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
