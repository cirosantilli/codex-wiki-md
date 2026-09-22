# Brunn-Minkowski theorem

↑ **Parent:** [Minkowski addition](minkowski-addition.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brunn–Minkowski_theorem)

Let $n\geq1$ and let $A,B\subseteq\mathbb R^n$ be nonempty [Lebesgue measurable sets](lebesgue-measurable-set.md) with finite [Lebesgue measures](lebesgue-measure.md). Assume that $A+B$ is also a [Lebesgue measurable set](lebesgue-measurable-set.md); its [measure](measure-split.md) may be infinite. Then

$$
\lambda_n(A+B)^{1/n}\geq\lambda_n(A)^{1/n}+\lambda_n(B)^{1/n}.
$$

Here $\lambda_n$ denotes $n$-dimensional [Lebesgue measure](lebesgue-measure.md) in [Euclidean space](euclidean-norm.md). Nonempty [compact sets](compact-space.md) and nonempty [open sets](open-set.md) of finite [measure](measure-split.md) satisfy the measurability assumptions. Measurability of arbitrary summands alone does not guarantee measurability of their [Minkowski sum](minkowski-addition.md). The theorem does not require [convexity](convex-function.md). See [R. J. Gardner, The Brunn-Minkowski Inequality (2002), Theorem 4.1 and the following remarks](https://sites.stat.washington.edu/jaw/COURSES/520s/523/HO.523.20/Gardner.BullAMS.02.pdf).

The $n$th root converts a volume into a quantity that scales like a [length](length.md): [uniform dilation](uniform-dilation.md) gives $\lambda_n(tA)^{1/n}=t\lambda_n(A)^{1/n}$ for $t>0$. In the [Euclidean plane](euclidean-plane.md) the theorem compares square roots of [areas](surface-area.md), not the [areas](surface-area.md) themselves. For the two [rectangles](rectangle.md) above it reads $3\geq\sqrt2+\sqrt2=2\sqrt2$. Equivalently their sum has [area](surface-area.md) $9\geq8$. For the two [disks](disk-mathematics.md), it reads $3\sqrt\pi=\sqrt\pi+2\sqrt\pi$, an equality. These are exact geometric examples, not measured data.

Applying the theorem to the scaled [sets](set-split.md) gives, whenever that sum is a [Lebesgue measurable set](lebesgue-measurable-set.md),

$$
\lambda_n((1-t)A+tB)^{1/n}\geq(1-t)\lambda_n(A)^{1/n}+t\lambda_n(B)^{1/n},\qquad 0<t<1.
$$

For [convex bodies](convex-body.md), this means the root-volume of the interpolated shape lies above the straight line between the input root-volumes. In fact $t\mapsto\lambda_n((1-t)A+tB)^{1/n}$ is a [concave function](concave-function.md) on $[0,1]$: [convexity](convex-function.md) gives $sA+tA=(s+t)A$ for $s,t\geq0$, so interpolating two intermediate shapes gives another intermediate shape and the same inequality applies. The beauty is that no particular boundary shape appears in the bound: possible pointwise displacements force a minimum amount of space.

For [convex bodies](convex-body.md) $A,B$, equality holds exactly when they are [homothetic convex bodies](homothetic-convex-bodies.md), meaning $B=v+sA$ for some [vector](vector.md) $v$ and $s>0$. This equality qualification is part of the [Brunn-Minkowski theorem](brunn-minkowski-theorem.md) for [convex bodies](convex-body.md). [Gardner (2002), introduction, equation 2 and its equality condition](https://sites.stat.washington.edu/jaw/COURSES/520s/523/HO.523.20/Gardner.BullAMS.02.pdf) For positive-sided axis-aligned [rectangles](rectangle.md), the comparison can be checked directly:

$$
(a+c)(b+d)-(\sqrt{ab}+\sqrt{cd})^2=(\sqrt{ad}-\sqrt{bc})^2\geq0.
$$

Equality requires $ad=bc$: the [rectangles](rectangle.md) must have the same aspect ratio. Our $2\times1$ and $1\times2$ [rectangles](rectangle.md) do not. All positive-radius [disks](disk-mathematics.md) are [homothetic convex bodies](homothetic-convex-bodies.md), explaining their equality.

Do not apply that equality criterion without its hypotheses. If $A=\{a\}$, its [Lebesgue measure](lebesgue-measure.md) is zero and $A+B$ is a [translation](translation-geometry.md) of $B$, so equality holds even for nonconvex $B$. Also, changing a summand on a [null set](null-set.md) can change the [measure](measure-split.md) of its [Minkowski sum](minkowski-addition.md): in one dimension, $A=[0,1]\cup\{3\}$ and $B=[0,1]$ both have [measure](measure-split.md) $1$, but $A+B=[0,2]\cup[3,4]$ has [measure](measure-split.md) $3$. Removing the single extra point restores equality with sum [measure](measure-split.md) $2$. Thus merely being equal almost everywhere to [homothetic convex bodies](homothetic-convex-bodies.md) is not a sufficient equality test for arbitrary [sets](set-split.md).

The [Brunn-Minkowski theorem](brunn-minkowski-theorem.md) also bounds the collision-region [volume](volume.md): for positive-volume [compact sets](compact-space.md) $O,R$, reflection preserves [Lebesgue measure](lebesgue-measure.md), so $\lambda_n(O+(-R))^{1/n}\geq\lambda_n(O)^{1/n}+\lambda_n(R)^{1/n}$. In the toy collision example this gives [area](surface-area.md) at least $(2+\sqrt2)^2=6+4\sqrt2\approx11.657$, compared with the exact [area](surface-area.md) $12$. A lower bound alone does not identify safe reference [positions](position.md); the actual [Minkowski sum](minkowski-addition.md) supplies those.

## ↑ Ancestors (6)

1. [Minkowski addition](minkowski-addition.md)
2. [Convex geometry](convex-geometry.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Brunn-Minkowski theorem](brunn-minkowski-theorem.md)
- [Convex body](convex-body.md)
- [Homothetic convex bodies](homothetic-convex-bodies.md)
- [Minkowski addition](minkowski-addition.md)
