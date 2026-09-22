<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $T=A-zI$. The squares of the singular values of $TP_n^*$ are the eigenvalues of the finite-dimensional positive operator

$$
P_nT^*TP_n^*.
$$

The [Rayleigh-Ritz variational principle](../../../../../../rayleigh-ritz-variational-principle.md) and its min-max characterization show that, as the trial space grows, its $(j+1)$-st eigenvalue counted upward cannot increase. Therefore, for each fixed $j\geq0$,

$$
\boxed{\sigma_{n-j}^{(n)}(z,A)
\text{ decreases with }n}
$$

once $n>j$. Being nonnegative, it has a limit

$$
\boxed{
\sigma_{\inf+j}(A-zI)
=\lim_{n\to\infty}\sigma_{n-j}^{(n)}(z,A)}.
$$

The core assumption ensures that these Ritz limits are the min-max values of $T^*T$, rather than values for a smaller closed restriction.

For a normal operator, the spectral theorem gives three possibilities.


- If $z\notin\operatorname{Sp}(A)$, then $\|Tx\|\geq c\|x\|$ for some $c>0$, so every $\sigma_{\inf+j}\geq c$.
- If $z$ is a discrete eigenvalue of multiplicity $m$, exactly


$$
\sigma_{\inf}(T),\ldots,\sigma_{\inf+m-1}(T)
$$

vanish, while $\sigma_{\inf+m}(T)>0$.
- If $z$ lies in the essential spectrum, the min-max principle or an orthonormal Weyl sequence gives $\sigma_{\inf+j}(T)=0$ for every fixed $j$.

For $k\in\mathbb N$, define

$$
H_k(z,A)=\sum_{j=0}^k
\max\{0,1-k\sigma_{\inf+j}(A-zI)\}.
$$

In the first case $H_k=0$ for all sufficiently large $k$. In the second case its first $m$ summands tend to one and all remaining summands eventually vanish, so $H_k\to m$. In the third case $H_k=k+1\to+\infty$. These are exactly the three values in the definition of $h$, and hence

$$
\boxed{
h(z,A)=
\lim_{k\to\infty}
\sum_{j=0}^k
\max\{0,1-k\sigma_{\inf+j}(A-zI)\}}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
