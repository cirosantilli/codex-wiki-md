<h1 id="question-6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [separation of variables](../../../../../../separation-of-variables.md), set $u=X(x)Y(y)$, with $X''/X=-Y''/Y=-\lambda$. The side [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md) give $X'(0)=X'(\pi)=0$. As in the standard [Sturm-Liouville problem](../../../../../../sturm-liouville-problem.md), [integration by parts](../../../../../../integration-by-parts.md) shows $\lambda\geq0$. The zero [eigenvalue](../../../../../../eigenvalue.md) gives constant $X$, and $Y''=0$ together with $Y'(\pi)=0$ makes $Y$ constant too.

For positive [eigenvalues](../../../../../../eigenvalue.md), the side conditions give $\lambda=n^2$, $X_n=\cos(nx)$, $n\geq1$. The top condition chooses the [hyperbolic cosine](../../../../../../hyperbolic-cosine.md) factor $\cosh(n(\pi-y))$. Normalize it to one at $y=0$, obtaining

$$
u(x,y)=A_0+\sum_{n=1}^\infty a_n\cos(nx)
\frac{\cosh(n(\pi-y))}{\cosh(n\pi)}.
$$

The [orthogonality of integer Fourier modes](../../../../../../orthogonality-of-integer-fourier-modes.md) and the permitted interchange of [summation](../../../../../../summation.md) and [integration](../../../../../../integral-split.md) give

$$
A_0=\frac1\pi\int_0^\pi x(\pi-x)\,dx=\frac{\pi^2}{6},
\qquad
 a_n=\frac2\pi\int_0^\pi x(\pi-x)\cos(nx)\,dx.
$$

For the remaining [Fourier coefficients](../../../../../../fourier-coefficient.md), integrate by parts twice. The [sine](../../../../../../sine.md) boundary term vanishes, and with $f=x(\pi-x)$,

$$
\begin{aligned}
\int_0^\pi f(x)\cos(nx)\,dx
&=-\frac1n\int_0^\pi f'(x)\sin(nx)\,dx\\
&=\frac{[f'(x)\cos(nx)]_0^\pi}{n^2}
-\frac1{n^2}\int_0^\pi f''(x)\cos(nx)\,dx\\
&=-\frac{\pi(1+(-1)^n)}{n^2}.
\end{aligned}
$$

The last [integral](../../../../../../integral-split.md) vanishes because $f''=-2$ and $n$ is a positive [integer](../../../../../../integer-split.md). Thus $a_n=-2(1+(-1)^n)/n^2$: only even [Fourier modes](../../../../../../fourier-mode.md) survive, as expected from [reflection symmetry](../../../../../../reflection-symmetry.md) about $x=\pi/2$. Writing $n=2m$ gives

$$
\boxed{u(x,y)=\frac{\pi^2}{6}
-\sum_{m=1}^\infty\frac{\cos(2mx)}{m^2}
\frac{\cosh(2m(\pi-y))}{\cosh(2m\pi)}.}
$$

The factor involving [hyperbolic cosine](../../../../../../hyperbolic-cosine.md) lies between zero and one on the closed [rectangle](../../../../../../rectangle.md). Comparison with $\sum m^{-2}$ proves [uniform convergence](../../../../../../uniform-convergence.md), so the solution is continuous on the entire boundary and takes the prescribed bottom values. On every strip $y\geq\varepsilon>0$, the [Fourier coefficients](../../../../../../fourier-coefficient.md) have additional [exponential decay](../../../../../../exponential-decay.md), allowing differentiation and verifying [Laplace's equation](../../../../../../laplace-equation.md) and all three [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md).

To justify the endpoint calculation in [b](../b.md), differentiate at $0<x<\pi$, $y=0$ in the interior-edge sense:

$$
u_y(x,0)=2\sum_{m=1}^\infty\frac{\tanh(2m\pi)}m\cos(2mx).
$$

Subtracting $1$ from the [hyperbolic tangent](../../../../../../hyperbolic-tangent.md) leaves an absolutely convergent [series](../../../../../../series-mathematics.md). For the remaining part, the [power series](../../../../../../power-series.md) $-\log(1-z)=\sum_{m\geq1}z^m/m$ gives, by taking real parts at $z=re^{2ix}$ and then $r\uparrow1$,

$$
\sum_{m=1}^\infty\frac{\cos(2mx)}m=-\log(2\sin x),\qquad0<x<\pi.
$$

The same formula follows as the limit of the differentiated interior solution, since its leading multiplier is $e^{-2my}$. This establishes the boundary [normal derivative](../../../../../../normal-derivative.md) used in [b](../b.md). It also explains why the failure of the [corner compatibility condition for mixed boundary data](../../../../../../corner-compatibility-condition-for-mixed-boundary-data.md) affects first [derivatives](../../../../../../derivative.md) at the bottom corners without spoiling continuity of $u$ itself.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [Question 6](../../question-6.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
