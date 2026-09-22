# Quadratic smoothing spline for interval averages

↑ **Parent:** [Smoothing spline](smoothing-spline.md)

Let $L_i g$ be the average of $g$ on successive knot intervals. Minimizing the displayed loss over $C^1[a,b]$ gives a [quadratic spline](quadratic-spline.md) with constant tails outside the first and last knots. To prove the reduction, choose the unique constant-tail quadratic spline $q$ with the same interval averages as a candidate $g$, and put $v=g-q$. Since $q''$ is constant on every knot interval, $q'$ is continuous and vanishes on both tails, [integration by parts](integration-by-parts.md) gives $\int q'v'=-\sum_iq''|_{I_i}\int_{I_i}v=0$. Consequently the data loss is unchanged and $\int(g')^2=\int(q')^2+\int(v')^2$. The penalty decreases strictly unless $v$ is constant; its zero interval averages then force $v=0$. The finite-dimensional quadratic optimization on this spline space also gives a unique minimizer because the interval-average map is injective.

## ↑ Ancestors (8)

1. [Smoothing spline](smoothing-spline.md)
2. [Nonparametric regression](nonparametric-regression.md)
3. [Nonparametric statistics](nonparametric-statistics-split.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/6/solution.md)
- [Quadratic spline](quadratic-spline.md)
