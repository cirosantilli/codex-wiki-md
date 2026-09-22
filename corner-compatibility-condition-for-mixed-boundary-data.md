# Corner compatibility condition for mixed boundary data

↑ **Parent:** [Mixed boundary condition](mixed-boundary-condition.md)

Consider the top-right corner $(b,d)$ of a rectangle. Suppose the top [Dirichlet boundary condition](dirichlet-boundary-condition.md) is $u(x,d)=g(x)$ and the right [Neumann boundary condition](neumann-boundary-condition.md), with outward normal in the positive $x$ direction, is $u_x(b,y)=q(y)$. A solution that is a [continuously differentiable function](continuously-differentiable-function.md) up to the corner necessarily satisfies $g'(b)=q(d)$: differentiating the top [boundary trace](boundary-trace-of-a-function.md) in its tangential $x$ direction gives $u_x(b,d)=g'(b)$, while the right-edge condition gives the same [partial derivative](partial-derivative.md) as $q(d)$.

This is a necessary compatibility condition, not an existence theorem. If it fails, a solution can still satisfy the interior equation and the boundary conditions on open edges while failing to have a continuous first derivative at that corner. In particular, homogeneous right-edge [Neumann boundary conditions](neumann-boundary-condition.md) require $g'(b)=0$ for a solution continuously differentiable at the top-right corner. Boundary values may remain continuous even when this derivative requirement fails.

## ↑ Ancestors (8)

1. [Mixed boundary condition](mixed-boundary-condition.md)
2. [Boundary condition](boundary-condition.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-v-resit/question-6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-v-resit/question-6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2021/prelims/mathematics-v-resit/question-6/b/solution.md)
