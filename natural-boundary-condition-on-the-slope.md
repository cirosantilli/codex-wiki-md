# Natural boundary condition on the slope

↑ **Parent:** [Natural boundary conditions for a free endpoint](natural-boundary-conditions-for-a-free-endpoint.md)

For a [functional](functional.md) $J[y]=\int F(x,y,y',y'')\,dx$, two applications of [integration by parts](integration-by-parts.md) leave the boundary term

$$
\left[\left(F_{y'}-\frac d{dx}F_{y''}\right)\delta y+F_{y''}\delta y'\right]_a^b.
$$

If the endpoint displacement is fixed but its slope is free, $\delta y=0$ while $\delta y'$ is arbitrary. The [first variation](first-variation.md) therefore forces $F_{y''}=0$ at that endpoint. For the beam energy density $F=\beta(y'')^2/2-\alpha(y')^2/2$ with $\beta>0$, this gives $y''=0$, the zero-[bending moment](bending-moment.md) condition. A clamped endpoint instead prescribes the slope and has $\delta y'=0$.

## ↑ Ancestors (6)

1. [Natural boundary conditions for a free endpoint](natural-boundary-conditions-for-a-free-endpoint.md)
2. [Euler-Lagrange equation](euler-lagrange-equation.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
