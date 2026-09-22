# Penrose equations

↑ **Parent:** [Moore-Penrose inverse](moore-penrose-inverse.md)

The Moore--Penrose inverse is characterized by

$$
AA^\dagger A=A,
\quad
A^\dagger AA^\dagger=A^\dagger,
\quad
(AA^\dagger)^*=AA^\dagger,
\quad
(A^\dagger A)^*=A^\dagger A.
$$

Here $A^\dagger=A^+$ denotes the [Moore-Penrose inverse](moore-penrose-inverse.md), while the star denotes the [conjugate transpose](conjugate-transpose.md). The first two identities express consistency when applying and reversing the [linear map](linear-map.md); the last two make the resulting [orthogonal projection matrices](orthogonal-projection-matrix.md) [Hermitian](hermitian-operator.md). They must hold together. For example, $A=(1\ \ 2)$ and $B=(1\ \ 0)^T$ satisfy $ABA=A$ and $BAB=B$, but

$$
BA=\begin{pmatrix}1&2\\0&0\end{pmatrix}
$$

is not [Hermitian](hermitian-operator.md). This $B$ is a [right inverse](right-inverse.md), yet $Bb=(3,0)^T$ is not the [minimum-norm least-squares solution](minimum-norm-least-squares-solution.md) for $b=3$. The last two [Penrose equations](penrose-equations.md) impose the [orthogonality](orthogonal-vectors.md) that selects the [pseudoinverse](moore-penrose-inverse.md).

## ↑ Ancestors (7)

1. [Moore-Penrose inverse](moore-penrose-inverse.md)
2. [Matrix inverse](matrix-inverse.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Moore-Penrose inverse](moore-penrose-inverse.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-326/1/1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-326/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-326/1/b/iv/solution.md)
- [Penrose equations](penrose-equations.md)
