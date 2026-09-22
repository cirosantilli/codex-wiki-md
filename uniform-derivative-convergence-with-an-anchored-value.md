# Uniform derivative convergence with an anchored value

↑ **Parent:** [Uniform convergence](uniform-convergence.md)

Let $f_n$ be [continuously differentiable functions](continuously-differentiable-function.md) on an [interval](interval-mathematics.md) $I$. If $f_n'\to g$ by [uniform convergence](uniform-convergence.md) on $I$ and $f_n(c)\to A$ at one fixed $c\in I$, then $f_n$ converge locally uniformly to a [continuously differentiable function](continuously-differentiable-function.md) $f$ with $f'=g$. If $I$ is bounded, the convergence is uniform on all of $I$.[Basic Analysis: Introduction to Real Analysis, Volume I by Jiří Lebl, §6.2.3, Theorem 6.2.10 and the unbounded-interval observation following its proof](basic-analysis-introduction-to-real-analysis-volume-i-by-jiri-lebl/6-2-interchange-of-limits.md)

The anchor fixes the additive constant that a [derivative](derivative.md) cannot see. By the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md), define

$$
f(x)=A+\int_c^xg(t)\,dt,\qquad |f_n(x)-f(x)|\leq|f_n(c)-A|+|x-c|\|f_n'-g\|_\infty.
$$

The [uniform limit theorem](uniform-limit-theorem.md) makes $g$ a [continuous function](continuous-function.md), so the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) gives $f'=g$. The displayed estimate proves [uniform convergence](uniform-convergence.md) wherever $|x-c|$ has a common finite bound, and therefore proves [locally uniform convergence](locally-uniform-convergence.md) on any [interval](interval-mathematics.md).

For example, on $[0,2]$ take $f_n(x)=3+1/n+x^2/2+x/n$. Its [derivative](derivative.md) is $x+1/n$, with [supremum error](supremum-error.md) $1/n$ from $g(x)=x$, and $f_n(0)\to3$. The reconstructed [uniform limit](uniform-limit.md) is $f(x)=3+x^2/2$; the exact [supremum error](supremum-error.md) is $3/n$, equal to the bound above. Without an anchor, the constant [functions](function-split.md) $f_n(x)=n$ have zero [derivatives](derivative.md) but no finite [pointwise limit](pointwise-limit.md). On the [real line](real-line.md), $f_n(x)=x/n$ has convergent anchored values and uniformly convergent [derivatives](derivative.md), but its [supremum error](supremum-error.md) from zero is infinite. The bounded-distance condition has a real role.

## ↑ Ancestors (7)

1. [Uniform convergence](uniform-convergence.md)
2. [Sequence and series](sequence-and-series-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-1/11f/solution.md)
- [Uniform convergence](uniform-convergence.md)
