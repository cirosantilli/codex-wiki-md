# Minimum roof length at fixed wall height and cross-sectional area

↑ **Parent:** [Lagrange multiplier](lagrange-multiplier.md)

For $A,h>0$, a rectangular cross section of width $w$ and height $h$, capped by a symmetric triangular roof at angle $0<\theta<\pi/2$, has area $A=wh+w^2\tan\theta/4$. Its total sloping roof length is $w\sec\theta$. A cost $2\alpha h+\beta w\sec\theta$ with $\beta>0$ has the same minimizing shape as this roof length, since the fixed wall term is constant.

The [Lagrange multiplier](lagrange-multiplier.md) equations for $w\sec\theta$ under the area constraint give $w(1-\tan^2\theta)=4h\tan\theta$. This is the first displayed condition; it also implies $\theta<\pi/4$. Eliminating $\tan\theta=4(A-wh)/w^2$ gives the second condition.

For a global check, the squared roof length is $Q(w)=w^2+16(A-wh)^2/w^2$ for $0<w<A/h$. Its [derivative](derivative.md) has the sign of $w^4+16Ahw-16A^2$, a strictly increasing expression with one root in that interval. Thus this root is the unique minimum. The shape is independent of the positive roof-cost coefficient and the constant wall cost. If $\beta=0$, every feasible shape has the same cost and these conditions are no longer necessary.

## ↑ Ancestors (5)

1. [Lagrange multiplier](lagrange-multiplier.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/20/b/solution.md)
