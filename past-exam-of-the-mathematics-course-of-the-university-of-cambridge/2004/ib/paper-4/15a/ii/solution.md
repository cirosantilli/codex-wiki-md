<h1 id="15a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take the [Fourier transform](../../../../../../fourier-transform.md) in $x$ of the [Laplace equation](../../../../../../laplace-equation.md). Writing $U(s,y)$ for the transformed solution gives $U_{yy}-s^2U=0$. Its boundary values give

$$
U(s,y)=\widehat g(s)\frac{\sinh(s(1-y))}{\sinh s},
$$

with the multiplier at $s=0$ understood as $1-y$. The particular data simplify this to $U(s,y)=2\sinh(s(1-y))$ for $|s|<1$, and zero outside. Thus, with $a=1-y$, the [Fourier solution of the strip Dirichlet problem](../../../../../../fourier-solution-of-the-strip-dirichlet-problem.md) is

$$
u(x,y)=\frac1\pi\int_{-1}^1\sinh(as)e^{-isx}ds,
\qquad
\boxed{u(x,y)=\frac{2i}{\pi(a^2+x^2)}\bigl(x\sinh a\cos x-a\cosh a\sin x\bigr).}
$$

The displayed closed expression applies in the open strip. The integral defines its continuous boundary values, including the removable point $(x,a)=(0,0)$. It gives $u(x,0)=g(x)$ and $u(x,1)=0$. Differentiation under this finite integral verifies $u_{xx}+u_{yy}=0$ directly, since each integrand has opposite second derivatives in $x$ and $y$.

The boundary conditions alone do not specify a unique solution without a growth restriction: adding $Ce^{\pi x}\sin(\pi y)$ preserves both boundary values and harmonicity. The constructed solution is bounded, and it is unique among bounded solutions continuous on the closed strip. To see this, apply the [maximum principle for harmonic functions](../../../../../../maximum-principle-for-harmonic-functions.md) to a bounded real or imaginary component $w$ of the difference. For $0<\delta<\pi$, the positive harmonic function $B(x,y)=\cosh(\delta x)\cos(\delta(y-1/2))$ has a positive minimum factor in $y\in[0,1]$. For any $\varepsilon>0$, the functions $\pm w-\varepsilon B$ are nonpositive on the horizontal sides of a sufficiently wide rectangle and on its vertical sides, because $w$ is bounded and $B$ grows there. The maximum principle gives $|w|\leq\varepsilon B$ at every fixed point. Letting $\varepsilon\downarrow0$ proves uniqueness in this natural Fourier solution class.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [15A](../../15a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
