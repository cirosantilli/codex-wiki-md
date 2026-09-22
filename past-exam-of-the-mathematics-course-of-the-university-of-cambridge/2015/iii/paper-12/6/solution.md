<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use the part-preserving [bipartite four-cycle density](../../../../../bipartite-four-cycle-density.md) convention

$$
t_4(G)=\frac1{n^4}\sum_{x,x'\in X}\sum_{y,y'\in Y}
G(x,y)G(x,y')G(x',y)G(x',y').
$$

Here $G(x,y)$ is the [indicator function](../../../../../indicator-function.md) of adjacency, and repeated labels are allowed. This is the [homomorphism density](../../../../../homomorphism-density.md) convention appropriate to the [four-cycle norm](../../../../../box-norm.md). We derive the needed counting and [operator norm](../../../../../operator-norm.md) facts directly.

Let $M=(G(x,y))$ be the $n$-by-$n$ [biadjacency matrix](../../../../../biadjacency-matrix.md), let $\mathbf1$ be the all-ones [vector](../../../../../vector.md), let $J=\mathbf1\mathbf1^{\mathsf T}$, and put $H=M-\delta J$. The degree hypothesis says

$$
M\mathbf1=\delta n\mathbf1,\qquad M^{\mathsf T}\mathbf1=\delta n\mathbf1,
$$

so the centered [matrix](../../../../../matrix.md) $H$ annihilates $\mathbf1$ on both sides. In particular, $HJ=JH^{\mathsf T}=0$, and

$$
MM^{\mathsf T}=\delta^2nJ+HH^{\mathsf T}.
$$

The two terms have zero products in either order. Expanding the [matrix trace](../../../../../matrix-trace.md) directly counts four adjacency factors:

$$
\operatorname{tr}\bigl((MM^{\mathsf T})^2\bigr)
=\sum_{x,x',y,y'}M_{xy}M_{x'y}M_{x'y'}M_{xy'}=n^4t_4(G).
$$

Since $J^2=nJ$ and $\operatorname{tr}J=n$, we obtain

$$
n^4t_4(G)=\delta^4n^4+\operatorname{tr}\bigl((HH^{\mathsf T})^2\bigr).
$$

The given upper bound therefore implies

$$
\operatorname{tr}\bigl((HH^{\mathsf T})^2\bigr)\leq c^4\delta^4n^4.
$$

This computation proves the [centered four-cycle identity for a biregular graph](../../../../../centered-four-cycle-identity-for-a-biregular-graph.md), rather than assuming a [four-cycle norm](../../../../../box-norm.md) identity.

The [matrix](../../../../../matrix.md) $Q=HH^{\mathsf T}$ is a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md). By the [spectral theorem for real symmetric matrices](../../../../../spectral-theorem-for-real-symmetric-matrices.md) it has nonnegative [eigenvalues](../../../../../eigenvalue.md) $\lambda_j$, and

$$
\lambda_{\max}^2\leq\sum_j\lambda_j^2=\operatorname{tr}(Q^2).
$$

Moreover, for the [Euclidean norm](../../../../../euclidean-norm.md),

$$
\|H\|_{\mathrm{op}}^2=\lambda_{\max}(HH^{\mathsf T}).
$$

Indeed $\|H^{\mathsf T}v\|_2^2=v^{\mathsf T}Qv$, whose maximum on unit [vectors](../../../../../vector.md) is $\lambda_{\max}$; the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) characterization $\|H\|_{\mathrm{op}}=\sup_{\|u\|_2=\|v\|_2=1}|u^{\mathsf T}Hv|$ also shows that $H$ and $H^{\mathsf T}$ have the same [operator norm](../../../../../operator-norm.md). Taking fourth roots thus gives

$$
\|H\|_{\mathrm{op}}\leq c\delta n,
$$

where the error parameter $c$ is nonnegative, as in the claimed bound.

Finally use the [indicator vectors](../../../../../indicator-vector.md) $a=\mathbf1_A$, $b=\mathbf1_B$. Their [Euclidean norms](../../../../../euclidean-norm.md) are $\sqrt{|A|}$ and $\sqrt{|B|}$, so the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and the [operator norm](../../../../../operator-norm.md) estimate yield

$$
\begin{aligned}
|e(A,B)-\delta|A||B||
&=|a^{\mathsf T}Hb|\\
&\leq\|a\|_2\|H\|_{\mathrm{op}}\|b\|_2\\
&\leq c\delta n\sqrt{|A||B|}
=c\delta\sqrt{\alpha\beta}\,n^2.
\end{aligned}
$$

**This is the required discrepancy bound.** It also holds when either subset is empty or $\delta=0$. In fact, because $H$ annihilates constants, replacing $a,b$ by $a-\alpha\mathbf1,b-\beta\mathbf1$ gives the stronger bound $c\delta n^2\sqrt{\alpha(1-\alpha)\beta(1-\beta)}$. This is the [spectral discrepancy bound for a biregular graph](../../../../../spectral-discrepancy-bound-for-a-biregular-graph.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
