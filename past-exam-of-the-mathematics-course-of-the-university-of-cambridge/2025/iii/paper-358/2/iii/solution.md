<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let

$$
L_n=\operatorname{span}\{e_1,\ldots,e_n\}
$$

and, for $w\in\mathbb C$, form the finite rectangular matrix

$$
M_{n_1,n_2}(w,A)
=\left(
\langle(A-wI)e_j,e_i\rangle
\right)_{\substack{1\leq i\leq n_1\\1\leq j\leq n_2}}.
$$

Every entry is available from $\Lambda$. Let its singular values, padded and ordered as in the question, be

$$
s_{n_2}^{(n_1,n_2)}
\leq\cdots\leq s_1^{(n_1,n_2)}.
$$

For fixed $n_2$, Parseval's identity gives convergence of the finite Gram matrices:

$$
M_{n_1,n_2}^*M_{n_1,n_2}
\longrightarrow
\left(
\langle(A-wI)e_j,(A-wI)e_\ell\rangle
\right)_{j,\ell\leq n_2}
$$

as $n_1\to\infty$. Consequently, if

$$
z_{n_2}=\lim_{n_1\to\infty}z_{n_2,n_1},
$$

then

$$
s_{n_2-j}^{(n_1,n_2)}(z_{n_2,n_1},A)
\longrightarrow
\sigma_{n_2-j}^{(n_2)}(z_{n_2},A).
$$

Singular values are Lipschitz under scalar shifts, so the subsequent limit $z_{n_2}\to z$ and part ii give

$$
\lim_{n_2\to\infty}\lim_{n_1\to\infty}
s_{n_2-j}^{(n_1,n_2)}(z_{n_2,n_1},A)
=\sigma_{\inf+j}(A-zI).
$$

Define the finite-information arithmetic functions

$$
\boxed{
h_{n_3,n_2,n_1}(w,A)
=
\sum_{j=0}^{\min\{n_3,n_2-1\}}
\max\left\{
0,\,
1-n_3s_{n_2-j}^{(n_1,n_2)}(w,A)
\right\}}.
$$

Finite-matrix singular values can be obtained by arithmetic eigenvalue approximation, so these functions form the required $\Delta_4^A$ arithmetic tower using only $\Lambda$. The two inner limits recover the limiting singular values, while the outer limit is exactly the multiplicity formula from part ii:

$$
\boxed{
\lim_{n_3\to\infty}
\lim_{n_2\to\infty}
\lim_{n_1\to\infty}
h_{n_3,n_2,n_1}(z_{n_2,n_1},A)
=h(z,A)}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
