<h1 id="8f/solution">Solution</h1>

↑ **Parent:** [8F](../8f.md)

Multiplying numerator and denominator by the same nonzero constant does not change a [Möbius transformation](../../../../../mobius-transformation.md). Since $b\ne0$, divide by $b$ and relabel the coefficients so that $b=1$. On $|z|=1$, preservation of the circle gives

$$
|a+z|^2=|c+dz|^2.
$$

Equating the constant and first [Fourier coefficients](../../../../../fourier-coefficient.md) yields

$$
|a|^2+1=|c|^2+|d|^2,\qquad \bar a=\bar c\,d.
$$

If $c=0$, the second equality forces $a=0$, contradicting the nonzero [determinant](../../../../../determinant.md). Hence $d=\bar a/\bar c$. With $C=|c|^2>0$, the first equality becomes

$$
C^2-(1+|a|^2)C+|a|^2=0,
\qquad (C-1)(C-|a|^2)=0.
$$

The root $C=|a|^2$ would imply $ad=|a|^2/\bar c=c$, making the numerator and denominator proportional. It is excluded by nondegeneracy. Thus $|c|=1$ and $d=c\bar a$. Writing $1/c=e^{i\psi}$ gives

$$
\boxed{f(z)=e^{i\psi}\frac{a+z}{1+\bar a z},\qquad |a|\ne1.}
$$

Here $a$ is the normalized coefficient after division by the original $b$. The inequality $|a|\ne1$ is again the [determinant](../../../../../determinant.md) condition. For $|a|<1$ the map preserves the disc; for $|a|>1$ it interchanges its inside and outside. Circle preservation alone does not justify restricting to [automorphisms of the unit disk](../../../../../automorphism-of-the-unit-disk.md).

## ↑ Ancestors (10)

1. [8F](../8f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
