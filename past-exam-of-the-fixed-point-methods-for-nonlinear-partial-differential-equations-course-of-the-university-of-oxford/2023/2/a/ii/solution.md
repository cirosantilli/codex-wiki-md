<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $E=\operatorname{aff}K$ be the [affine hull](../../../../../affine-hull.md) and put $k=\dim E\leq n$. If $k=0$, $K$ is a singleton and is [homeomorphic](../../../../../homeomorphism.md) to $\mathbb B^0$. Suppose $k>0$. Choose $k+1$ [affinely independent](../../../../../affine-independence.md) points of $K$ spanning $E$. Their [simplex](../../../../../simplex.md) is contained in $K$ because $K$ is a [convex set](../../../../../convex-set-split.md), and its [barycentre](../../../../../barycenter.md) $a$ has a neighbourhood in $E$ contained in that [simplex](../../../../../simplex.md). Identifying $E-a$ with $\mathbb R^k$, put $D=K-a$. For some $0<r\leq R<\infty$,

$$
r\mathbb B^k\subset D\subset R\mathbb B^k.
$$

Here the inner inclusion follows from that neighbourhood, and the outer one follows from the [compactness](../../../../../compact-space.md) of $K$.

Use the [Minkowski functional](../../../../../minkowski-functional.md)

$$
p(z)=\inf\{t>0:z\in tD\}.
$$

The inclusions imply $|z|/R\leq p(z)\leq|z|/r$. The fact that $D$ is a [convex set](../../../../../convex-set-split.md) implies $p(z+w)\leq p(z)+p(w)$: if $z\in sD$ and $w\in tD$, then $(z+w)/(s+t)$ is a [convex combination](../../../../../convex-combination.md) of points of $D$. Also $p(tz)=tp(z)$ for $t\geq0$. Consequently

$$
p(z)-p(w)\leq p(z-w)\leq|z-w|/r,
\qquad |p(z)-p(w)|\leq|z-w|/r.
$$

Thus $p$ is a [continuous function](../../../../../continuous-function.md). Since $D$ is closed and contains zero, $D=\{p\leq1\}$: the forward inclusion is immediate, and for the reverse inclusion one takes a limit of $z/t_j\in D$ with $t_j\to p(z)\leq1$, using [positive homogeneity](../../../../../positively-homogeneous-function-degree-one.md) and the fact that $D$ is a [convex set](../../../../../convex-set-split.md). For $z\ne0$, $p(z)>0$, so this limiting argument has no division by zero.

Define a radial [continuous map](../../../../../continuous-map.md) by

$$
h(0)=a,\qquad h(t\theta)=a+\frac{t}{p(\theta)}\theta
\quad(0<t\leq1,\ |\theta|=1).
$$

Each ray meets $D$ in exactly $\{s\theta:0\leq s\leq1/p(\theta)\}$. Hence $h$ is a [bijection](../../../../../bijection.md) from $\mathbb B^k$ to $K$. Away from zero its [continuity](../../../../../continuous-function.md) follows from that of $p$, and at zero $|h(t\theta)-a|\leq Rt$. A [continuous map](../../../../../continuous-map.md) that is a [bijection](../../../../../bijection.md) from a [compact space](../../../../../compact-space.md) to a [Hausdorff space](../../../../../hausdorff-space.md) is a [homeomorphism](../../../../../homeomorphism.md). Therefore

$$
\boxed{K\cong\mathbb B^k,\qquad k=\dim(\operatorname{aff}K).}
$$

Using the [affine hull](../../../../../affine-hull.md) is essential: $K$ can have empty interior in the ambient $\mathbb R^n$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../split.md)
6. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
