<h1 id="39a/solution">Solution</h1>

↑ **Parent:** [39A](../39a.md)

Take the boundary-fitted grid $h=1/(M+1)$ and assume the standard [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) hypothesis $u\in C^4(\overline\Omega)$ with bounded fourth partial [derivatives](../../../../../derivative.md). [Taylor expansion](../../../../../taylor-expansion.md) along each coordinate, including a bounded fourth-order remainder, gives the [five-point Laplacian](../../../../../five-point-laplacian.md) [truncation error](../../../../../truncation-error.md)

$$
\tau_{ij}:=\Delta_hu(ih,jh)-f(ih,jh),\qquad |\tau_{ij}|\le C_0h^2.
$$

The numerical equation and exact grid values therefore imply $A_h\mathbf e=\boldsymbol\tau$, where $A_h=-\Delta_h$ with zero boundary values. Its [discrete sine transform](../../../../../discrete-sine-transform.md) [eigenvectors](../../../../../eigenvector.md) are $\sin(\pi rih)\sin(\pi sjh)$, $1\le r,s\le M$, and its [eigenvalues](../../../../../eigenvalue.md) are

$$
\lambda_{rs}=\frac4{h^2}\left[\sin^2\frac{\pi rh}2+\sin^2\frac{\pi sh}2\right].
$$

The one-dimensional sine vectors form an [orthogonal basis](../../../../../orthogonal-basis.md), hence so do their [tensor products](../../../../../tensor-product.md). The least [eigenvalue](../../../../../eigenvalue.md) occurs at $r=s=1$. Since $\sin(\pi h/2)\ge h$ for $0<h\le1$, $\lambda_{11}\ge8$, so the Euclidean [operator norm](../../../../../operator-norm.md) of $A_h^{-1}$ is at most $1/8$. There are $M^2$ residual components, and $Mh<1$, giving

$$
\boxed{\|\mathbf e\|_2\le\tfrac18\|\boldsymbol\tau\|_2
\le\tfrac18 C_0h^2M\le\tfrac18 C_0h.}
$$

The factor $M$ matters: pointwise second-order [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) becomes first order in the unweighted Euclidean grid norm.

The PDF does not explicitly impose regularity on the exact solution. Without such a hypothesis its unrestricted error claim is false. Here is a counterexample, with a classical solution smooth in the open square and continuous with zero boundary values:

$$
u(x,y)=g(x)\sin(\pi y),\qquad g(x)=\sqrt x(1-x),\qquad f=\Delta u.
$$

The sampled numerical solution separates as $v_i\sin(\pi jh)$. Its error $e_i=v_i-g(ih)$ solves $A e=\tau$, where $A=-\Delta_{h,x}+\lambda_y I$ and $\lambda_y=4h^{-2}\sin^2(\pi h/2)$. The one-dimensional residual is $\tau_i=\Delta_{h,x}g(ih)-g''(ih)+(\pi^2-\lambda_y)g(ih)$. At the first node,

$$
\tau_1=(\sqrt2-7/4)h^{-3/2}-(2\sqrt2-11/4)h^{-1/2}+O(h^2).
$$

The leading coefficient is strictly negative. Moreover $g''''<0$ on $(0,1)$, so the triangular-average formula for the second difference and [concavity](../../../../../concave-function.md) of $g''$ give $\Delta_{h,x}g\le g''$. Thus the positive part of every residual is at most $Ch^2$. The matrix $A$ has a nonnegative inverse, and its first diagonal inverse entry is at least $1/(2h^{-2}+\lambda_y)$, as follows from the nonnegative Neumann expansion of its tridiagonal matrix. The discrete comparison principle bounds the inverse image of the residual's positive part by $Ch^2$, while the negative first residual gives $e_1\le-c\sqrt h+Ch^2$. Hence $|e_1|\ge c'\sqrt h$ for small $h$. Since $\sum_{j=1}^M\sin^2(\pi jh)=1/(2h)$, the full Euclidean error is bounded below by a positive constant. It cannot be $O(h)$. Thus **the boxed estimate holds for the intended smooth solution class; a regularity condition is genuinely necessary**.

## ↑ Ancestors (10)

1. [39A](../39a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
