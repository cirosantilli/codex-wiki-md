<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For [probability distributions](../../../../../probability-distribution.md) $p$ and $q$ on a finite alphabet, their classical [relative entropy](../../../../../kullback-leibler-divergence.md) in bits is

$$
D(p\|q)=\sum_{x:p(x)>0}p(x)\log_2\frac{p(x)}{q(x)}.
$$

A zero-$p$ term contributes zero, including when $q(x)=0$; a term with $p(x)>0$ and $q(x)=0$ makes the result $+\infty$. In that infinite case nonnegativity is immediate. Otherwise $q(x)>0$ on the support $J_p$ of $p$. For every $u>0$, $\ln u\leq u-1$: the function $u-1-\ln u$ has derivative $1-1/u$ and its minimum zero at $u=1$. Apply this with $u=q(x)/p(x)$ to obtain

$$
\begin{aligned}
D(p\|q)&=-\frac1{\ln2}\sum_{x\in J_p}p(x)\ln\frac{q(x)}{p(x)}\\
&\geq\frac1{\ln2}\sum_{x\in J_p}[p(x)-q(x)]\\
&=\frac{1-\sum_{x\in J_p}q(x)}{\ln2}\geq0.
\end{aligned}
$$

The last inequality uses normalization of $q$. Thus $\boxed{D(p\|q)\geq0}$. Equality requires $q(x)=p(x)$ wherever $p(x)>0$ and no $q$-mass outside that support, hence occurs precisely when $p=q$.

For [density matrices](../../../../../density-matrix.md), use

$$
S(\rho\|\sigma)=\operatorname{Tr}\rho(\log_2\rho-\log_2\sigma)
$$

when the [support of a positive operator](../../../../../support-of-a-positive-operator.md) $\rho$ is contained in that of $\sigma$, and set it to $+\infty$ otherwise. The [data-processing inequality for quantum relative entropy](../../../../../data-processing-inequality-for-quantum-relative-entropy.md) states that for any [quantum channel](../../../../../quantum-channel.md) $\Phi$,

$$
\boxed{S(\Phi(\rho)\|\Phi(\sigma))\leq S(\rho\|\sigma).}
$$

Thus the relative entropy of the two output states cannot exceed that of the inputs.

For the states with a classical flag, omit indices of weight zero. On a positive-weight block, the [matrix logarithms](../../../../../matrix-logarithm.md) obey

$$
\log_2(p_i\rho_i)=(\log_2p_i)I+\log_2\rho_i,
\qquad
\log_2(p_i\sigma_i)=(\log_2p_i)I+\log_2\sigma_i
$$

on the relevant supports. The logarithms of $p_i$ cancel. Taking the trace block by block therefore gives the [relative entropy of classically flagged states](../../../../../relative-entropy-of-classically-flagged-states.md):

$$
\boxed{S\!\left(\sum_ip_i|i\rangle\langle i|\otimes\rho_i\ \middle\|\
\sum_ip_i|i\rangle\langle i|\otimes\sigma_i\right)
=\sum_{i:p_i>0}p_iS(\rho_i\|\sigma_i).}
$$

If support inclusion fails in a positive-weight block, both sides are infinite. A zero-weight block makes no contribution, even if its unweighted relative entropy is infinite.

Tracing out the flag is a [quantum channel](../../../../../quantum-channel.md) with operators $A_i=\langle i|\otimes I$, since $\sum_iA_i^\dagger A_i=I$. It sends the two flagged states to $\sum_ip_i\rho_i$ and $\sum_ip_i\sigma_i$. Applying the [data-processing inequality for quantum relative entropy](../../../../../data-processing-inequality-for-quantum-relative-entropy.md) to this [partial trace](../../../../../partial-trace.md) proves [joint convexity of quantum relative entropy](../../../../../joint-convexity-of-quantum-relative-entropy.md):

$$
\boxed{S\!\left(\sum_ip_i\rho_i\ \middle\|\ \sum_ip_i\sigma_i\right)
\leq\sum_{i:p_i>0}p_iS(\rho_i\|\sigma_i).}
$$

For a bipartite state, set $\rho_A=\operatorname{Tr}_B\rho_{AB}$ and $\rho_B=\operatorname{Tr}_A\rho_{AB}$. Its [quantum mutual information](../../../../../quantum-mutual-information.md) is

$$
S(A:B)=S(\rho_A)+S(\rho_B)-S(\rho_{AB}),
$$

where $S(\tau)=-\operatorname{Tr}\tau\log_2\tau$ is the [Von Neumann entropy](../../../../../von-neumann-entropy-split.md). The support of $\rho_{AB}$ lies in $\operatorname{supp}\rho_A\otimes\operatorname{supp}\rho_B$. To justify this when marginals are singular, let $Q_A$ project onto $\ker\rho_A$. Then $\operatorname{Tr}[(Q_A\otimes I)\rho_{AB}]=\operatorname{Tr}(Q_A\rho_A)=0$; positivity implies $(Q_A\otimes I)\rho_{AB}=0$. Applying the same argument on $B$ proves the claimed support inclusion.

On that support, product eigenvectors show

$$
\log_2(\rho_A\otimes\rho_B)=\log_2\rho_A\otimes I+I\otimes\log_2\rho_B.
$$

The definition of the [partial trace](../../../../../partial-trace.md) therefore gives

$$
\begin{aligned}
S(\rho_{AB}\|\rho_A\otimes\rho_B)
&=\operatorname{Tr}\rho_{AB}\log_2\rho_{AB}
-\operatorname{Tr}\rho_A\log_2\rho_A
-\operatorname{Tr}\rho_B\log_2\rho_B\\
&=S(\rho_A)+S(\rho_B)-S(\rho_{AB}).
\end{aligned}
$$

Consequently $\boxed{S(A:B)=S(\rho_{AB}\|\rho_A\otimes\rho_B)}$.

For completeness, [nonnegativity of quantum relative entropy](../../../../../nonnegativity-of-quantum-relative-entropy.md) also follows from the classical proof above. Diagonalize $\rho$ in a basis $|j\rangle$, with [eigenvalues](../../../../../eigenvalue.md) $r_j$, and put $q_j=\langle j|\sigma|j\rangle$. These are two classical [probability distributions](../../../../../probability-distribution.md). Scalar concavity of the logarithm applied to the spectral weights of $\sigma$ gives $\langle j|\log_2\sigma|j\rangle\leq\log_2q_j$ whenever $r_j>0$ and support inclusion holds. Hence

$$
S(\rho\|\sigma)\geq\sum_{j:r_j>0}r_j\log_2\frac{r_j}{q_j}=D(r\|q)\geq0.
$$

The support-failure case is again infinite. Applying this to the product of the marginals proves $\boxed{S(A:B)\geq0}$ without requiring an additional entropy inequality.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
