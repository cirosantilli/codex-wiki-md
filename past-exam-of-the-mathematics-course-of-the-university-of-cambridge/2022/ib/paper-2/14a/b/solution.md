<h1 id="14a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The solution $x+\lambda$ satisfies the left [boundary condition](../../../../../../boundary-condition.md), while $e^{-x}$ satisfies decay at infinity. The proposed expression for $x<\xi$ is therefore the correct left homogeneous solution. For $x>\xi$, write $G=Ce^{-x}$. Continuity at $x=\xi$ gives

$$
Ce^{-\xi}=-\frac{\xi+\lambda}{\xi+\lambda+1}.
$$

Hence the [Green function](../../../../../../green-s-function.md) is

$$
\boxed{
G(x;\xi)=
\begin{cases}
-\dfrac{x+\lambda}{\xi+\lambda+1},&0\leq x<\xi,\\[6pt]
-\dfrac{\xi+\lambda}{\xi+\lambda+1}e^{\xi-x},&x>\xi.
\end{cases}}
$$

Indeed, its derivative has the required unit jump,

$$
G_x(\xi^+;\xi)-G_x(\xi^-;\xi)=1,
$$

which produces the [Dirac delta distribution](../../../../../../dirac-delta-function.md) in $L[G]$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14A](../../14a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
