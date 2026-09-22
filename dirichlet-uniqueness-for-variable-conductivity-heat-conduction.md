# Dirichlet uniqueness for variable-conductivity heat conduction

↑ **Parent:** [Heat equation](heat-equation.md)

Suppose $k>0$ and two sufficiently regular [steady state](steady-state.md) [temperature](temperature-split.md) profiles solve the same [heat equation](heat-equation.md) with the same [PDE source term](source-term-in-a-partial-differential-equation.md) $H$ and the same [Dirichlet boundary condition](dirichlet-boundary-condition.md) $h$. Their difference $w$ satisfies $\nabla\cdot(k\nabla w)=0$ and $w=0$ on the boundary. The [divergence theorem](divergence-theorem.md) applied to $wk\nabla w$ gives

$$
0=\int_Rw\nabla\cdot(k\nabla w)\,dV=-\int_Rk\|\nabla w\|^2\,dV.
$$

Thus $\nabla w=0$, and the zero boundary values force $w=0$ on each connected component. The argument proves uniqueness without asserting existence and without replacing the spatially varying [thermal conductivity](thermal-conductivity.md) by a constant. For [weak solutions](weak-solution.md), the same calculation is the energy argument obtained by choosing $w$ as the [test function](test-function.md), under the usual boundedness and positive lower bound assumptions on $k$.

## ↑ Ancestors (7)

1. [Heat equation](heat-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-v/2/d/i/solution.md)
