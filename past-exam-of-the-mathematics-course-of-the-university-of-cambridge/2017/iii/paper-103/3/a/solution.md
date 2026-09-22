<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a [Gelfand–Tsetlin basis](../../../../../../gelfand-tsetlin-basis.md) in [Young seminormal form](../../../../../../young-seminormal-form.md).

For a [standard Young tableau](../../../../../../standard-young-tableau.md) $T$, put $d=c_T(i+1)-c_T(i)$, using the [Content of a Young-diagram cell](../../../../../../content-of-a-young-diagram-cell.md). Choose the row-reading tableau $T_0$, and let $\ell(T)$ be the [Coxeter length](../../../../../../coxeter-length.md) of the unique permutation sending $T_0$ to $T$. A [Gelfand–Tsetlin basis](../../../../../../gelfand-tsetlin-basis.md) can be chosen so that, when $R=s_iT$ is standard and $\ell(R)=\ell(T)+1$,

$$
\boxed{s_iv_T=d^{-1}v_T+v_R,\qquad
s_iv_R=(1-d^{-2})v_T-d^{-1}v_R.}
$$

If $R$ is not standard, the action is $+v_T$ for two consecutive entries in one row, and $-v_T$ for two in one column. This is one usual normalization of the [Young seminormal form](../../../../../../young-seminormal-form.md).

Here is a construction and proof of the normalization. Fix $v_{T_0}\ne0$, let $P_T$ be the projection onto the tableau line, and define

$$
v_T=P_T\pi_Tv_{T_0}.
$$

The permutation $\pi_T$ has a reduced expression consisting entirely of admissible swaps, by the [reduced adjacent-swap path between linear extensions](../../../../../../reduced-adjacent-swap-path-between-linear-extensions.md). At each swap the off-diagonal coefficient is nonzero. In its expansion, the only term that can reach a tableau at distance $\ell(T)$ uses all $\ell(T)$ swaps; omitting a swap gives a shorter path. Thus $v_T\ne0$. This also makes its definition independent of a chosen reduced expression, because $\pi_T$ itself is fixed.

The relation $s_iX_is_i+s_i=X_{i+1}$ forces the coefficient of $v_T$ in $s_iv_T$ to be $1/d$, and forces every other component to lie on the swapped line. If length increases, project the identity $\pi_R=s_i\pi_T$ onto the line for $R$. The shorter terms of $\pi_Tv_{T_0}$ cannot reach $R$ in one step, so the coefficient of $v_R$ is exactly one. Applying $s_i^2=1$ then gives the reverse coefficient $1-d^{-2}$ and diagonal coefficient $-1/d$. In the nonstandard cases the same relation gives $d=\pm1$ and the asserted scalar action. This proves the theorem rather than merely specifying pairwise scalings.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
