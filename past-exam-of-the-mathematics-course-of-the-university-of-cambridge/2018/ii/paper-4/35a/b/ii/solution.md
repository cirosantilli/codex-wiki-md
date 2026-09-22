<h1 id="35a/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At $B=0$,

$$
M=\begin{pmatrix}a&b\\b&a\end{pmatrix},
\qquad a=e^{\beta J},\quad b=e^{-\beta J},
$$

with eigenvalues $\lambda_+=a+b=2\cosh(\beta J)$ and $\lambda_-=a-b=2\sinh(\beta J)$. Diagonalizing gives

$$
\boxed{M^p=\frac12
\begin{pmatrix}
\lambda_+^p+\lambda_-^p&\lambda_+^p-\lambda_-^p\\
\lambda_+^p-\lambda_-^p&\lambda_+^p+\lambda_-^p
\end{pmatrix}}.
$$

Substitution in part (i), together with $Z=\lambda_+^N+\lambda_-^N$, gives

$$
\langle s_1s_i\rangle
=\frac{\lambda_-^{i-1}\lambda_+^{N-i+1}
+\lambda_+^{i-1}\lambda_-^{N-i+1}}
{\lambda_+^N+\lambda_-^N}.
$$

Since $\lambda_-/\lambda_+=\tanh(\beta J)$, the required [One-dimensional Ising correlation function](../../../../../../../one-dimensional-ising-correlation-function.md) is

$$
\boxed{\langle s_1s_i\rangle
=\frac{\tanh^{i-1}(\beta J)+\tanh^{N-i+1}(\beta J)}
{1+\tanh^N(\beta J)}}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [35A](../../../35a.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
