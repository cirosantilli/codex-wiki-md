# Mixed Dirichlet-Neumann Green function in a quadrant

↑ **Parent:** [Green's function](green-s-function-split.md)

For the quadrant $x,y>0$, the displayed [Green function](green-s-function-split.md) satisfies $\Delta G=\delta_{(\xi,\eta)}$, zero value on $y=0$ and zero outward normal [derivative](derivative.md) on $x=0$. The [method of images](method-of-images.md) uses the logarithmic [fundamental solution of the Laplace equation](fundamental-solution-of-the-laplace-equation.md) with coefficient $1/(2\pi)$: keep the source sign when reflecting across the Neumann side and reverse it when reflecting across the Dirichlet side. The four image signs are therefore $+,+,-,-$ for sources $(\xi,\eta),(-\xi,\eta),(\xi,-\eta),(-\xi,-\eta)$.

On $y=0$, equal numerator and denominator give zero. Evenness in $x$ gives the Neumann condition at $x=0$. The outward normal [derivative](derivative.md) on the Dirichlet side is the positive kernel

$$
\partial_nG(x,0,\xi,\eta)=\frac\eta\pi\left(\frac1{(x-\xi)^2+\eta^2}+\frac1{(x+\xi)^2+\eta^2}\right).
$$

[Green's second identity](green-second-identity.md) consequently gives $u(P)=\int_DGf+\int_{y=0}g\partial_nG$ for $\Delta u=f$ with these mixed boundary data, assuming any remote-boundary contribution vanishes. The sign convention is $\Delta G=+\delta$; changing to $-\Delta G=\delta$ changes both the Green function and the representation signs.

## ↑ Ancestors (5)

1. [Green's function](green-s-function-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-differential-equations-2-course-of-the-university-of-oxford/2014/2/b/solution.md)
