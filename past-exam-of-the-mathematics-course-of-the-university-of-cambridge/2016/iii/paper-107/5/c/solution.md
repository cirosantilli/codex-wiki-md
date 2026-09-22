<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $\Omega'$ nonempty and compactly contained in $\Omega$. The argument is a [compactness proof of a nonnegative elliptic solution estimate](../../../../../../compactness-proof-of-a-nonnegative-elliptic-solution-estimate.md), with the [global Schauder estimate](../../../../../../global-schauder-estimate.md) retaining control all the way to the boundary. The operator and the [Hölder space](../../../../../../holder-space.md) exponent are fixed throughout.

Suppose the estimate fails. For each integer $k$ there is an admissible nonnegative solution $u_k$, with forcing $f_k$, such that

$$
M_k:=\sup_\Omega u_k>k\left(\inf_{\Omega'}u_k+\|f_k\|_{C^{0,\mu}(\overline\Omega)}\right).
$$

Put $v_k=u_k/M_k$ and $g_k=f_k/M_k$. Then $0\leq v_k\leq1$, $\max_{\overline\Omega}v_k=1$, $v_k=0$ on the boundary, $Lv_k=g_k$, and

$$
\inf_{\Omega'}v_k<\frac1k,\qquad
\|g_k\|_{C^{0,\mu}(\overline\Omega)}<\frac1k.
$$

Global [elliptic regularity](../../../../../../elliptic-regularity.md) and the [global Schauder estimate](../../../../../../global-schauder-estimate.md) for zero [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) give

$$
\|v_k\|_{C^{2,\mu}(\overline\Omega)}\leq C\left(\|v_k\|_{C^0(\overline\Omega)}+\|g_k\|_{C^{0,\mu}(\overline\Omega)}\right)\leq2C.
$$

This estimate includes the $C^0$ term, so it does not require invertibility of $L$ or a sign restriction on $c$. The [compact embedding of Hölder spaces](../../../../../../compact-embedding-of-holder-spaces.md), or the [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) applied through second [partial derivatives](../../../../../../partial-derivative.md), gives a subsequence converging in $C^2(\overline\Omega)$ to $v$. Thus $v\geq0$, $Lv=0$, $v=0$ on the boundary, and $\max v=1$.

Choose $x_k\in\Omega'$ with $v_k(x_k)\leq\inf_{\Omega'}v_k+1/k$. A further subsequence has $x_k\to x_*\in\overline{\Omega'}\subset\Omega$. [Uniform convergence](../../../../../../uniform-convergence.md) yields $v(x_*)=0$. Part (b) says that a nonnegative homogeneous solution on the [connected](../../../../../../connected-space.md) domain is either zero everywhere or strictly positive inside. Both alternatives contradict, respectively, $\max v=1$ and $v(x_*)=0$. Therefore

$$
\boxed{\sup_\Omega u\leq C(n,L,\Omega',\Omega)\left(\inf_{\Omega'}u+\|f\|_{C^{0,\mu}(\overline\Omega)}\right).}
$$

**The interior infimum and the forcing control the global supremum.** Global boundary control is crucial here: an interior-only [compactness](../../../../../../compact-space.md) argument could lose the normalized maximum at the boundary.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
