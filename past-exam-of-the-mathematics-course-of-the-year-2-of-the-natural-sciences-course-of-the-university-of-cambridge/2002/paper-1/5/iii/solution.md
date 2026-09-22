<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The original PDF uses the [conjugate transpose](../../../../../conjugate-transpose.md) $N^\dagger$, rather than the transpose found in the transcription. The printed diagonalisation criterion is correct when diagonalisation means [unitary diagonalization of a normal matrix](../../../../../unitary-diagonalization-of-a-normal-matrix.md). Since $N^\dagger=A-iB$,

$$
NN^\dagger=A^2+B^2-i(AB-BA),\qquad N^\dagger N=A^2+B^2+i(AB-BA).
$$

Consequently $NN^\dagger=N^\dagger N$ if and only if $AB=BA$. By part (ii), this gives a common [unitary matrix](../../../../../unitary-matrix.md) $U$ and

$$
U^\dagger NU=D_A+iD_B,
$$

which is diagonal. Conversely, if $N=UDU^\dagger$ for a diagonal $D$ and a [unitary matrix](../../../../../unitary-matrix.md) $U$, then

$$
NN^\dagger=UDD^\dagger U^\dagger=UD^\dagger DU^\dagger=N^\dagger N.
$$

Thus the precise conclusion is

$$
\boxed{N\text{ is unitarily diagonalizable}\quad\Longleftrightarrow\quad N\text{ is normal}\quad\Longleftrightarrow\quad AB=BA.}
$$

If arbitrary invertible changes of basis are allowed, the printed assertion is false. For example,

$$
N=\begin{pmatrix}1&1\\0&2\end{pmatrix},\quad A=\begin{pmatrix}1&1/2\\1/2&2\end{pmatrix},\quad B=\begin{pmatrix}0&-i/2\\i/2&0\end{pmatrix}
$$

satisfy $N=A+iB$. Both [Hermitian matrices](../../../../../hermitian-operator.md) have distinct [eigenvalues](../../../../../eigenvalue.md): $(3\pm\sqrt2)/2$ for $A$ and $\pm1/2$ for $B$. The distinct [eigenvalues](../../../../../eigenvalue.md) $1,2$ make $N$ diagonalizable by similarity, but $NN^\dagger=\begin{pmatrix}2&2\\2&4\end{pmatrix}$ and $N^\dagger N=\begin{pmatrix}1&1\\1&5\end{pmatrix}$ differ. This distinguishes ordinary [diagonalization](../../../../../diagonalization-of-a-matrix.md) from the required unitary version.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
