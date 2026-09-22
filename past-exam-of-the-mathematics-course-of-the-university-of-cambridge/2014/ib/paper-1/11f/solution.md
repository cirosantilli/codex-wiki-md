<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

Two [Lipschitz equivalent norms](../../../../../equivalent-norms.md) $N_1,N_2$ satisfy $cN_1(v)\leq N_2(v)\leq CN_1(v)$ for all $v$, for constants $0<c\leq C<\infty$. These inequalities give the same convergent sequences in both norms. A subset of a [metric space](../../../../../metric-space.md) is [closed](../../../../../closed-set.md) exactly when it contains the limits of all convergent sequences from that subset. Therefore **closedness is the same in the two norms**.

For finite [dimension](../../../../../dimension-vector-space.md), fix a [basis](../../../../../basis.md) $e_1,\ldots,e_d$ and let $x=\sum_jx_je_j$. For any norm $N$,

$$
N(x)\leq\sum_j|x_j|N(e_j)\leq C\left(\sum_jx_j^2\right)^{1/2}.
$$

The reverse triangle inequality then makes $N$ continuous in the Euclidean coordinate norm. If no positive lower bound existed on the Euclidean unit sphere, choose $x_m$ there with $N(x_m)\to0$. By the [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md), a subsequence converges to $x$ on the unit sphere. Continuity would give $N(x)=0$, although $x\ne0$, a contradiction. Thus $N$ is bounded below by a positive multiple of the Euclidean norm. Comparing any two norms through that coordinate norm proves **all norms in finite dimension are Lipschitz equivalent**.

On $C[0,1]$, nonnegativity, absolute homogeneity and the triangle inequality for $\|f\|_1=\int_0^1|f|$ follow from the corresponding real-number properties and integration. If a continuous $f$ is nonzero at a point, it has absolute value bounded below by a positive constant on a nontrivial one-sided or two-sided interval around that point. Its integral is then positive. Hence $\|f\|_1=0$ implies $f=0$, completing the [norm](../../../../../norm.md) axioms.

For $n\geq2$, put $g_n(x)=\max\{1-n|x-1/2|,0\}$ and $f_n=1-g_n$. Then $f_n(1/2)=0$, but

$$
\|f_n-1\|_1=\int_0^1g_n(x)\,dx=\frac1n\longrightarrow0.
$$

The limit function $1$ is not in the indicated [point evaluation](../../../../../point-evaluation-functional.md) kernel. Consequently **that set is not closed in the integral norm**. This is the [point-evaluation kernel is not closed in the integral norm](../../../../../point-evaluation-kernel-is-not-closed-in-the-integral-norm.md) phenomenon.

Finally $\|g_n\|_\infty=1$ while $\|g_n\|_1=1/n$. Thus no constant can bound the [uniform norm](../../../../../supremum-norm.md) by a multiple of the integral norm. Although $\|f\|_1\leq\|f\|_\infty$ on this unit interval, the converse comparison fails: **the two norms are not Lipschitz equivalent**. The finite-dimensional theorem cannot be applied to this infinite-dimensional function space.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
