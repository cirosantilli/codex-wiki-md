# Single free node on a four-triangle mixed-boundary mesh

↑ **Parent:** [Finite element assembly](finite-element-assembly.md)

Triangulate the region $0\leq x,y\leq2$, $x+y\geq2$ by $x=1$, $y=1$, and $x+y=3$. Impose zero Dirichlet data on the horizontal and vertical exterior edges and zero Neumann data on the sloping edge. Only the midpoint $B=(1,1)$ of the sloping edge remains free in the continuous piecewise linear space. For source one, its stiffness entry is $1/2+1/2+1=2$, while its load is three triangle contributions of $1/6$. The single free value is therefore $1/4$.

## ↑ Ancestors (7)

1. [Finite element assembly](finite-element-assembly.md)
2. [Finite element method](finite-element-method-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
