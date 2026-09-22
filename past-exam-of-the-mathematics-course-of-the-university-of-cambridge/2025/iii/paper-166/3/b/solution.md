<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write

$$
P(X)=\sum_{j=0}^np_jX^j,
\qquad
Q(X)=\sum_{j=0}^nq_jX^j,
$$

so there are $N=2(n+1)$ unknown integer coefficients. Let $t$ be the number of integers $r$ with

$$
0\leq r<\frac{(2-\kappa)n}{d}-1.
$$

For each such $r$, impose the linear equation over $K=\mathbb Q(\alpha)$

$$
L_r(\mathbf p,\mathbf q)
=D_r(P+\alpha Q)(\alpha)
=0,
$$

where $D_r$ is the [normalized derivative of a polynomial](../../../../../../normalized-derivative-of-a-polynomial.md). The coefficient of $p_j$ is $\binom jr\alpha^{j-r}$ and that of $q_j$ is $\binom jr\alpha^{j-r+1}$. The local definition of [projective height](../../../../../../projective-height.md), together with $\binom jr\leq2^n$, gives

$$
H_p(L_r)\leq C_0^n
$$

for a constant $C_0$ depending only on $\alpha$.

There are $M=t$ forms over the degree-$d$ field $K$, and

$$
dM<(2-\kappa)n-d<N.
$$

Moreover $N-dM\geq\kappa n+2$. Applying [Siegel lemma](../../../../../../siegel-s-lemma.md) gives a nonzero integral coefficient vector with

$$
\max\{H(P),H(Q)\}
\leq(NC_0^n)^{dM/(N-dM)}
\leq C_1^n,
$$

because the exponent is bounded in terms of $\kappa$ and every fixed power of $n$ is at most exponential in $n$. These $P,Q$ have all the required vanishing normalized derivatives.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 166](../../../paper-166-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
