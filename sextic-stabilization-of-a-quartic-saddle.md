# Sextic stabilization of a quartic saddle

↑ **Parent:** [Saddle point of a scalar function](saddle-point-of-a-scalar-function.md)

For every $\kappa>0$, the [polynomial](polynomial-split.md) $H_\kappa$ has exactly five [stationary points](stationary-point.md): the origin and the four points with $x^2=y^2=\kappa/3$. Its [gradient](gradient.md) factors as

$$
\nabla H_\kappa=2\bigl(x(3x^4-\kappa y^2),\ y(3y^4-\kappa x^2)\bigr).
$$

If a coordinate vanishes at a [stationary point](stationary-point.md), both do. Otherwise put $u=x^2$, $v=y^2$ to obtain $u^2=(\kappa/3)v$ and $v^2=(\kappa/3)u$. Dividing gives $u=v$ and then $u=v=\kappa/3$.

At the origin, the [Hessian matrix](hessian-matrix.md) vanishes. Axis restrictions give $H_\kappa(t,0)=t^6>0$, while diagonal restrictions give $H_\kappa(t,\pm t)=2t^6-\kappa t^4<0$ for small nonzero $t$. Thus the origin is a degenerate [saddle point of a scalar function](saddle-point-of-a-scalar-function.md). Its leading quartic term is nonpositive, showing why the sign of the first nonzero homogeneous term alone need not settle the problem when that term vanishes along some directions.

At each nonzero [stationary point](stationary-point.md), the [Hessian matrix](hessian-matrix.md) has diagonal entries $8\kappa^2/3$ and off-diagonal entries $\pm4\kappa^2/3$. Its positive [eigenvalues](eigenvalue.md) $4\kappa^2/3$ and $4\kappa^2$ prove strict [local minima](local-minimum.md). They are also [global minima](global-minimum.md) of value $-\kappa^3/27$: the [arithmetic-geometric mean inequality](arithmetic-geometric-mean-inequality.md) gives $x^6+y^6\geq2|xy|^3$, and the minimum of $2u^3-\kappa u^2$ for $u\geq0$ is $-\kappa^3/27$ at $u=\kappa/3$. Equality requires $|x|=|y|$.

## ↑ Ancestors (6)

1. [Saddle point of a scalar function](saddle-point-of-a-scalar-function.md)
2. [Critical point](critical-point.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
