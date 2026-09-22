<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [integral curve of a vector field](../../../../../../integral-curve-of-a-vector-field.md) $X$ is a smooth curve $\gamma:I\to M$ satisfying $\dot\gamma(t)=X_{\gamma(t)}$ for every $t$ in its interval of definition. Passing through $p$ at time zero means $\gamma(0)=p$. The tangent-vector equality is intrinsic; in a [coordinate chart](../../../../../../manifold-chart.md) $x:U\to\mathbb R^n$ it becomes

$$
\frac{d}{dt}x^i(\gamma(t))=X^i(x(\gamma(t))).
$$

Smoothness makes the coordinate right side locally [Lipschitz continuous](../../../../../../lipschitz-continuity.md). The [Picard-Lindelöf theorem](../../../../../../picard-lindelof-theorem.md) supplies a locally unique solution through each coordinate initial value.

In fact, **two integral curves of $X$ with the same initial point agree throughout their common time interval containing zero**. To pass from local to global uniqueness, the set of coincidence times is nonempty and closed by [continuity](../../../../../../continuous-function.md) and the Hausdorff property of the [smooth manifold](../../../../../../smooth-manifold.md). At a coincidence time, put both curves in one [coordinate chart](../../../../../../manifold-chart.md); local [ordinary differential equation](../../../../../../ordinary-differential-equation.md) uniqueness makes them agree on a neighborhood of that time. Thus the coincidence set is open as well as closed in the connected common interval, so it is the whole interval. This argument applies around any prescribed time, not only zero.

By joining all extensions that agree on overlaps, one obtains the unique maximal [integral curve of a vector field](../../../../../../integral-curve-of-a-vector-field.md) through $p$. Its maximal interval need not be all of $\mathbb R$: completeness is an additional property of the [vector field](../../../../../../vector-field.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
