<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a rectangular diagonal matrix $D$, define $D^+\in\mathbb R^{n\times m}$ by transposing its shape and taking

$$
\boxed{(D^+)_{ii}=\begin{cases}D_{ii}^{-1},&D_{ii}\ne0,\\0,&D_{ii}=0,\end{cases}\qquad(D^+)_{ij}=0\ (i\ne j).}
$$

Entry by entry, $DD^+D=D$ and $D^+DD^+=D^+$. For $A=U\Sigma V^T$, orthogonality therefore gives

$$
\boxed{A^+=V\Sigma^+U^T,}
$$

since $AA^+A=U\Sigma\Sigma^+\Sigma V^T=A$, and similarly $A^+AA^+=A^+$. This candidate is the [Moore-Penrose inverse](../../../../../moore-penrose-inverse.md). It also makes $AA^+$ and $A^+A$ symmetric, although those two extra conditions are not required by the question's stated definition. The two displayed conditions alone need not specify a unique generalized inverse.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
