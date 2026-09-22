<h1 id="f/f1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each fixed $(x,y)$, the function $z\mapsto z^3+z+xy-1$ is continuous, strictly increasing because its derivative is $3z^2+1>0$, and tends to opposite infinities at the two ends of the real line. The intermediate value theorem therefore gives exactly one zero.

For $F(x,y,z)=z^3+z+xy-1$, its partial derivative $F_z=3z^2+1$ never vanishes. The [implicit function theorem](../../../../../implicit-function-theorem.md) gives a local $C^1$ solution near every point of the solution set. Uniqueness makes these local solutions agree, producing a global $g\in C^1(\mathbb R^2)$. Implicit differentiation gives

$$
Dg(x,y)=\frac{-1}{3g(x,y)^2+1}\begin{pmatrix}y&x\end{pmatrix}.
$$

At $(1,1)$ the [root](../../../../../root-of-a-root-system.md) is $g(1,1)=0$, so

$$
\boxed{Dg(1,1)=\begin{pmatrix}-1&-1\end{pmatrix}.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [F1](../../f1.md)
3. [F](../../../f.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
