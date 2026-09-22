# Spectrum of a three-dimensional matrix with zero row sums

↑ **Parent:** [Zero eigenvalue](zero-eigenvalue.md)

Consider

$$
B=\begin{pmatrix}-(a+b)&a&b\\c&-(c+d)&d\\e&f&-(e+f)\end{pmatrix}.
$$

Its row sums vanish, so $(1,1,1)^T$ is an [eigenvector](eigenvector.md) for the [zero eigenvalue](zero-eigenvalue.md). Its [characteristic polynomial](characteristic-polynomial.md) is

$$
\det(\lambda I-B)=\lambda(\lambda^2+S\lambda+T),\qquad S=a+b+c+d+e+f,
$$

with sum of [principal minors](principal-minor.md) of order two

$$
T=ad+bc+bd+ae+af+bf+ce+cf+de.
$$

The other [eigenvalues](eigenvalue.md) are $(-S\pm\sqrt{S^2-4T})/2$. No symmetry is required for this formula; [positive diagonal symmetrization of a matrix](positive-diagonal-symmetrization-of-a-matrix.md) is a sufficient condition for real roots.

## ↑ Ancestors (8)

1. [Zero eigenvalue](zero-eigenvalue.md)
2. [Eigenvalue](eigenvalue.md)
3. [Operator theory](linear-operator-theory-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-316/4/ii/solution.md)
