<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use logarithms to base two, so all entropies are in bits. For a discrete [probability distribution](../../../../../probability-distribution.md) $p$ and a [density operator](../../../../../density-matrix.md) $\rho$ with [eigenvalues](../../../../../eigenvalue.md) $\lambda_j$, the [Shannon entropy](../../../../../information-entropy.md) and [Von Neumann entropy](../../../../../von-neumann-entropy-split.md) are respectively

$$
\boxed{H(p)=-\sum_xp_x\log_2p_x,\qquad
S(\rho)=-\operatorname{Tr}(\rho\log_2\rho)=-\sum_j\lambda_j\log_2\lambda_j.}
$$

Use $0\log0=0$. The second definition is basis-independent by the [spectral theorem](../../../../../spectral-theorem.md); for a density operator diagonal with probabilities $p_x$, it agrees with the first.

The classical [relative entropy](../../../../../kullback-leibler-divergence.md), or [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md), of $p$ from $q$ is

$$
\boxed{D(p\Vert q)=\sum_{x:p_x>0}p_x\log_2\frac{p_x}{q_x}.}
$$

It is $+\infty$ if some $p_x>0$ has $q_x=0$. The [quantum relative entropy](../../../../../quantum-relative-entropy.md) is

$$
\boxed{D(\rho\Vert\sigma)=\operatorname{Tr}\bigl[\rho(\log_2\rho-\log_2\sigma)\bigr]}
$$

when the support of $\rho$ is contained in that of $\sigma$, and is $+\infty$ otherwise. Matrix logarithms are taken on the corresponding positive supports. In a common eigenbasis this reduces to classical relative entropy; both divergences are nonnegative and are generally asymmetric.

To prove [Fano's inequality](../../../../../fano-s-inequality.md), let the finite alphabet size be $m\geq2$ and let $E$ indicate an incorrect guess. Since $E$ is determined by $(X,Y)$, the [chain rule for conditional entropy](../../../../../chain-rule-for-conditional-entropy.md) first gives

$$
H(E,X\mid Y)=H(X\mid Y)+H(E\mid X,Y)=H(X\mid Y).
$$

Expanding in the opposite order gives

$$
H(E,X\mid Y)=H(E\mid Y)+H(X\mid E,Y).
$$

[Conditioning reduces entropy](../../../../../conditioning-reduces-entropy.md), so $H(E\mid Y)\leq H(E)=h_2(p_e)$, the [binary entropy function](../../../../../binary-entropy-function.md). When $E=0$, knowledge of $Y$ determines $X=f(Y)$ and the conditional entropy is zero. When $E=1$, $X$ can lie in at most the $m-1$ alphabet values other than $f(Y)$. Entropy on $m-1$ values is at most $\log_2(m-1)$: its deficit from that number is the nonnegative [relative entropy](../../../../../kullback-leibler-divergence.md) from the uniform distribution. Averaging the two cases therefore gives

$$
H(X\mid E,Y)\leq p_e\log_2(m-1).
$$

Combining the two expansions proves

$$
\boxed{H(X\mid Y)\leq h_2(p_e)+p_e\log_2(m-1).}
$$

This proof of [Fano's inequality via an error indicator](../../../../../fano-s-inequality-via-an-error-indicator.md) works for any alphabet-valued guessing rule, not just an optimal one. If $m=1$, there is no guessing uncertainty and the claim is simply $H(X\mid Y)=0$; that case is treated separately rather than writing $\log0$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
