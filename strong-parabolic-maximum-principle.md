# Strong parabolic maximum principle

↑ **Parent:** [Maximum principle](maximum-principle.md)

Let $\Omega$ be a connected domain and $u$ a classical subsolution of

$$
u_t-\sum_{i,j}a_{ij}(x,t)u_{x_ix_j}+\sum_i b_i(x,t)u_{x_i}+c(x,t)u\leq0,
$$

with uniformly positive definite diffusion matrix, continuous bounded coefficients, and $c\geq0$. If $u\leq0$ on $\Omega\times(0,T]$ and $u(x_0,t_0)=0$ at a spatial interior point with $t_0>0$, then $u=0$ on $\Omega\times(0,t_0]$. Continuity supplies the same conclusion at initial and lateral points where the solution extends continuously. There is generally no conclusion about times after $t_0$ for a subsolution.

One proof applies the strict positivity principle to $w=-u\geq0$, a supersolution: any positive value at an earlier interior point propagates to positive values at every later interior point along a chain of overlapping interior balls, contradicting $w(x_0,t_0)=0$. Nonnegative zeroth-order terms can be bounded on each compact time cylinder and removed from this positivity argument by an exponential multiplier. For the inequality $u_t-\Delta u+b\cdot\nabla u+u^3\leq0$, use $c=u^2\geq0$ after the weak [maximum principle](maximum-principle.md) has established $u\leq0$.

## ↑ Ancestors (6)

1. [Maximum principle](maximum-principle.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-differential-equations-1-course-of-the-university-of-oxford/2023/3/a/i/solution.md)
