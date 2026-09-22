<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Both functionals are finite on $X$: a [continuous function](../../../../../continuous-function.md) on the [compact metric space](../../../../../compact-metric-space.md) $[0,1]$ is bounded and integrable. Homogeneity follows from $|af|=|a||f|$, and the [triangle inequality](../../../../../triangle-inequality.md) follows by integrating, or taking the supremum of, $|f+g|\leq|f|+|g|$. Each is nonnegative. If $\|f\|_\infty=0$, then $f$ vanishes everywhere. If a [continuous function](../../../../../continuous-function.md) $f$ is nonzero at some point, continuity supplies an interval of positive length on which $|f|$ is bounded below by a positive number; hence $\|f\|_1>0$. Thus both are [norms](../../../../../norm.md).

For the nonnegative $f_n$, direct integration gives the [L1 norm](../../../../../l1-norm.md)

$$
\|f_n\|_1=n\int_0^1(t^n-t^{n+1})\,dt=\frac{n}{(n+1)(n+2)}\longrightarrow0.
$$

Therefore $\boxed{f_n\longrightarrow0\text{ in }\|\cdot\|_1}$. On the other hand, differentiation places the maximum of $t^n(1-t)$ at $t=n/(n+1)$, giving the [supremum norm](../../../../../supremum-norm.md)

$$
\|f_n\|_\infty=\left(\frac{n}{n+1}\right)^{n+1}\longrightarrow e^{-1}.
$$

For $t<1$, exponential decay implies $nt^n(1-t)\to0$, while $f_n(1)=0$. Thus the [pointwise convergence](../../../../../pointwise-convergence.md) is to zero throughout $[0,1]$. Any convergence in the [supremum norm](../../../../../supremum-norm.md) would imply [uniform convergence](../../../../../uniform-convergence.md), hence the same pointwise limit zero, contradicting the displayed positive limiting [norm](../../../../../norm.md). Therefore **there is no convergence in the supremum [norm](../../../../../norm.md)**.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
