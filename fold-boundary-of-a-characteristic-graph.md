# Fold boundary of a characteristic graph

↑ **Parent:** [Method of characteristics](method-of-characteristics.md)

A smooth characteristic surface in three-dimensional $(x,y,u)$ space need not remain the graph of a [differentiable function](differentiable-function.md) after [projection](projection-linear-algebra.md) to the $(x,y)$ plane. Locally, if its implicit equation is $F(x,y,u)=0$, the [implicit function theorem](implicit-function-theorem.md) produces a smooth graph wherever $F_u\ne0$. At a point where $F_u=0$, the [projection](projection-linear-algebra.md) can fold and two graph branches can meet. A real radical formula may continue to that boundary even though its [partial derivatives](partial-derivative.md) diverge there. Thus the closed set on which the radical is real can be larger than the open domain of a [classical solution](classical-solution.md).

For example,

$$
F=16u^2-(30x+24y)u+9y^2-40xy
$$

has two branches $u=(15x+12y\pm5\sqrt{9x^2+40xy})/16$. On them $F_u=\pm10\sqrt{9x^2+40xy}$, so the graph [projection](projection-linear-algebra.md) folds on the nonzero boundary points of $9x^2+40xy\ge0$. Its gradient in the base variables does not vanish at those points, and [differentiation](differentiation.md) of the radical gives the transverse [derivative](derivative.md) singularity. The characteristic surface itself can be smooth there: its graph coordinate is the part which fails. Boundary values may still be defined continuously, but they do not create an open classical-solution neighborhood.

## ↑ Ancestors (8)

1. [Method of characteristics](method-of-characteristics.md)
2. [Characteristic curve](characteristic-curve.md)
3. [Transport equation](transport-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2008-printed-variant/8/solution.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2008/8/solution.md)
