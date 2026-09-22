<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $n\geq1$, choose the integer $m$ with

$$
3^m\leq n\lt3^{m+1}
$$

and define the partial sum

$$
p_n(x)=\sum_{k=0}^ma_kT_{3^k}(x).
$$

It belongs to $\mathcal P_n$, and the [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
\|f_0-p_n\|_\infty\leq\sum_{k=m+1}^\infty a_k.
$$

At the $3^{m+1}+1$ points

$$
x_j=\cos\frac{j\pi}{3^{m+1}},
\qquad j=0,\ldots,3^{m+1},
$$

every tail term has the same alternating sign because

$$
T_{3^k}(x_j)
=\cos\left(j\pi3^{k-m-1}\right)=(-1)^j,
\qquad k\geq m+1.
$$

Thus

$$
f_0(x_j)-p_n(x_j)=(-1)^j
\sum_{k=m+1}^\infty a_k.
$$

There are at least $n+2$ such points because $n\lt3^{m+1}$. The [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) proves

$$
\boxed{p_n=\sum_{k=0}^ma_kT_{3^k}},
\qquad
\boxed{E_n(f_0)=\sum_{k=m+1}^\infty a_k},
\qquad 3^m\leq n\lt3^{m+1}.
$$

For $n=0$, the partial sum is empty and the same argument at $x=\pm1$ gives $p_0=0$ and $E_0(f_0)=\sum_{k=0}^\infty a_k$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
