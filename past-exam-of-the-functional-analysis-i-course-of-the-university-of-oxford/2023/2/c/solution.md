<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $M=2^{1/p'}$, the common [operator norm](../../../../operator-norm.md) from part (b). Given $\varepsilon>0$, choose $N$ with $\|f-f_N\|_p<\varepsilon/(3M)$. Since $f_N\in Y$, the scalar limit of $T_hf_N$ exists. The [Cauchy criterion for a function limit](../../../../cauchy-criterion-for-a-function-limit.md) gives $\delta>0$ such that

$$
|T_hf_N-T_{\widetilde h}f_N|<\frac\varepsilon3
\qquad(0<h,\widetilde h<\delta).
$$

Using the [triangle inequality](../../../../triangle-inequality.md) and the uniform [operator norm](../../../../operator-norm.md) bound,

$$
\begin{aligned}
|T_hf-T_{\widetilde h}f|
&\leq|T_h(f-f_N)|+|T_hf_N-T_{\widetilde h}f_N|+|T_{\widetilde h}(f_N-f)|\\
&\leq2M\|f-f_N\|_p+|T_hf_N-T_{\widetilde h}f_N|<\varepsilon.
\end{aligned}
$$

This is the requested estimate. The [completeness](../../../../completeness.md) of $\mathbb R$ makes the scalar [Cauchy criterion for a function limit](../../../../cauchy-criterion-for-a-function-limit.md) sufficient, hence $\lim_{h\to0^+}T_hf$ exists and $f\in Y$.

For $u,v\in Y$ and real $a,b$, the [linearity](../../../../linearity.md) of $T_h$ gives $T_h(au+bv)=aT_hu+bT_hv$, which also has a limit. Thus $Y$ is a [linear subspace](../../../../vector-subspace.md). The preceding argument shows it contains every [norm convergence](../../../../norm-convergence.md) limit of its [sequences](../../../../sequence.md), so the sequential criterion for [closed sets](../../../../closed-set.md) in a [metric space](../../../../metric-space.md) gives

$$
\boxed{Y\text{ is a closed linear subspace of }X.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the functional analysis I course of the University of Oxford](../../../split.md)
5. [Functional analysis I course of the University of Oxford](../../../../functional-analysis-i-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
