<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [vector](../../../../../vector.md) equation, the [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J(x,y)=
\begin{pmatrix}
6x^5&-20y^3\\1&-1
\end{pmatrix}.
$$

Write the updated coordinates as $(X,Y)$. The second equation of the [multivariable Newton iteration](../../../../../multivariable-newton-iteration.md) gives $X-Y=0$. Substituting $X=Y$ into its first linearized equation gives

$$
(6x^5-20y^3)X=5x^6-15y^4-6.
$$

Hence **$h(x,y)=6x^5-20y^3$**, and, whenever $h\ne0$,

$$
\boxed{
(x_{k+1},y_{k+1})
=\frac{5x_k^6-15y_k^4-6}{6x_k^5-20y_k^3}(1,1).
}
$$

Starting from $(0,1)$ gives $(x_1,y_1)=(21/20,21/20)$. Every subsequent iterate remains on the diagonal, where this is exactly the scalar [Newton root-finding iteration](../../../../../newton-root-finding-iteration.md) from (b). The value $f(21/20)>0$, so $21/20<r$.

For $1\le x<r$, concavity again puts the tangent's zero at or above $r$. Also

$$
N'(x)=\frac{f(x)f''(x)}{f'(x)^2}<0,
$$

so $r\le N(21/20)\le N(1)=8/7<6/5$. After one scalar step the sequence therefore enters the invariant [interval](../../../../../interval-mathematics.md) proved in (b). It converges to **$(r,r)$ at least quadratically**. If the [vector](../../../../../vector.md) error is measured in the [Euclidean norm](../../../../../euclidean-norm.md), then $\|(x_k,y_k)-(r,r)\|=\sqrt2\,|x_k-r|$, so the scalar quadratic estimate also gives a quadratic [vector](../../../../../vector.md) estimate. The initial off-diagonal step causes no difficulty because its [Jacobian matrix](../../../../../jacobian-matrix.md) is invertible and lands exactly on the diagonal.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
