<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use $I_i=\mathbf1_{A_i}$ and interpret the printed overlap term as $2\Delta=\sum_i\sum_{j\in J_i}\Pr(A_i\cap A_j)$; its unindexed $A,B$ are a typographical slip. Take $i\notin J_i$, as usual. If necessary, deleting $i$ from its own neighbourhood gives the proof below with a smaller nonnegative right-hand side, so the stated bound still follows.

If $\lambda=0$, every indicator is zero almost surely and the [Poisson distribution](../../../../../poisson-distribution.md) with parameter zero is the same point mass. Suppose $\lambda>0$. For any $B\subseteq\mathbb Z_{\geq0}$, put $h_B(k)=\mathbf1_{k\in B}$ and let $Z$ have [Poisson distribution](../../../../../poisson-distribution.md) with mean $\lambda$. Solve the [Poisson Stein equation](../../../../../poisson-stein-equation.md)

$$
\lambda g(k+1)-kg(k)=h_B(k)-\Pr(Z\in B).
$$

For example, for $k\geq1$ one can take

$$
g(k)=\frac{(k-1)!}{\lambda^k}\sum_{j=0}^{k-1}
\frac{\lambda^j}{j!}[h_B(j)-\Pr(Z\in B)].
$$

The full weighted sum is zero, so using its complementary tail also shows this solution is bounded. The allowed Stein factor is $\|\Delta g\|_\infty\leq\min(1,\lambda^{-1})$, where $\Delta g(k)=g(k+1)-g(k)$.

Define

$$
V_i=\sum_{j\in J_i}I_j,\qquad W_i=W-I_i-V_i.
$$

Joint independence of $A_i$ from all [events](../../../../../event.md) outside its neighbourhood makes $I_i$ independent of $W_i$, so $p_i\mathbb Eg(W_i+1)=\mathbb EI_ig(W_i+1)$. Adding and subtracting those terms gives

$$
\begin{aligned}
\lambda\mathbb Eg(W+1)-\mathbb EWg(W)
&=\sum_i p_i\mathbb E[g(W+1)-g(W_i+1)]\\
&\quad+\sum_i\mathbb EI_i[g(W_i+1)-g(W)].
\end{aligned}
$$

A difference over $m$ integer steps has magnitude at most $m\|\Delta g\|_\infty$. In the first sum the step count is $I_i+V_i$; in the second, on $I_i=1$, it is $V_i$. Consequently the absolute value is at most

$$
\|\Delta g\|_\infty\left[
\sum_i p_i\left(p_i+\sum_{j\in J_i}p_j\right)
+\sum_i\sum_{j\in J_i}\mathbb EI_iI_j\right].
$$

The Stein equation identifies the left side with $|\Pr(W\in B)-\Pr(Z\in B)|$. Taking the supremum over $B$ is the definition of [total variation distance](../../../../../total-variation-distance.md), proving the [Stein-Chen bound with the Poisson Stein factor](../../../../../stein-chen-bound-with-the-poisson-stein-factor.md):

$$
\boxed{d_{TV}(\mathcal L(W),\operatorname{Po}(\lambda))
\leq\min(1,\lambda^{-1})
\left[\sum_i p_i^2+\sum_i\sum_{j\in J_i}p_ip_j+2\Delta\right].}
$$

For the random [uniform hypergraph](../../../../../uniform-hypergraph.md), index indicators by four-vertex [sets](../../../../../set-split.md). Each such [set](../../../../../set-split.md) is a [hypergraph clique](../../../../../complete-uniform-hypergraph.md) exactly when its four triples are all present, so its [probability](../../../../../probability.md) is $p^4$. Distinct [sets](../../../../../set-split.md) use disjoint triple indicators unless their intersection has size three; disjoint underlying trials give the required joint independence. A fixed four-set has $d=4(n-4)$ dependent others, and each overlapping pair requires seven distinct triples, with joint [probability](../../../../../probability.md) $p^7$. Thus, with $N=\binom n4$ and $\lambda=Np^4$, the bracket is

$$
N[(1+d)p^8+dp^7]=\lambda[(1+d)p^4+dp^3].
$$

Since $\lambda\min(1,\lambda^{-1})\leq1$,

$$
\boxed{d_{TV}(\mathcal L(W),\operatorname{Po}(\lambda))
\leq(4n-15)p^4+(4n-16)p^3\leq4np^4+4np^3.}
$$

This calculation applies for $n\geq4$ and $p>0$; if $p=0$ or $n<4$, the count and its Poisson parameter are zero and the conclusion is immediate.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
