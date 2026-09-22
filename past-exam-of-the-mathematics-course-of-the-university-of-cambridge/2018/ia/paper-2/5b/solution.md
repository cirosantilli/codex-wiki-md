<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

After multiplying by the inverse of the derivative matrix, the system is

$$
\dot z+Az=e^{-4t}\binom{2}{3b/2-1}+e^{-t}\binom{c-1}{-c/2-1},
\quad
A=\begin{pmatrix}2&-1\\-2&3\end{pmatrix}.
$$

Choose eigenvectors $(1,1)^T$ and $(-1/2,1)^T$ of eigenvalues $1$ and $4$, and write

$$
\binom xy=
\begin{pmatrix}1&-1/2\\1&1\end{pmatrix}\binom{w_1}{w_2}.
$$

Then

$$
\begin{aligned}
\dot w_1+w_1&=(b/2+1)e^{-4t}+(c/2-1)e^{-t},\\
\dot w_2+4w_2&=(b-2)e^{-4t}-ce^{-t}.
\end{aligned}
$$

The zero initial data give

$$
\boxed{\begin{aligned}
w_1&=\frac{b+2}{6}(e^{-t}-e^{-4t})+\frac{c-2}{2}te^{-t},\\
w_2&=(b-2)te^{-4t}-\frac c3(e^{-t}-e^{-4t}),\\
x&=w_1-\frac12w_2,\qquad y=w_1+w_2.
\end{aligned}}
$$

The $te^{-4t}$ and $te^{-t}$ terms are [resonant responses](../../../../../resonance.md). When $b=2$ or $c=2$, respectively, the corresponding resonant forcing vanishes and so does that secular factor.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
