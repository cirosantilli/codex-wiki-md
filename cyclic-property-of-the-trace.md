# Cyclic property of the trace

↑ **Parent:** [Matrix trace](matrix-trace.md)

If $A$ is an $m$-by-$n$ [matrix](matrix.md) and $B$ is an $n$-by-$m$ [matrix](matrix.md) over the same [field](field.md), both products are [square matrices](square-matrix.md) and

$$
\operatorname{tr}(AB)=\sum_{i=1}^m\sum_{j=1}^n a_{ij}b_{ji}
=\sum_{j=1}^n\sum_{i=1}^m b_{ji}a_{ij}=\operatorname{tr}(BA).
$$

The products can even have different sizes: for $A=(1\ \ 2)$ and $B=(3\ \ 4)^T$, $AB=(11)$ and $BA=\begin{pmatrix}3&6\\4&8\end{pmatrix}$, but both have [trace](matrix-trace.md) $11$.[Axler, Linear Algebra Done Right, fourth edition, §8D, result 8.49](linear-algebra-done-right-by-sheldon-axler-4th-edition.md)

Grouping all but one factor proves that $\operatorname{tr}(A_1A_2\cdots A_k)$ is unchanged by a cyclic permutation whenever the cyclic products are defined and square. In particular, every [commutator](commutator.md) has [trace](matrix-trace.md) zero, since $\operatorname{tr}(AB-BA)=0$ by [linearity](linearity.md).

Cyclic rotation does not allow arbitrary reordering. For

$$
A=\begin{pmatrix}1&0\\0&0\end{pmatrix},\quad
B=\begin{pmatrix}0&1\\0&0\end{pmatrix},\quad
C=\begin{pmatrix}0&0\\1&0\end{pmatrix},
$$

one has $ABC=A$, so $\operatorname{tr}(ABC)=1$, but $AC=0$, so $\operatorname{tr}(ACB)=0$. Rotating $ABC$ to $BCA$ or $CAB$ preserves its [trace](matrix-trace.md); swapping just $B$ and $C$ need not.

## ↑ Ancestors (6)

1. [Matrix trace](matrix-trace.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Cubic trace tensor of a Lie algebra representation](cubic-trace-tensor-of-a-lie-algebra-representation.md)
- [Killing-form invariance under a Lie-group adjoint action](killing-form-invariance-under-a-lie-group-adjoint-action.md)
- [Matrix trace](matrix-trace.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-62/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-68/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3/10h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-50/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-52/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-49/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-43/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-1/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-301/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-302/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-302/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/33c/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-325/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-304/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-102/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-102/1/iii/solution.md)
