<h1 id="25j/solution">Solution</h1>

↑ **Parent:** [25J](../25j.md)

Let $M$ be the [linear subspace](../../../../../vector-subspace.md) of $L^2(P)$ consisting of classes admitting $\mathcal G$-measurable representatives. It is closed. Indeed, if $Y_n\in M$ converges in $L^2$ to $Y$, choose a [subsequence](../../../../../subsequence.md) converging almost surely: take $\|Y_{n_j}-Y\|_2^2\le2^{-3j}$ and apply [Markov inequality](../../../../../markov-inequality.md) and the [Borel-Cantelli lemma](../../../../../borel-cantelli-lemmas.md) to errors exceeding $2^{-j}$. The pointwise limit of its $\mathcal G$-measurable representatives, set to zero wherever the finite limit does not exist, is $\mathcal G$-measurable and equals $Y$ almost surely. This also works when $\mathcal G$ is not complete.

Here is a proof of the [orthogonal projection](../../../../../orthogonal-projection.md) construction using only completeness. Put $d=\inf_{W\in M}\|X-W\|_2$ and take $W_n$ approaching this infimum. The [parallelogram law](../../../../../parallelogram-law.md) gives

$$
\|W_n-W_m\|_2^2=2\|X-W_n\|_2^2+2\|X-W_m\|_2^2-4\left\|X-\frac{W_n+W_m}{2}\right\|_2^2\longrightarrow0.
$$

Completeness and closedness give a minimizer $Y\in M$. For every $Z\in M$, expand $\|X-Y-tZ\|_2^2$ for real $t$. Its minimum at zero implies

$$
\boxed{E((X-Y)Z)=0\quad\text{for every }Z\in M.}
$$

This $Y$ is unique almost surely, because the difference of two possible choices belongs to $M$ and is orthogonal to itself. It is the [conditional expectation](../../../../../conditional-expectation.md) $E(X\mid\mathcal G)$, as also follows by testing indicators of events in $\mathcal G$.

For the jointly Gaussian pair, if $u>0$, set

$$
\boxed{Y=\nu+\frac vu(G-\mu).}
$$

The residual $R=X-Y$ has mean zero and [covariance](../../../../../covariance.md) $\operatorname{Cov}(R,G)=v-(v/u)u=0$. Since $(R,G)$ is jointly Gaussian, its characteristic function factors when this [covariance](../../../../../covariance.md) is zero, so $R$ and $G$ are independent. Hence $E(RZ)=E(R)E(Z)=0$ for every square-integrable function $Z$ of $G$; [independence](../../../../../independent-random-variables.md) first proves this for bounded functions, and truncation plus [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives the general case. This proves the [Gaussian conditional expectation](../../../../../gaussian-conditional-expectation.md) formula, including a zero residual [variance](../../../../../variance-split.md). If $u=0$, $G=\mu$ almost surely and the [covariance](../../../../../covariance.md) inequality gives $v=0$; **$Y=\nu$** is the answer.

## ↑ Ancestors (10)

1. [25J](../25j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
