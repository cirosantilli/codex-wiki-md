# Sticking solutions of a bounded square-root differential equation

↑ **Parent:** [Delayed solutions of a square-root differential equation](delayed-solutions-of-a-square-root-differential-equation.md)

For the [autonomous differential equation](autonomous-system-mathematics.md) $v'=\sqrt{1-v^2}$, the real solutions are nondecreasing and lie in $[-1,1]$. On each nonconstant interval, [separation of variables](separation-of-variables.md) gives $\arcsin v=t-C$, so the solution crosses from $-1$ to $1$ in exactly time $\pi$. Every nonconstant solution on the entire real time axis is consequently

$$
v(t)=\begin{cases}-1,&t\leq a,\\-\cos(t-a),&a<t<a+\pi,\\1,&t\geq a+\pi,\end{cases}
$$

for some real $a$. The two constant solutions $v\equiv\pm1$ complete the list; solutions on shorter intervals are restrictions of these. At the joins both the [derivative](derivative.md) and the right-hand side are zero, so these are [continuously differentiable functions](continuously-differentiable-function.md). The right-hand side is continuous but fails [Lipschitz continuity](lipschitz-continuity.md) at both endpoints, allowing arbitrary waiting time at $-1$ before departure. Once $v$ reaches $1$, monotonicity forces it to stay there. The sine representation without the nonnegative-cosine restriction would incorrectly introduce decreasing pieces.

## ↑ Ancestors (8)

1. [Delayed solutions of a square-root differential equation](delayed-solutions-of-a-square-root-differential-equation.md)
2. [Peano existence theorem](peano-existence-theorem.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1/16/a/iii/solution.md)
