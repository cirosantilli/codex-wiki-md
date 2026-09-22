<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First suppose the stated nonnegative [vectors](../../../../../vector.md) $y,z$ exist. If $x\in P\cap Q$, multiply $Ax\leq b$ by $y^T$ and $Cx\leq d$ by $z^T$. Since $x\geq0$ and $y^TA+z^TC\geq0$, this gives the contradiction

$$
0\leq(y^TA+z^TC)x\leq y^Tb+z^Td<0.
$$

Thus the certificate implies $P\cap Q=\varnothing$.

For the converse, put

$$
M=\begin{pmatrix}A\\C\end{pmatrix},\qquad h=\begin{pmatrix}b\\d\end{pmatrix}.
$$

A common [feasible point](../../../../../feasible-point.md) exists exactly when $Mx\leq h$, $x\geq0$. Introducing a nonnegative [vector](../../../../../vector.md) of [slack variables](../../../../../slack-variable.md) $s$ makes this equivalent to

$$
\begin{pmatrix}M&I\end{pmatrix}\begin{pmatrix}x\\s\end{pmatrix}=h,\qquad x,s\geq0.
$$

If this system is infeasible, the nonnegative-equations version of [Farkas' lemma](../../../../../farkas-lemma.md) supplies an unrestricted [vector](../../../../../vector.md) $u$ such that

$$
M^Tu\geq0,\qquad I^Tu=u\geq0,\qquad h^Tu<0.
$$

Split $u=(y,z)^T$ according to the original two blocks of inequalities. The three conditions become **$y,z\geq0$, $y^TA+z^TC\geq0$ and $y^Tb+z^Td<0$**, exactly the desired certificate. Both directions are proved. The role of $x\geq0$ is essential: it is why the combined normal need only be nonnegative rather than zero.[§5.8.3, printed pp. 261–262, linear-inequality alternatives and Farkas' lemma](../../../../../convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
