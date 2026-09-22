<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $f_j(z)=f(p^jz)$ for $0\le j\le r$, and write $a=a_p(f)$ and $W_Mf=\varepsilon f$. The [Hecke operator](../../../../../../hecke-operator.md) $U_p$ acts on the Fourier expansion by $\sum a_nq^n\mapsto\sum a_{pn}q^n$. Since $p\mid M$, the primitive relation is $a_{pn}=a_pa_n$. Hence $U_pf_0=af_0$ and $U_pf_j=f_{j-1}$ for $j\ge1$. Substituting the argument directly in the [Fricke involution](../../../../../../fricke-involution.md) gives

$$
W_N f_j=\varepsilon p^{k(r/2-j)}f_{r-j}.
$$

Thus, in the basis $e_j=p^{jk/2}f_j$, put $b=p^{k/2}$ and let $R$ be the reversal matrix, $Re_j=e_{r-j}$. The matrices are

$$
\boxed{[U_p]=\begin{pmatrix}
a&b&0&\cdots&0\\
0&0&b&\cdots&0\\
\vdots&&\ddots&\ddots&\vdots\\
0&\cdots&0&0&b\\
0&\cdots&0&0&0
\end{pmatrix},\qquad[W_N]=\varepsilon R.}
$$

If the exam's rescaling $w_N=N^{k-1}W_N$ is used, multiply the second matrix by $N^{k-1}$.

Here is an explicit irreducibility argument for the [prime-power old block at a bad prime](../../../../../../prime-power-old-block-at-a-bad-prime.md). Any nonzero common invariant complex subspace $V$ contains an [eigenvector](../../../../../../eigenvector.md) of the restricted $U_p$. Its eigenvalue is either $a$ or zero. If $a\ne0$, the $a$-eigenspace is $\mathbb Ce_0$; containing it gives $e_r$ by reversal, then every $e_j$ by successive powers of $U_p$. The kernel of $U_p$ is $\mathbb C(e_1-(b/a)e_0)$. If $V$ instead contains this vector, reversal and $U_p^r$ give

$$
U_p^rR(e_1-(b/a)e_0)=b^{r-1}(a-b^2/a)e_0.
$$

This is nonzero: the [bad-prime eigenvalue of a trivial-character newform](../../../../../../bad-prime-eigenvalue-of-a-trivial-character-newform.md) satisfies $a^2=p^{k-2}$ when $p\parallel M$, and $a=0$ when $p^2\mid M$, whereas $b^2=p^k$. If $a=0$, the kernel is already $\mathbb Ce_0$, and the same reversal-and-shift argument works. Therefore **the block has no nonzero proper subspace invariant under $U_p$ and the Fricke operator**, and hence none invariant under the full ring in the question.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
