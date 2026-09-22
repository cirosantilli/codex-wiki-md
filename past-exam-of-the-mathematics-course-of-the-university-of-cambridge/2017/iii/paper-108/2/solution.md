<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a probability [measure-preserving system](../../../../../measure-preserving-system.md), [strong mixing](../../../../../strong-mixing.md) means that for every pair of measurable sets $A,B$,

$$
\mu(T^{-n}A\cap B)\longrightarrow\mu(A)\mu(B).
$$

A sequence $a_n$ has [convergence in density of a sequence](../../../../../convergence-in-density-of-a-sequence.md) to $a$ when for each $\varepsilon>0$ the exceptional set $\{n:|a_n-a|\ge\varepsilon\}$ has [natural density](../../../../../natural-density.md) zero. A [weakly mixing measure-preserving transformation](../../../../../weakly-mixing-measure-preserving-transformation.md) has convergence in density of $\mu(T^{-n}A\cap B)$ to $\mu(A)\mu(B)$ for every $A,B$. Equivalently, because these correlations are bounded,

$$
\frac1N\sum_{n=0}^{N-1}|\mu(T^{-n}A\cap B)-\mu(A)\mu(B)|\longrightarrow0.
$$

Indeed the mean of the absolute discrepancy is at least $\varepsilon$ times the exceptional frequency, while it is at most $\varepsilon$ plus a uniform bound times that frequency. A signed [Cesaro convergence of a sequence](../../../../../cesaro-convergence-of-a-sequence.md) without absolute values is insufficient to define weak mixing.

The standard three-cut [Chacon map](../../../../../chacon-transformation.md) is obtained by [cutting and stacking](../../../../../cutting-and-stacking.md). Start on $[0,1)$ with normalized [Lebesgue measure](../../../../../lebesgue-measure.md), an initial tower consisting of $[0,2/3)$, and a reservoir $[2/3,1)$ for spacers. At stage $j$, cut every level of the current tower into three equal subintervals, producing three subcolumns. Add one new interval of the same width above the middle subcolumn. Stack the first subcolumn at the bottom, then the middle subcolumn with its spacer, then the third at the top. Define the partial transformation by translation from each level to the next, leaving the current top unmapped. These assignments extend the earlier partial transformation. Repeat indefinitely.

If $h_j$ is the number of levels and $w_j$ their width, then

$$
\boxed{h_0=1,\quad w_0=\frac23,\quad h_{j+1}=3h_j+1,\quad w_{j+1}=\frac{w_j}{3}}.
$$

Hence $h_j=(3^{j+1}-1)/2$, $w_j=2/3^{j+1}$, and the stage-$j$ tower has measure $1-3^{-j-1}$. The spacers consume total measure $\sum_{j\ge0}w_{j+1}=1/3$, precisely the reservoir. The increasing partial maps give the [Chacon map](../../../../../chacon-transformation.md) modulo null sets. The tower tops and unused reservoir have measures tending to zero, and the construction yields an invertible [measure-preserving transformation](../../../../../measure-preserving-transformation.md). With $0$ marking an original level and $1$ a spacer, the tower words satisfy $W_0=0$ and $W_{j+1}=W_jW_j1W_j$, so the first new word is $0010$. This describes the spacer placement without needing a proof of well-definedness. The three-cut convention agrees with the classical constant spacer vector $(0,1,0)$ described in [Ryzhikov's construction](https://arxiv.org/html/1311.4524v3).

For the correlation assertion, take the [L2 inner product](../../../../../l2-inner-product.md) to be $\langle u,v\rangle=\int u\overline v\,d\mu$, linear in its first argument, and put $U=U_T$. The [Koopman operator](../../../../../koopman-operator.md) is an [isometry](../../../../../isometry.md) on $L^2$, even when $T$ is not invertible. For $n\ge k$ the hint gives

$$
\langle U^nf,U^kf\rangle=\langle U^{n-k}f,f\rangle\longrightarrow|a|^2,\qquad a=\int f\,d\mu.
$$

To extend rigorously to all test functions, centre the observable: $v=f-a\mathbf1$. Invariance of the integral gives $\langle U^nv,v\rangle=\langle U^nf,f\rangle-|a|^2\to0$. Let

$$
M=\overline{\operatorname{span}}\{U^kv:k\ge0\}\subset L^2.
$$

For each fixed $k$, $\langle U^nv,U^kv\rangle\to0$ by the same [isometry](../../../../../isometry.md) identity. Therefore the limit is zero for every finite [linear combination](../../../../../linear-combination.md) of these orbit vectors. By the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and $\|U^nv\|_2=\|v\|_2$, approximation extends this conclusion to every $g\in M$: the approximation error in the correlation is bounded by $\|v\|_2\|g-g_0\|_2$ uniformly in $n$. For $g\in M^\perp$, the correlation is identically zero because $U^nv\in M$. The [orthogonal decomposition by a closed subspace](../../../../../orthogonal-decomposition-by-a-closed-subspace.md) now gives the result for all $g\in L^2$. Thus

$$
\boxed{\langle U_T^nf,g\rangle\longrightarrow a\int\overline g\,d\mu=\left(\int f\,d\mu\right)\left(\int\overline g\,d\mu\right)}.
$$

This is [decay of autocorrelation implies weak convergence of an observable](../../../../../decay-of-autocorrelation-implies-weak-convergence-of-an-observable.md); no assumption that $T$ is an [ergodic transformation](../../../../../ergodicity.md), and no invertibility hypothesis was used, and $a=0$ is included.

Finally, [strong mixing](../../../../../strong-mixing.md) immediately implies the stated diagonal limit by taking $B=A$. Conversely, suppose that limit holds for every $A$. Apply the correlation result with $f=\mathbf1_A$ and $g=\mathbf1_B$. Its hypothesis is exactly $\langle U^n\mathbf1_A,\mathbf1_A\rangle\to\mu(A)^2$, and its conclusion is

$$
\boxed{\mu(T^{-n}A\cap B)\longrightarrow\mu(A)\mu(B)\quad\text{for every }A,B}.
$$

Hence [strong mixing](../../../../../strong-mixing.md) is equivalent to [diagonal set-correlation criterion for mixing](../../../../../diagonal-set-correlation-criterion-for-mixing.md). Using the orbit-span proof avoids an invalid polarization argument that would recover only the sum of the two directed cross-correlations from diagonal correlations.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
