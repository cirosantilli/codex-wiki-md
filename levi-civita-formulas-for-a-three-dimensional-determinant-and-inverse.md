# Levi-Civita formulas for a three-dimensional determinant and inverse

↑ **Parent:** [Contraction of two Levi-Civita symbols](contraction-of-two-levi-civita-symbols.md)

For a $3\times3$ [matrix](matrix.md) $A$, contraction of $\epsilon_{lmn}A_{il}A_{jm}A_{kn}=(\det A)\epsilon_{ijk}$ with $\epsilon_{ijk}$ proves the title identity, because $\epsilon_{ijk}\epsilon_{ijk}=6$. Define

$$
C_{ab}=\frac12\epsilon_{ajk}\epsilon_{bmn}A_{jm}A_{kn}.
$$

Expansion shows that $C$ is the [cofactor matrix](cofactor-matrix.md). Equivalently, the determinant identity gives $A_{ib}C_{ab}=(\det A)\delta_{ia}$. Thus for invertible $A$,

$$
(A^{-1})_{ba}=\frac{C_{ab}}{\det A}=\frac{\epsilon_{ajk}\epsilon_{bmn}A_{jm}A_{kn}}{2\det A}.
$$

Differentiating the cubic determinant formula gives three equal terms, so $\partial(\det A)/\partial A_{ab}=C_{ab}$. This is the entrywise [derivative of the determinant](derivative-of-the-determinant.md) and remains valid for singular $A$ through the cofactor expression. The inverse expression requires $\det A\ne0$.

## ↑ Ancestors (10)

1. [Contraction of two Levi-Civita symbols](contraction-of-two-levi-civita-symbols.md)
2. [Levi-Civita symbol](levi-civita-symbol.md)
3. [Vector calculus](vector-calculus.md)
4. [Multivariable calculus](multivariable-calculus-split.md)
5. [Calculus](calculus-split.md)
6. [Real analysis](real-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/6/solution.md)
