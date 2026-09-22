<h1 id="31e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Cole-Hopf transformation](../../../../../../cole-hopf-transformation.md) for the sign convention here is $Q=q_x/q$, with $q\ne0$ and $q_t=q_{xx}$. Indeed $q_t/q=Q_x+Q^2$, so

$$
Q_t=\partial_x(Q_x+Q^2)=Q_{xx}+2QQ_x.
$$

Conversely a solution $Q$ determines a locally nonzero $q$ through $q_x=Qq$, $q_t=(Q_x+Q^2)q$; their compatibility is this Burgers equation. A spatially constant term can be removed by rescaling $q$ in time.

Set $\mu=q\psi$ in the heat-equation pair. Division by $q$ gives

$$
\boxed{\psi_x+(Q-ik)\psi=1,\qquad\psi_t+(Q_x+Q^2+k^2)\psi=Q+ik.}
$$

Their compatibility can be checked without referring back to $q$: writing $A=ik-Q$, $B=-Q_x-Q^2-k^2$, we have $\psi_x=A\psi+1$, $\psi_t=B\psi+Q+ik$. The coefficient of $\psi$ in $\psi_{xt}-\psi_{tx}$ is $-Q_t+Q_{xx}+2QQ_x$, and the constant term is $(ik-Q)(Q+ik)-Q_x-B=0$. Thus this linear auxiliary pair is compatible exactly for the required [viscous Burgers equation](../../../../../../viscous-burgers-equation.md). As in part (a), adjoining a constant component turns it into a homogeneous $2\times2$ [matrix](../../../../../../matrix.md) [Lax pair](../../../../../../lax-pair.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [31E](../../31e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
