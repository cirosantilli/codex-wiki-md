<h1 id="stationary-points-are-fixed-points-of-newton-s-method">Stationary points are fixed points of Newton's method</h1>

↑ **Parent:** [Newton's method in optimization](newton-s-method-in-optimization.md)

For a twice continuously differentiable real [function](function-split.md), define the [Newton map in optimization](newton-map-in-optimization.md) $N(p)=p-H(p)^{-1}\nabla f(p)$ wherever its [Hessian matrix](hessian-matrix.md) $H$ is invertible. Every [stationary point](stationary-point.md) in this domain is a [fixed point](fixed-point.md), because its [gradient](gradient.md) is zero. This includes a [local maximum](local-maximum.md) and a [saddle point of a scalar function](saddle-point-of-a-scalar-function.md), as well as a [local minimum](local-minimum.md). Thus [Newton's method in optimization](newton-s-method-in-optimization.md) needs a separate [minimum](minimum-of-a-subset-of-a-total-order.md) classification or a method for ensuring descent when it is used for [minimization problem](minimization-problem.md).

For example, $f(x,y)=(x+y^2)^2+(x^2+y)^2$ has a [stationary point](stationary-point.md) at $(-1/2,-1/2)$, with [Hessian matrix](hessian-matrix.md)

$$
H=\begin{pmatrix}3&-4\\-4&3\end{pmatrix}.
$$

Its [eigenvalues](eigenvalue.md) are $-1$ and $7$, so it is a [saddle point of a scalar function](saddle-point-of-a-scalar-function.md), but starting [Newton's method in optimization](newton-s-method-in-optimization.md) there gives a constant sequence. Its value is $1/8$, whereas the [global minimum](global-minimum.md) zero is attained at $(0,0)$ and $(-1,-1)$.

## ↑ Ancestors (5)

1. [Newton's method in optimization](newton-s-method-in-optimization.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-iv-resit/7/b/ii/solution.md)
