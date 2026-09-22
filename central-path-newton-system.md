# Central-path Newton system

↑ **Parent:** [Central path](central-path.md)

At a target barrier parameter $\mu$, let $r_p=Ax-b-s$, $r_d=A^\top y-c$, $r_c=y+\mu\nabla F(s)$. The Newton direction solves

$$
A\Delta x-\Delta s=-r_p,\quad A^\top\Delta y=-r_d,\quad\Delta y+\mu\nabla^2F(s)\Delta s=-r_c.
$$

Full column rank of $A$ and a positive-definite barrier Hessian give a positive-definite reduced matrix. Backtracking must keep both cone variables interior; solving the linear equations alone does not guarantee that a full step stays inside the cones.

## ↑ Ancestors (9)

1. [Central path](central-path.md)
2. [Self-concordant barrier](self-concordant-barrier.md)
3. [Interior-point method](interior-point-method.md)
4. [Conic optimization](conic-optimization.md)
5. [Convex optimization](convex-optimization-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Central path](central-path.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-62/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-65/4/a/solution.md)
