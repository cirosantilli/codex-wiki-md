<h1 id="8f/solution">Solution</h1>

↑ **Parent:** [8F](../8f.md)

For an $n\times n$ [matrix](../../../../../matrix.md) $A$, the characteristic [polynomial](../../../../../polynomial-split.md) is

$$
\chi_A(t)=\det(tI-A).
$$

The [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem.md) states that $\chi_A(A)=0$.

Over $\mathbb C$, choose a [basis](../../../../../basis.md) in which $A$ is upper triangular, with diagonal entries $\lambda_1,\ldots,\lambda_n$. For the standard invariant flag $V_j=\langle e_1,\ldots,e_j\rangle$,

$$
(A-\lambda_jI)V_j\subseteq V_{j-1}.
$$

The factors $A-\lambda_jI$ commute, so applying their product in descending order sends $V_n$ successively into $V_{n-1},\ldots,V_0=0$. Hence

$$
0=\prod_{j=1}^n(A-\lambda_jI)=\chi_A(A),
$$

which proves the theorem.

Direct expansion gives the commutator product rule:

$$
\begin{aligned}
[X,YZ]
&=XYZ-YZX\\
&=(XY-YX)Z+Y(XZ-ZX)\\
&=[X,Y]Z+Y[X,Z].
\end{aligned}
$$

Put $C=[B,A]$. Since $C$ commutes with $A$, repeated use of the product rule gives

$$
[B,A^r]=\sum_{j=0}^{r-1}A^jCA^{r-1-j}=rA^{r-1}C.
$$

By [linearity](../../../../../linearity.md), for every [polynomial](../../../../../polynomial-split.md) $\varphi$,

$$
[B,\varphi(A)]=\varphi'(A)C.
$$

Let $D(X)=[B,X]$ and suppose $f(A)=0$. For $k=1$,

$$
f'(A)C=D(f(A))=0.
$$

Assume inductively that

$$
uC^m=0,
\qquad
u=f^{(k)}(A),\quad m=2^k-1.
$$

Both $u$ and $C$ are [polynomials](../../../../../polynomial-split.md) in, or commute with, $A$, so $uC^m=C^mu=0$. Apply the derivation $D$ to $uC^m=0$ and multiply on the left by $C^m$:

$$
0=C^mD(u)C^m+C^muD(C^m)=C^mD(u)C^m.
$$

Since $D(u)=f^{(k+1)}(A)C$, this says

$$
f^{(k+1)}(A)C^{2m+1}
=f^{(k+1)}(A)C^{2^{k+1}-1}=0.
$$

The induction is complete. Taking $f=\chi_A$ and $k=n$ gives

$$
n!\,C^{2^n-1}=0.
$$

**Thus $[B,A]$ is nilpotent, which is the [Jacobson lemma for a commuting commutator](../../../../../jacobson-lemma-for-a-commuting-commutator.md).**

## ↑ Ancestors (10)

1. [8F](../8f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
