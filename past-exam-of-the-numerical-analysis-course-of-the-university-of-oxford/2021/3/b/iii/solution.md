<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With $f(x,y)=-xy^2-y^5$, write $t=x_{n+1}=x_n+h$ and $z=y_{n+1}$. The [Backward Euler method](../../../../../backward-euler-method.md) requires

$$
z=y_n-htz^2-hz^5,
$$

or the monic [quintic polynomial](../../../../../quintic-polynomial.md) equation

$$
p(z)=z^5+tz^2+h^{-1}z-h^{-1}y_n=0.
$$

Construct its $5\times5$ [companion matrix](../../../../../companion-matrix.md)

$$
\boxed{C_n=\begin{pmatrix}
0&0&0&0&y_n/h\\
1&0&0&0&-1/h\\
0&1&0&0&-t\\
0&0&1&0&0\\
0&0&0&1&0
\end{pmatrix}.}
$$

Its [characteristic polynomial](../../../../../characteristic-polynomial.md) is $\det(zI-C_n)=p(z)$. Thus the [polynomial roots](../../../../../root-of-a-polynomial.md) needed for this update are exactly the [eigenvalues](../../../../../eigenvalue.md) of $C_n$.

At each step, assemble $C_n$, compute its [eigenvalues](../../../../../eigenvalue.md), for example with the [QR algorithm](../../../../../qr-algorithm.md), and choose its unique positive real [eigenvalue](../../../../../eigenvalue.md) as $y_{n+1}$. To justify this selection, let

$$
F(z)=hz^5+htz^2+z-y_n.
$$

If $y_n>0$, then $F(0)=-y_n<0$, $F(y_n)=hy_n^5+hty_n^2>0$, and

$$
F'(z)=5hz^4+2htz+1>0\qquad(z\geq0).
$$

The [intermediate value theorem](../../../../../intermediate-value-theorem.md) and strict [monotonicity](../../../../../monotonic-function.md) prove there is exactly one positive [polynomial root](../../../../../root-of-a-polynomial.md), located in $(0,y_n)$. Starting at $y_0=1$ therefore makes every update well defined, positive and decreasing. In numerical arithmetic, select the nearly real [eigenvalue](../../../../../eigenvalue.md) in this interval and check the [polynomial residual](../../../../../polynomial-residual.md) $|F(z)|$; a final [Newton root-finding iteration](../../../../../newton-root-finding-iteration.md) can refine it. This reduces each update to the requested [eigenvalue problem](../../../../../eigenvalue-problem.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
