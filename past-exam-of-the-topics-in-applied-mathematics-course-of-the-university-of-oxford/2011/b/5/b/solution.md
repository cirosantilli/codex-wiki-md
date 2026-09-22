<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There is always the [fixed point](../../../../../fixed-point.md) $(0,0)$. For $P>0$, the first fixed-point equation gives $e^{-P}=1/r$, and the second gives $P=N(1-1/r)$. Thus for $r>1$ there is exactly one positive [fixed point](../../../../../fixed-point.md),

$$
\boxed{P_* =\log r,\qquad N_* =\frac{r\log r}{r-1}.}
$$

For $r=1$, every point $(N,0)$, $N\geq0$, is fixed. There are no other nonnegative [fixed points](../../../../../fixed-point.md).

At the origin the [Jacobian matrix](../../../../../jacobian-matrix.md) has [eigenvalues](../../../../../eigenvalue.md) $r,0$. It is asymptotically stable for $0<r<1$ and a saddle for $r>1$. For $r<1$, the bounds $N_{t+1}\leq rN_t$ and $P_{t+1}\leq N_t$ also prove global extinction in the nonnegative quadrant.

At the positive [fixed point](../../../../../fixed-point.md),

$$
J_* =\begin{pmatrix}1&-N_*\\(r-1)/r&N_*/r\end{pmatrix},\qquad\operatorname{tr}J_* =1+\frac{\log r}{r-1}<2,\qquad\det J_* =N_*>1.
$$

Here $\log r<r-1$ and $\log r>1-1/r$ for $r>1$. The discriminant is negative because the positive trace is less than two and [determinant](../../../../../determinant.md) exceeds one. The conjugate multipliers have modulus $\sqrt{N_*}>1$, so **the positive [fixed point](../../../../../fixed-point.md) is always unstable**. This is the [instability of the Nicholson-Bailey equilibrium](../../../../../instability-of-the-nicholson-bailey-equilibrium.md).

For completeness, on the $r=1$ fixed line,

$$
J(N,0)=\begin{pmatrix}1&-N\\0&N\end{pmatrix}.
$$

For $0\leq N<1$, linear perturbations are bounded but have a neutral component along the fixed line; there is no asymptotic stability of an individual point. For $N>1$ there is transverse instability. At $N=1$, the repeated unit [eigenvalue](../../../../../eigenvalue.md) has a nontrivial [Jordan block](../../../../../jordan-block.md), so powers have an unbounded off-diagonal entry and the linearized system is unstable. This degenerate case is not covered by a distinct-[eigenvalue](../../../../../eigenvalue.md) assumption.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
