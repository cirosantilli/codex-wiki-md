# Quartic surface with axes and a circle as its zero set

↑ **Parent:** [Critical point](critical-point.md)

The zero [level set](level-set.md) of $F_R$ is the union of the coordinate axes and the [circle](circle.md) of [radius](radius.md) $R$. The [gradient](gradient.md) is

$$
\nabla F_R=\bigl(y(3x^2+y^2-R^2),\ x(x^2+3y^2-R^2)\bigr)^T.
$$

Its nine [stationary points](stationary-point.md) are the origin, the four axis points at distance $R$, and the four points with $x^2=y^2=R^2/4$. The factored [gradient](gradient.md) proves completeness: a zero coordinate gives the five axis cases; two nonzero coordinates give a linear system in $x^2,y^2$.

The [Hessian matrix](hessian-matrix.md) has diagonal entries $6xy$ and off-diagonal entries $3(x^2+y^2)-R^2$. At the origin its [eigenvalues](eigenvalue.md) are $\pm R^2$; at the four unit-direction axis points they are $\pm2R^2$. These are [saddle points of a scalar function](saddle-point-of-a-scalar-function.md). At the two interior points with equal coordinate signs, the [eigenvalues](eigenvalue.md) are $R^2,2R^2$, giving strict [local minima](local-minimum.md) of value $-R^4/8$. Opposite coordinate signs give the negative [eigenvalues](eigenvalue.md) and strict [local maxima](local-maximum.md) of value $R^4/8$.

On the zero circle, $\nabla F_R=2xy(x,y)^T$. Hence its direction is radial outward for $xy>0$, inward for $xy<0$, and zero at the four axis crossings. This simple geometric sign rule links the zero [level set](level-set.md) to the [gradient](gradient.md) sketch without requiring numerical differentiation.

## ↑ Ancestors (5)

1. [Critical point](critical-point.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/16/a/solution.md)
