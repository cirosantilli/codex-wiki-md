<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Translate the [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) to the origin by $z=(x-a,y-b)^T$. If the [vector field](../../../../../vector-field.md) is continuously differentiable, its first-order [Taylor expansion](../../../../../taylor-expansion.md) is

$$
\dot z=Mz+r(z),\qquad\frac{\|r(z)\|}{\|z\|}\longrightarrow0.
$$

The [Jacobian matrix](../../../../../jacobian-matrix.md) $M$ gives the [linearization](../../../../../linearization.md) $\dot z=Mz$, whose general solution is $z(t)=e^{tM}z(0)$ using the [matrix exponential](../../../../../matrix-exponential.md). Its [eigenvalues](../../../../../eigenvalue.md) determine the exponential factors, while its [eigenvectors](../../../../../eigenvector.md) and, when necessary, [generalized eigenvectors](../../../../../generalized-eigenvector.md) determine their directions.

For distinct [eigenvalues](../../../../../eigenvalue.md) $\lambda_1,\lambda_2$ and corresponding [eigenvectors](../../../../../eigenvector.md) $v_1,v_2$,

$$
\boxed{z(t)=c_1e^{\lambda_1t}v_1+c_2e^{\lambda_2t}v_2.}
$$

For a real [matrix](../../../../../matrix.md) with nonreal conjugate [eigenvalues](../../../../../eigenvalue.md), choose conjugate coefficients to obtain real solutions. Equivalently, if $\lambda=a+ib$ and $v=p+iq$, a real pair of independent solutions is

$$
e^{at}(p\cos bt-q\sin bt),\qquad e^{at}(p\sin bt+q\cos bt).
$$

For a repeated [eigenvalue](../../../../../eigenvalue.md) $\lambda$, there are two cases:

- If two independent [eigenvectors](../../../../../eigenvector.md) exist, $M=\lambda I$ and $\boxed{z(t)=e^{\lambda t}(c_1v_1+c_2v_2)}$.
- Otherwise choose a [Jordan chain](../../../../../jordan-chain.md) $(M-\lambda I)v=0$, $(M-\lambda I)w=v$. Then $\boxed{z(t)=e^{\lambda t}\bigl[c_1v+c_2(w+tv)\bigr]}$.

The factor $t$ in the second case is essential. These are exact solutions of the [linearization](../../../../../linearization.md); the remainder describes the error for the nonlinear [differential equation](../../../../../differential-equation-split.md). When no [eigenvalue](../../../../../eigenvalue.md) has zero real part, the [hyperbolic equilibrium](../../../../../hyperbolic-equilibrium-point.md) theory justifies the corresponding local qualitative classification. Zero real parts require additional nonlinear analysis.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
