<h1 id="9/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At a fixed point the first equation gives $\alpha S_*I_*=B$. The second gives $I_* =\alpha S_*I_*$, so $I_*=B>0$ and

$$
\boxed{(S_*,I_*)=(1/\alpha,B).}
$$

There is no disease-free fixed point: with $I=0$, susceptibles still increase by $B$ each step.

Set $r=\alpha B>0$. The [Jacobian matrix](../../../../../jacobian-matrix.md) of the update at the fixed point is

$$
M=\begin{pmatrix}1-r&-1\\r&1\end{pmatrix},\qquad
\det M=1,\quad\operatorname{tr}M=2-r.
$$

Its characteristic equation and multipliers are

$$
\lambda^2-(2-r)\lambda+1=0,\qquad
\lambda_\pm=1-\frac r2\pm\frac12\sqrt{r(r-4)}.
$$

For $0<r<4$, these are distinct complex conjugates with product one, so both have modulus one. The linearized iterates are bounded and oscillatory: **neutral linear stability holds for $0<\alpha B<4$**, with no linear asymptotic attraction.

At $r=4$, the repeated multiplier is $-1$, but $M\ne-I$. Writing $M=-I+N$ gives $N\ne0$, $N^2=0$ and $M^n=(-1)^n(I-nN)$, so generic linearized perturbations grow linearly. For $r>4$, a real multiplier has modulus greater than one. Thus **the equilibrium is linearly unstable for $\alpha B\geq4$**.

For the unit-modulus range, the nonlinear behavior is not determined by this calculation: [unit-modulus multipliers do not determine nonlinear stability](../../../../../unit-modulus-multipliers-do-not-determine-nonlinear-stability.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
