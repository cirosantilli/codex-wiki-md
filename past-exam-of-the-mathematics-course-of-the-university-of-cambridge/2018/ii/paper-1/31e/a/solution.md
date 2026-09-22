<h1 id="31e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The stationary equations are

$$
2x(y-a)=0,
\qquad x^2+y^2=1.
$$

Thus

$$
P_+=(0,1),
\qquad P_-=(0,-1),
$$

always exist, and for $|a|\leq1$ there are also

$$
Q_\pm=(\pm\sqrt{1-a^2},a).
$$

The [Jacobian matrix](../../../../../../jacobian-matrix.md) is

$$
J(x,y)=\begin{pmatrix}2(y-a)&2x\\-2x&-2y\end{pmatrix}.
$$

At $P_+$ its eigenvalues are $2(1-a),-2$, so it is a saddle for $a<1$, a stable node for $a>1$, and nonhyperbolic at $a=1$. At $P_-$ they are $-2(1+a),2$, so it is a saddle for $a>-1$, an unstable node for $a<-1$, and nonhyperbolic at $a=-1$.

At $Q_\pm$, for $|a|<1$, the characteristic polynomial is

$$
\lambda^2+2a\lambda+4(1-a^2).
$$

The equilibria are stable for $a>0$ and unstable for $a<0$; they are foci when $|a|<2/\sqrt5$ and nodes when $2/\sqrt5<|a|<1$, with a repeated-eigenvalue transition at equality. For $a=0$ the eigenvalues are purely imaginary. In that case the system is Hamiltonian with [first integral](../../../../../../first-integral.md)

$$
H(x,y)=xy^2+\frac{x^3}{3}-x,
$$

because $\dot x=H_y$ and $\dot y=-H_x$. The Hessian of $H$ is positive definite at $(1,0)$ and negative definite at $(-1,0)$, so nearby regular level sets are closed curves. Hence both nonhyperbolic equilibria are genuine nonlinear centers.

Finally,

$$
\nabla\mathbin\cdot(\dot x,\dot y)
=2(y-a)-2y=-2a.
$$

For $a\ne0$ this has a strict constant sign throughout the simply connected plane, so the [Bendixson-Dulac criterion](../../../../../../bendixson-dulac-theorem.md) proves that **there are no periodic orbits**. These results comprise the [phase portrait of x dot equals two x times y minus a](../../../../../../phase-portrait-of-x-dot-equals-two-x-times-y-minus-a.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31E](../../31e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
