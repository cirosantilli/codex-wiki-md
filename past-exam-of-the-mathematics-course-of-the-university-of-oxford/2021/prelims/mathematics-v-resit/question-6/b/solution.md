<h1 id="question-6/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

Set $u=X(x)Y(y)$ in [Laplace's equation](../../../../../../laplace-equation.md). [Separation of variables](../../../../../../separation-of-variables.md) gives

$$
X''+\lambda X=0,\qquad Y''-\lambda Y=0,\qquad X'(0)=X'(\pi)=0.
$$

The [Sturm-Liouville problem](../../../../../../sturm-liouville-problem.md) in $x$ has the constant mode $X_0=1$ with $\lambda_0=0$, and the [eigenfunctions](../../../../../../eigenfunction.md) $X_n=\cos(nx)$ with $\lambda_n=n^2$, $n\geq1$. Indeed, [integration by parts](../../../../../../integration-by-parts.md) makes $\lambda$ nonnegative; for $\lambda>0$ the first [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) removes the [sine](../../../../../../sine.md) term and the second requires $\sqrt\lambda$ to be an [integer](../../../../../../integer-split.md). For $\lambda=0$, both derivative conditions make $X$ constant.

Expand the top data using a [Fourier cosine series](../../../../../../fourier-cosine-series.md):

$$
g(x)=\pi^2-x^2=\frac{g_0}{2}+\sum_{n=1}^{\infty}g_n\cos(nx).
$$

The constant coefficient is

$$
g_0=\frac2\pi\int_0^\pi(\pi^2-x^2)\,dx=\frac{4\pi^2}{3}.
$$

For $n\geq1$, the constant part has zero [integral](../../../../../../integral-split.md) against $\cos(nx)$, and two [integrations by parts](../../../../../../integration-by-parts.md) give

$$
\begin{aligned}
g_n&=-\frac2\pi\int_0^\pi x^2\cos(nx)\,dx\\
&=-\frac2\pi\left[
\frac{x^2\sin(nx)}n+\frac{2x\cos(nx)}{n^2}-\frac{2\sin(nx)}{n^3}
\right]_0^\pi
=\frac{4(-1)^{n+1}}{n^2}.
\end{aligned}
$$

Since the bottom value is zero, a convenient factor depending on $y$ for the nonconstant modes is $\sinh(n(y+1))$, which vanishes at $y=-1$. Its value at $y=1$ is $\sinh(2n)$. The zero mode is linear in $y$, so matching both constant boundary values gives

$$
\boxed{u(x,y)=\frac{\pi^2}{3}(y+1)
+\sum_{n=1}^{\infty}\frac{4(-1)^{n+1}}{n^2}
\frac{\sinh(n(y+1))}{\sinh(2n)}\cos(nx)}.
$$

To obtain exactly the paper's form, use the [hyperbolic-function identity](../../../../../../hyperbolic-function-identity.md)

$$
\frac{\sinh(n(y+1))}{\sinh(2n)}
=\frac{\sinh(ny)\cosh n+\cosh(ny)\sinh n}{2\sinh n\cosh n}
=\frac{\sinh(ny)+\tanh n\cosh(ny)}{2\sinh n}.
$$

Thus

$$
\boxed{u(x,y)=\frac{\pi^2}{3}(1+y)
+\sum_{n=1}^{\infty}\frac{2(-1)^{n+1}}{n^2\sinh n}
\bigl(\sinh(ny)+\tanh(n)\cosh(ny)\bigr)\cos(nx)}.
$$

Each product of [hyperbolic sine](../../../../../../hyperbolic-sine.md) or [hyperbolic cosine](../../../../../../hyperbolic-cosine.md) with $\cos(nx)$ has $u_{xx}+u_{yy}=0$. The zero mode is also a [harmonic function](../../../../../../harmonic-function.md). On $-1\leq y\leq1$, the factor $\sinh(n(y+1))/\sinh(2n)$ lies between zero and one. Since $\sum n^{-2}$ converges, the [Weierstrass M-test](../../../../../../weierstrass-m-test.md) gives [uniform convergence](../../../../../../uniform-convergence.md) on the closed rectangle. The series therefore gives zero at the bottom and the continuous [Fourier cosine series](../../../../../../fourier-cosine-series.md) of $\pi^2-x^2$ at the top, including its endpoints. On compact subsets with $y<1$, the factors decay exponentially with $n$, justifying termwise [partial derivatives](../../../../../../partial-derivative.md). In particular $u_x=0$ on both open vertical edges because every differentiated [cosine](../../../../../../cosine.md) factor vanishes there. The solution has finite [Dirichlet energy](../../../../../../dirichlet-energy.md): [Fourier orthogonality](../../../../../../fourier-orthogonality.md) gives the $n$th nonconstant mode's energy as $(\pi/2)ng_n^2\coth(2n)=O(n^{-3})$, whose sum is finite. Here $\coth$ is the [hyperbolic cotangent](../../../../../../hyperbolic-cotangent.md). Thus [a](../a.md) proves uniqueness in that class.

There is a [corner compatibility condition for mixed boundary data](../../../../../../corner-compatibility-condition-for-mixed-boundary-data.md) in the printed wording. The top data have $g'(\pi)=-2\pi$, but the paper writes $u_x(\pi,y)=0$ even at $y=1$. **The series solves the interior equation and all the open-edge boundary conditions; the literal derivative condition at $(\pi,1)$ is incompatible with the top data.** A function differentiable in $x$ along the top edge would necessarily have $u_x(\pi,1)=g'(\pi)=-2\pi$. Hence it cannot simultaneously satisfy the printed zero derivative at that corner, and there is no solution with all those literal corner requirements. The standard interpretation of this [mixed boundary condition](../../../../../../mixed-boundary-condition.md) imposes the [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) on the open sides and the [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) continuously on the horizontal edges. Differentiating the series term by term on the top edge would be invalid at this corner; the uniform convergence of the undifferentiated series does not license that operation.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [Question 6](../../question-6.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
