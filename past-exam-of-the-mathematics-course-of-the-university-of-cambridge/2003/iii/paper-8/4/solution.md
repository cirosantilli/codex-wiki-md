<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Painlevé property](../../../../../painleve-property.md) says that the general solution has no movable critical singularities: [analytic continuation](../../../../../analytic-continuation.md) around a singularity whose location depends on the initial data must not create a different branch. A [fixed singularity of a complex differential equation](../../../../../fixed-singularity-of-a-complex-differential-equation.md) has its location prescribed by the coefficients; a [movable singularity of a complex differential equation](../../../../../movable-singularity-of-a-complex-differential-equation.md) has a location which varies with the initial data. A commonly used stronger form requires movable singularities to be [poles](../../../../../pole.md), so that the solution is locally a [meromorphic function](../../../../../meromorphic-function.md) there. Movable [branch points](../../../../../branch-point.md) are excluded; a movable [pole](../../../../../pole.md) is permitted. We will prove the stronger form for this equation by finding its complete general solution family as [rational functions](../../../../../rational-function.md).

Use the [linearization of a Riccati equation](../../../../../linearization-of-a-riccati-equation.md). If $w'=aw^2+bw+c$, put $w=-v'/(av)$ wherever $a,v\ne0$. Differentiating this expression and cancelling the quadratic terms yields

$$
v''-\left(\frac{a'}a+b\right)v'+acv=0.
$$

Conversely a nonzero solution $v$ of this [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md) gives a solution $w$, wherever the quotient is defined. Every local finite solution $w$ at an [ordinary point](../../../../../ordinary-point-criterion-for-a-second-order-equation.md) arises this way: solve $v'=-awv$ with a nonzero initial value and differentiate to get the second-order equation. Multiplying $v$ by a nonzero constant leaves $w$ unchanged, giving the one effective [constant of integration](../../../../../constant-of-integration.md) expected for a first-order [Riccati equation](../../../../../riccati-equation.md).

For the present coefficients, $a'/a=1/z+1/(z+1)$, so the [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md) simplifies to

$$
z(z+1)v''+(z-1)v'-v=0.
$$

Two direct substitutions give solutions $v_1=z-1$ and $v_2=1/(z+1)$. Their [Wronskian](../../../../../wronskian.md) is

$$
v_1v_2'-v_1'v_2=-\frac{2z}{(z+1)^2},
$$

which is nonzero at every [ordinary point](../../../../../ordinary-point-criterion-for-a-second-order-equation.md) $z\notin\{0,-1\}$. They therefore form a fundamental pair there, and all local solutions have the form

$$
v=C_1(z-1)+\frac{C_2}{z+1}
=\frac{C_1z^2+C_2-C_1}{z+1},\qquad (C_1,C_2)\ne(0,0).
$$

Taking its [logarithmic derivative](../../../../../logarithmic-derivative.md) gives

$$
w=\frac{1}{z(z+1)^2}-\frac{2C_1}{(z+1)(C_1z^2+C_2-C_1)}.
$$

Thus, for $C_1\ne0$, writing $k=(C_2-C_1)/C_1$, the general family is

$$
\boxed{w(z)=\frac{1}{z(z+1)^2}-\frac{2}{(z+1)(z^2+k)},\qquad k\in\mathbb C.}
$$

The remaining member, corresponding to $C_1=0$, is

$$
\boxed{w(z)=\frac{1}{z(z+1)^2}.}
$$

The completeness of the linearizing pair proves that no other local solution is omitted. These are [rational functions](../../../../../rational-function.md), single-valued [meromorphic functions](../../../../../meromorphic-function.md); hence their continuation has no [branch points](../../../../../branch-point.md). Their only possible moving singularities are zeros of $z^2+k$. A root $z_0$ outside $\{0,-1\}$ is simple, and its [residue](../../../../../residue.md) is

$$
\operatorname*{Res}_{z=z_0}w=-\frac{1}{z_0(z_0+1)}.
$$

Equivalently, [poles of a Riccati solution from zeros of its linearizing solution](../../../../../poles-of-a-riccati-solution-from-zeros-of-its-linearizing-solution.md) are simple at [ordinary points](../../../../../ordinary-point-criterion-for-a-second-order-equation.md), because a nontrivial solution of a [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md) cannot have both $v(z_0)=0$ and $v'(z_0)=0$. The exceptional collisions $k=0$ or $k=-1$ occur at the fixed coefficient singularities, and still give [rational functions](../../../../../rational-function.md). Consequently every movable singularity is a [pole](../../../../../pole.md), establishing the [Painlevé property](../../../../../painleve-property.md) in its stronger meromorphic sense.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
