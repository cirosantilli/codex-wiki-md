<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the [optimal three-to-one qubit random access code](../../../../../../optimal-three-to-one-qubit-random-access-code.md). For Alice's bits $(b_1,b_2,b_3)$, put $s_j=(-1)^{b_j}$ and send the [pure state](../../../../../../pure-state.md) with [Bloch vector](../../../../../../bloch-vector.md)

$$
\boxed{r_b=(s_1,s_2,s_3)/\sqrt3.}
$$

These are the eight vertices of a cube inscribed in the [Bloch sphere](../../../../../../bloch-sphere.md). If an explicit ket is wanted, choose $\cos\theta_b=s_3/\sqrt3$ and $e^{i\varphi_b}=(s_1+is_2)/\sqrt2$, and prepare $\cos(\theta_b/2)|0\rangle+e^{i\varphi_b}\sin(\theta_b/2)|1\rangle$.

Bob wanting bit $j$ performs a [Pauli measurement](../../../../../../measurement-of-a-pauli-observable.md) of $\sigma_x,\sigma_y,\sigma_z$ respectively, reporting zero for [eigenvalue](../../../../../../eigenvalue.md) $+1$ and one for $-1$. Its success for every input and every requested bit is

$$
\boxed{p_*=\frac12\left(1+\frac1{\sqrt3}\right)\simeq0.788675.}
$$

Only one chosen bit is extracted; the protocol does not recover all three simultaneously and uses no shared [entanglement](../../../../../../entangled-state.md).

To prove that no one-qubit protocol gives a greater guaranteed probability, allow Alice arbitrary mixed encoding vectors $|r_b|\le1$ and Bob any binary [positive operator-valued measure](../../../../../../positive-operator-valued-measure.md). Write his decision difference as $D_j=E_{j,0}-E_{j,1}=t_jI+v_j\cdot\sigma$. Its [eigenvalues](../../../../../../eigenvalue.md) lie in $[-1,1]$, implying $|v_j|\le1-|t_j|\le1$. On input $b$, success for bit $j$ is $[1+s_j(t_j+v_j\cdot r_b)]/2$. Average over all eight strings and three choices. The terms in $t_j$ cancel, leaving

$$
p_{\mathrm{avg}}=\frac12+\frac1{48}\sum_b r_b\cdot V_b
\le\frac12+\frac1{48}\sum_b|V_b|,\qquad V_b=\sum_{j=1}^3s_jv_j.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and cancellation of cross terms over all sign choices give

$$
\frac18\sum_b|V_b|\le\sqrt{\frac18\sum_b|V_b|^2}
=\sqrt{\sum_j|v_j|^2}\le\sqrt3.
$$

Hence $p_{\mathrm{avg}}\le p_*$. Any worst-case guarantee is no greater than this average; the cube protocol attains it uniformly, proving optimality both for guaranteed success and for the uniform-input average. Biased prior information about the bits would define a different optimization problem.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
