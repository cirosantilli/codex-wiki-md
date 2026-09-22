# Periodic square-wave relaxation for the inviscid Burgers equation

↑ **Parent:** [Inviscid Burgers equation](inviscid-burgers-equation.md)

Take period-one data equal to one on $[k-1/2,k]$ and zero on $(k,k+1/2)$. Before $t=1$, the separate [rectangular pulse solutions of the inviscid Burgers equation](rectangular-pulse-solution-of-the-inviscid-burgers-equation.md) do not overlap in their interiors. At $t=1$ each shock meets the two neighboring fans. Afterward, on the interval between shocks $s_{k-1}$ and $s_k$, the solution remains $(x-k+1/2)/t$. The [Rankine-Hugoniot condition](rankine-hugoniot-conditions.md) gives $s_k'=(s_k-k)/t$ and $s_k(1)=k+1/2$, hence $s_k=k+t/2$.

The title formula uses the [fractional part](fractional-part.md) and chooses right-hand shock values. Its left and right states are $1/2+1/(2t)$ and $1/2-1/(2t)$, making every shock a causal [entropy shock](entropy-shock.md) of speed $1/2$. Therefore $\sup_x|u(x,t)-1/2|\leq1/(2t)$: the periodic [entropy solution](entropy-solution.md) converges uniformly to its conserved mean even though it has a jump at every finite time. Periodizing a nonlinear solution is valid here only before the supports interact; after interaction the matching shock calculation is essential.

## ↑ Ancestors (8)

1. [Inviscid Burgers equation](inviscid-burgers-equation.md)
2. [Scalar conservation law](scalar-conservation-law.md)
3. [Transport equation](transport-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-applied-partial-differential-equations-course-of-the-university-of-oxford/2023/2/c/iii/solution.md)
