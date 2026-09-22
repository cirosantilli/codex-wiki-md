<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The only nonconstant entry of the [metric tensor](../../../../metric-tensor.md) is $g_{\phi\phi}=R^2\sin^2\theta$, whose [partial derivative](../../../../partial-derivative.md) is $\partial_\theta g_{\phi\phi}=2R^2\sin\theta\cos\theta$. The nonzero [Christoffel symbols](../../../../christoffel-symbol.md) are

$$
\boxed{\Gamma^\theta_{\phi\phi}=-\sin\theta\cos\theta,\qquad
\Gamma^\phi_{\theta\phi}=\Gamma^\phi_{\phi\theta}=\cot\theta.}
$$

Along a fixed latitude with $0<\theta<\pi$, [parallel transport](../../../../parallel-transport.md) gives

$$
\frac{dV^\theta}{d\phi}=\sin\theta\cos\theta\,V^\phi,
\qquad
\frac{dV^\phi}{d\phi}=-\cot\theta\,V^\theta.
$$

Set $X=V^\theta$ and $Y=\sin\theta\,V^\phi$. Since $\theta$ is fixed, this [linear ordinary differential equation](../../../../linear-ordinary-differential-equation-split.md) becomes

$$
X'=\cos\theta\,Y,\qquad Y'=-\cos\theta\,X.
$$

It is a rotation at constant rate $-\cos\theta$. Its general solution, also valid at the equator where the rate is zero, is

$$
\boxed{\begin{aligned}
V^\theta&=A\cos(\phi\cos\theta)+B\sin(\phi\cos\theta),\\
V^\phi&=\frac{-A\sin(\phi\cos\theta)+B\cos(\phi\cos\theta)}{\sin\theta}.
\end{aligned}}
$$

The initial data give $A=1$ and $B=0$. At $\theta=\pi/3$, a complete circuit has $\phi\cos\theta=\pi$, so

$$
\boxed{(V^\theta,V^\phi)_{\phi=2\pi}=(-1,0).}
$$

The physical squared length uses the [metric tensor](../../../../metric-tensor.md), rather than the Euclidean sum of coordinate components:

$$
\boxed{|\mathbf V|^2=R^2\bigl[(V^\theta)^2+\sin^2\theta(V^\phi)^2\bigr]
=R^2(A^2+B^2).}
$$

It is constant and equals $R^2$ for these data. More generally, [metric compatibility](../../../../metric-compatibility.md) gives $d\,g(V,V)/d\phi=(\nabla_{\partial_\phi}g)(V,V)+2g(\nabla_{\partial_\phi}V,V)=0$. The final change of direction is [holonomy](../../../../holonomy.md), exemplified by [parallel transport around a latitude of the unit sphere](../../../../parallel-transport-around-a-latitude-of-the-unit-sphere.md); [parallel transport](../../../../parallel-transport.md) preserves length without requiring the direction to return unchanged.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
