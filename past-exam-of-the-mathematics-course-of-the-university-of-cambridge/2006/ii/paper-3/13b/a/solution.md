<h1 id="13b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A homogeneous [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) has $v_0=u_0^2$. Besides $u_0=0$, a nonzero [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) satisfies $r=u_0^2-u_0$, giving $u_\pm=(1\pm\sqrt{1+4r})/2$. Concentrations are nonnegative, so only nonnegative roots are physically admissible. At a positive [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md), the reaction [Jacobian matrix](../../../../../../jacobian-matrix.md) is

$$
J=\begin{pmatrix}u_0&-u_0\\2su_0&-s\end{pmatrix},\qquad \operatorname{tr}J=u_0-s,\qquad\det J=su_0(2u_0-1).
$$

Negative [trace](../../../../../../matrix-trace.md) and positive [determinant](../../../../../../determinant.md) are equivalent to

$$
\boxed{\tfrac12<u_0<s.}
$$

Thus a positive homogeneous stable branch exists precisely when $s>1/2$ and $-1/4<r<s^2-s$, on the upper root $u_+$. The lower positive branch has negative [determinant](../../../../../../determinant.md) and is unstable. At $r=-1/4$ the branches meet and have a zero [eigenvalue](../../../../../../eigenvalue.md); at $u_0=s$ the strict linear stability condition also fails.

The trivial [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) $(0,0)$ has [eigenvalues](../../../../../../eigenvalue.md) $r,-s$, so it is asymptotically stable for $r<0$. It exists for all $r$, independently of the nonzero branches. If negative $u_0$ were allowed mathematically, the negative branch for $r>0$ would also be homogeneously stable, but it does not represent a chemical concentration.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13B](../../13b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
