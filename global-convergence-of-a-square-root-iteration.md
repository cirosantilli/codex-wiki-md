# Global convergence of a square-root iteration

↑ **Parent:** [Fixed point stability for an iteration](fixed-point-stability-for-an-iteration.md)

For every $y_0\geq0$, this [recurrence relation](recurrence-relation.md) converges to the unique nonnegative [fixed point](fixed-point.md) $2$. If $0\leq y<2$, then $y<\sqrt{2+y}<2$, since $2+y-y^2=(2-y)(1+y)>0$. If $y>2$, then $2<\sqrt{2+y}<y$. Thus the iterates form a [monotone bounded sequence](monotone-bounded-sequence.md), and [continuity](continuous-function.md) forces their limit to be $2$. A [cobweb plot](cobweb-plot.md) alternates vertical steps to $v=\sqrt{2+u}$ and horizontal steps to $v=u$, approaching the same intersection from either side. More quantitatively,

$$
y_{n+1}-2=\frac{y_n-2}{\sqrt{2+y_n}+2},
$$

so the error keeps its sign and decreases in [absolute value](absolute-value.md) by at least the uniform factor $1/(2+\sqrt2)$. The asymptotic factor is $1/4$.

## ↑ Ancestors (5)

1. [Fixed point stability for an iteration](fixed-point-stability-for-an-iteration.md)
2. [Dynamical systems](dynamical-systems-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/19/b/ii/solution.md)
