<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Introduce a parameter $t$ to keep track of total degree. The [power series](../../../../../power-series.md) for the [matrix exponential](../../../../../matrix-exponential.md) gives

$$
e^{tX}e^{tY}=I+t(X+Y)+t^2\left(\frac{X^2}{2}+XY+\frac{Y^2}{2}\right)+O(t^3).
$$

Set $S=X+Y$ and $C=\tfrac12[X,Y]$, where the [commutator](../../../../../commutator.md) is $[X,Y]=XY-YX$. Expanding a second [matrix exponential](../../../../../matrix-exponential.md) gives

$$
e^{tS+t^2C}=I+tS+t^2\left(C+\frac{S^2}{2}\right)+O(t^3).
$$

Since

$$
C+\frac{S^2}{2}=\frac12(XY-YX)+\frac12(X^2+XY+YX+Y^2)=\frac{X^2}{2}+XY+\frac{Y^2}{2},
$$

the two expressions agree through total degree two. More explicitly, applying the local [matrix logarithm](../../../../../matrix-logarithm.md) to the first expansion gives $\log(e^{tX}e^{tY})=t(X+Y)+\tfrac12t^2[X,Y]+O(t^3)$. This proves the displayed order of the [Baker--Campbell--Hausdorff formula](../../../../../baker-campbell-hausdorff-formula.md). The [Lie algebra](../../../../../lie-algebra-split.md) is closed under the [commutator](../../../../../commutator.md), so its displayed exponent lies in the same [Lie algebra](../../../../../lie-algebra-split.md). The expansion is a [formal power series](../../../../../formal-power-series.md) identity, or a convergent identity sufficiently near the [identity matrix](../../../../../identity-matrix.md); this argument does not assert unrestricted global convergence.

The next two terms of the [Baker--Campbell--Hausdorff formula](../../../../../baker-campbell-hausdorff-formula.md) are the two cubic [commutators](../../../../../commutator.md):

$$
\boxed{\log(e^Xe^Y)=X+Y+\frac12[X,Y]+\frac1{12}[X,[X,Y]]+\frac1{12}[Y,[Y,X]]+O(4).}
$$

Here $O(4)$ means total degree at least four in $X,Y$. If one continues by one more degree, the quartic contribution is $-\tfrac1{24}[Y,[X,[X,Y]]]$.

For the [Pauli matrices](../../../../../pauli-matrices.md), use the [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md)

$$
\tau_a\tau_b=\delta_{ab}I+i\epsilon_{abc}\tau_c.
$$

Put $N=\mathbf n\cdot\boldsymbol\tau$. The antisymmetric term disappears when contracted with $n_an_b$, so $N^2=|\mathbf n|^2I=I$. Consequently every even power of $N$ equals $I$, and every odd power equals $N$. Splitting the [matrix exponential](../../../../../matrix-exponential.md) into even and odd terms of its [power series](../../../../../power-series.md) yields

$$
\boxed{e^{i\alpha N}=\cos\alpha\,I+i\sin\alpha\,N.}
$$

The [Pauli matrices](../../../../../pauli-matrices.md) are [Hermitian matrices](../../../../../hermitian-operator.md), and the components of $\mathbf n$ are real, so $N^\dagger=N$. For real $\alpha$, the resulting matrix $U$ satisfies

$$
U^\dagger U=(\cos\alpha I-i\sin\alpha N)(\cos\alpha I+i\sin\alpha N)=I.
$$

Also $\operatorname{tr}N=0$ and $N^2=I$, so its two [eigenvalues](../../../../../eigenvalue.md) are $1,-1$. The [eigenvalues](../../../../../eigenvalue.md) of $U$ are therefore $e^{i\alpha},e^{-i\alpha}$, whose product is one. Thus $U$ is a [unitary matrix](../../../../../unitary-matrix.md) with [determinant](../../../../../determinant.md) one: **it belongs to the [SU(2) group](../../../../../su-2-group.md)**.

Multiplying the two exact [Pauli matrix](../../../../../pauli-matrices.md) exponentials, and using $\tau_1\tau_2=i\tau_3$, gives

$$
\boxed{e^{i\alpha\tau_1}e^{i\beta\tau_2}=\cos\alpha\cos\beta\,I+i\left(\sin\alpha\cos\beta\,\tau_1+\cos\alpha\sin\beta\,\tau_2-\sin\alpha\sin\beta\,\tau_3\right).}
$$

In particular, the $\tau_3$ term has a minus sign. Its quadratic [Taylor expansion](../../../../../taylor-expansion.md) is

$$
I+i\alpha\tau_1+i\beta\tau_2-i\alpha\beta\tau_3-\frac12(\alpha^2+\beta^2)I+O(3).
$$

Taking $X=i\alpha\tau_1$, $Y=i\beta\tau_2$, the [Pauli matrix commutator identity](../../../../../pauli-matrix-commutator-identity.md) gives $[X,Y]=-2i\alpha\beta\tau_3$. The quadratic exponent in the [Baker--Campbell--Hausdorff formula](../../../../../baker-campbell-hausdorff-formula.md) is therefore $Z=i\alpha\tau_1+i\beta\tau_2-i\alpha\beta\tau_3$. In $e^Z=I+Z+\tfrac12Z^2+O(3)$, only the linear part of $Z$ contributes to $Z^2$ through degree two. The anticommutator $\tau_1\tau_2+\tau_2\tau_1=0$ gives $Z^2=-(\alpha^2+\beta^2)I+O(3)$, reproducing the exact product's quadratic expansion.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
