<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

From $Te_0=e_0\ne0$, one is an [eigenvalue](../../../../../eigenvalue.md). Zero is also an [eigenvalue](../../../../../eigenvalue.md): the nonzero [continuous function](../../../../../continuous-function.md) $q(x)=x(1-x)$ has both endpoint values zero, so $Tq=0$.

For $\lambda\notin\{0,1\}$, the [linear projection](../../../../../projection-linear-algebra.md) identity $T^2=T$ gives an explicit bounded inverse:

$$
(\lambda I-T)^{-1}=\frac1\lambda(I-T)+\frac1{\lambda-1}T.
$$

Multiplying on either side by $\lambda I-T$ yields $(I-T)+T=I$. There are no other points in the [spectrum](../../../../../spectrum-functional-analysis.md), and thus the [spectrum of a nontrivial bounded projection](../../../../../spectrum-of-a-nontrivial-bounded-projection.md) here is

$$
\boxed{\sigma(T)=\{0,1\},\qquad r(T)=1.}
$$

Let $M=\|T\|$, as calculated in part (ii). Its endpoint values ensure $1\leq M<\infty$. Since $T^j=T$ for all $j\geq1$,

$$
\|T^j\|^{1/j}=M^{1/j}\longrightarrow1,
\qquad\inf_{j\geq1}\|T^j\|^{1/j}=1.
$$

This verifies the [spectral radius formula](../../../../../spectral-radius-formula.md) explicitly:

$$
\boxed{r(T)=\inf_{j\geq1}\|T^j\|^{1/j}=\lim_{j\to\infty}\|T^j\|^{1/j}=1.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis I course of the University of Oxford](../../../../split.md)
6. [Functional analysis I course of the University of Oxford](../../../../../functional-analysis-i-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
