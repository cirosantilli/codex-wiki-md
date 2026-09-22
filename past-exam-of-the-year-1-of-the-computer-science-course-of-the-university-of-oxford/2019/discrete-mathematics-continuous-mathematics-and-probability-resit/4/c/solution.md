<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $h(x,y)=2y^3+xy^2-y^2-4x$, so $g=e^h>0$. Its [gradient](../../../../../gradient.md) is $\nabla g=g\nabla h$, and

$$
\nabla h=\begin{pmatrix}y^2-4\\2y(3y+x-1)\end{pmatrix}.
$$

Thus a [stationary point](../../../../../stationary-point.md) must have $y=\pm2$ and $x=1-3y$, giving **$(-5,2)$ and $(7,-2)$**. To classify them, use

$$
H_g=g\bigl(H_h+\nabla h\nabla h^T\bigr),\qquad
H_h=\begin{pmatrix}0&2y\\2y&12y+2x-2\end{pmatrix}.
$$

At either [stationary point](../../../../../stationary-point.md), $\nabla h=0$ and $12y+2x-2=6y$. Hence $\det H_g=g^2(-4y^2)=-16g^2<0$. The [Hessian](../../../../../hessian-matrix.md) has one positive and one negative [eigenvalue](../../../../../eigenvalue.md), so **both are [saddle points](../../../../../saddle-point.md)**. There are no other [stationary points](../../../../../stationary-point.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics, and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
