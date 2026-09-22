<h1 id="analysis/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The complex [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) says that for a [holomorphic](../../../../../holomorphic-function-split.md) [antiderivative](../../../../../antiderivative.md) $F$ and a piecewise $C^1$ path $\gamma$ from $a$ to $b$, one has $\int_\gamma F'(z)dz=F(b)-F(a)$. The integral is therefore zero on a closed path; the [antiderivative](../../../../../antiderivative.md) need only be defined on a neighborhood of that path, rather than on all its interior.

The assumptions make $F(z)=z/f(z)^n$ [holomorphic](../../../../../holomorphic-function-split.md) near $\gamma$. Differentiate:

$$
F'(z)=\frac1{f(z)^n}-n\frac{zf'(z)}{f(z)^{n+1}}.
$$

Integrate this [derivative](../../../../../derivative.md) around the closed path to obtain

$$
\boxed{\int_\gamma\frac{dz}{f(z)^n}=n\int_\gamma\frac{zf'(z)}{f(z)^{n+1}}dz.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [Analysis](../../../analysis.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
