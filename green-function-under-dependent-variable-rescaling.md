# Green function under dependent-variable rescaling

↑ **Parent:** [Green's function](green-s-function-split.md)

Suppose a linear ordinary [differential operator](differential-operator.md) satisfies $L(qv)=rMv$ on an interval, where the functions $q,r$ never vanish and homogeneous endpoint [boundary conditions](boundary-condition.md) for $y=qv$ correspond to those used for $v$. If $G_M$ is a [Green's function](green-s-function-split.md) for $M$, then $Ly=f$ is equivalent to $Mv=f/r$, so

$$
y(x)=q(x)\int G_M(x,s)\frac{f(s)}{r(s)}\,ds.
$$

Thus the displayed kernel is the [Green's function](green-s-function-split.md) for the original, possibly non-normalized operator. The source factor belongs at $s$, while the dependent-variable factor belongs at $x$.

For $Ly=x^2y''-2xy'+(x^2+2)y$ on $[\pi/2,\pi]$ with zero endpoint values, $q=x$ and $r=x^3$ reduce the equation to $Mv=v''+v$. The kernel of $M$ is $\cos(x_<)\sin(x_>)$, where $x_<=\min(x,s)$ and $x_>=\max(x,s)$. Therefore $G_L(x,s)=x\cos(x_<)\sin(x_>)/s^3$. Its first derivative has jump $1/s^2$, as required by the leading coefficient $s^2$ of $L$.

## ↑ Ancestors (5)

1. [Green's function](green-s-function-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford/2011/7/solution.md)
