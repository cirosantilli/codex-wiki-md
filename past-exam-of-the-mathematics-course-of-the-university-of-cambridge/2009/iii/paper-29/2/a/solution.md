<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The intended setting is $X=M+A$ with $A$ continuous and adapted. These conditions are needed for the requested continuous-semimartingale conclusion; [finite variation](../../../../../../total-variation-of-a-function.md) alone does not supply them. For example, $M=0$, $A_t=\mathbf1_{\{t\geq1\}}$ satisfies the printed deterministic bound and starts at zero, but $f_n(X)$ has a jump for sufficiently large $n$. We use the continuous adapted interpretation throughout this question.

Define $f_n(x)=\int_0^x\phi(ny)dy$. Then $f_n\in C^2$, $|f_n'|\leq1$ and $f_n''(x)=n\phi'(nx)\geq0$. The [Itô formula](../../../../../../ito-s-lemma.md) gives the canonical [continuous semimartingale decomposition](../../../../../../continuous-semimartingale-decomposition.md)

$$
\boxed{f_n(X_t)=N_t^{(n)}+V_t^{(n)},\quad N_t^{(n)}=\int_0^t f_n'(X_s)dM_s,\quad V_t^{(n)}=\int_0^t f_n'(X_s)dA_s+\frac12\int_0^t f_n''(X_s)d[M]_s.}
$$

The initial value is zero. The first term is a [continuous martingale](../../../../../../continuous-martingale.md), since $M$ is bounded and the integrand is bounded. The second is continuous adapted [finite variation](../../../../../../total-variation-of-a-function.md), hence predictable. This decomposition is unique because a [continuous finite-variation local martingale is constant](../../../../../../continuous-finite-variation-local-martingale-is-constant.md). The phrase Doob-Meyer here must mean this [semimartingale](../../../../../../semimartingale.md) decomposition: $V^{(n)}$ need not be nondecreasing, and the hypotheses do not make $f_n(X)$ a submartingale as required by the [Doob-Meyer decomposition theorem](../../../../../../doob-meyer-decomposition-theorem.md). Indeed $f_n'(0)=-1$, so the bounded deterministic drift $A_t=t\wedge\delta$ makes $f_n(A_t)$ initially decrease, excluding the submartingale property.

The sign process is predictable because it is a Borel function of the continuous adapted, and therefore predictable, process $X$. Its paths need not themselves be left-continuous. Pointwise, including at $x=0$,

$$
f_n'(x)=\phi(nx)\longrightarrow\operatorname{sgn}_-(x):=\mathbf1_{\{x>0\}}-\mathbf1_{\{x\leq0\}},\qquad|f_n'(x)-\operatorname{sgn}_-(x)|\leq2.
$$

For a fixed horizon $T$, $\mathbb E[M]_T=\mathbb EM_T^2\leq K^2$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) for the finite measure $\mathbb E\,d[M]$ on $[0,T]$ gives

$$
\mathbb E\int_0^T|f_n'(X_s)-\operatorname{sgn}_-(X_s)|^2d[M]_s\longrightarrow0.
$$

The [Itô isometry](../../../../../../ito-isometry.md), extended from simple predictable integrands by their density, and the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) now imply

$$
\mathbb E\sup_{t\leq T}\left|N_t^{(n)}-\int_0^t\operatorname{sgn}_-(X_s)dM_s\right|^2\leq4\mathbb E\int_0^T|f_n'(X_s)-\operatorname{sgn}_-(X_s)|^2d[M]_s\longrightarrow0.
$$

Hence

$$
\boxed{N^{(n)}\longrightarrow\operatorname{sgn}_-(X)\cdot M\text{ uniformly on compacts in probability}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
