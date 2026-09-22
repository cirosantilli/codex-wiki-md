<h1 id="p/p1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $p_1(x)=a+bx$. It suffices to impose orthogonality of the error to the basis $1,x$ of $\Pi_1$. With the printed weight $x^{-1/2}$ and $f=x^{3/2}$, the [normal equations](../../../../../normal-equation.md) are

$$
\begin{pmatrix}2&2/3\\2/3&2/5\end{pmatrix}
\begin{pmatrix}a\\b\end{pmatrix}
=\begin{pmatrix}1/2\\1/3\end{pmatrix}.
$$

Here, for example, $\langle f,1\rangle=\int_0^1x\,dx=1/2$ and $\langle f,x\rangle=\int_0^1x^2\,dx=1/3$. Solving gives $a=-1/16$, $b=15/16$. Therefore

$$
\boxed{p_1(x)=\frac{15x-1}{16}.}
$$

The two [normal equations](../../../../../normal-equation.md) make the error [orthogonal](../../../../../orthogonal-vectors.md) to every linear polynomial, and part (b) then proves optimality, rather than merely furnishing a candidate fit.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [P1](../../p1.md)
3. [P](../../../p.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
