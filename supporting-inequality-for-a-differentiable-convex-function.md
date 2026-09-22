# Supporting inequality for a differentiable convex function

↑ **Parent:** [Convex function](convex-function.md)

For a differentiable real-valued [function](function-split.md) on an open [convex set](convex-set-split.md), [convexity](convex-function.md) is equivalent to the displayed inequality for all $x,y$ in its domain. To prove the forward direction, convexity gives $[f(x+t(y-x))-f(x)]/t\le f(y)-f(x)$ for $0<t\le1$. Take the [limit](limit-of-a-function.md) as $t\downarrow0$ using first-order [Taylor expansion](taylor-expansion.md).

Conversely, put $z=(1-t)x+ty$ and apply the supporting inequality at $z$ to both $x$ and $y$. Multiply the two inequalities by $1-t$ and $t$ and add them. The gradient terms cancel because $(1-t)(x-z)+t(y-z)=0$, leaving $f(z)\le(1-t)f(x)+tf(y)$. This is the defining [convexity](convex-function.md) inequality. The endpoint values $t=0,1$ hold as equalities.

## ↑ Ancestors (6)

1. [Convex function](convex-function.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Coordinate derivatives give directional Taylor expansion for convex functions](coordinate-derivatives-give-directional-taylor-expansion-for-convex-functions.md)
- [Solution](past-exam-of-the-probability-measure-and-martingales-course-of-the-university-of-oxford/2021/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/discrete-mathematics-probability-and-continuous-mathematics/4/a/solution.md)
