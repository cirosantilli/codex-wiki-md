<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The sufficiency claim requires a domain qualification. For a continuously differentiable [vector field](../../../../../../vector-field.md) on all of $\mathbb R^3$, or more generally on a [simply connected](../../../../../../simply-connected-space.md) open domain, the equivalence is valid. On an arbitrary domain, vanishing [curl](../../../../../../curl.md) is necessary but may fail to be sufficient.

**Necessity.** Suppose every closed-curve [line integral](../../../../../../line-integral.md) vanishes. Fix a point $p$ in the open domain and a [unit vector](../../../../../../unit-vector.md) $a$. A sufficiently small planar disk $D_\varepsilon$ of radius $\varepsilon$, centred at $p$ and normal to $a$, lies in the domain. [Stokes theorem](../../../../../../stokes-theorem.md) gives

$$
0=\oint_{\partial D_\varepsilon}\mathbf F\cdot d\mathbf r
=\iint_{D_\varepsilon}(\nabla\times\mathbf F)\cdot a\,dS.
$$

Divide by $\pi\varepsilon^2$ and let $\varepsilon\downarrow0$. By [continuity](../../../../../../continuous-function.md), the average tends to $(\nabla\times\mathbf F)(p)\cdot a$. Taking the three coordinate directions proves $\boxed{\nabla\times\mathbf F=0}$ everywhere.

**Sufficiency on $\mathbb R^3$.** A direct proof constructs a [potential of a conservative vector field](../../../../../../potential-of-a-conservative-vector-field.md). Put

$$
\phi(x)=\int_0^1\mathbf F(tx)\cdot x\,dt.
$$

Write $F_j$ for the components of $\mathbf F$. Vanishing [curl](../../../../../../curl.md) says $\partial_iF_j=\partial_jF_i$. Differentiation under the integral, followed by the [chain rule](../../../../../../chain-rule.md), gives

$$
\begin{aligned}
\partial_i\phi(x)
&=\int_0^1\left[F_i(tx)+t\sum_{j=1}^3x_j\partial_iF_j(tx)\right]dt\\
&=\int_0^1\left[F_i(tx)+t\frac d{dt}F_i(tx)\right]dt
=\bigl[tF_i(tx)\bigr]_0^1=F_i(x).
\end{aligned}
$$

This is the [radial integral potential for a curl-free field](../../../../../../radial-integral-potential-for-a-curl-free-field.md). The [fundamental theorem for line integrals](../../../../../../fundamental-theorem-for-line-integrals.md) now gives zero on every closed curve. On a [simply connected](../../../../../../simply-connected-space.md) open domain the analogous argument uses path integrals: every loop can be contracted within the domain, and applying [Stokes theorem](../../../../../../stokes-theorem.md) to a piecewise smooth contraction makes its [circulation](../../../../../../circulation-physics.md) zero. Equivalently, whenever a particular loop bounds an oriented spanning surface entirely in the domain, [Stokes theorem](../../../../../../stokes-theorem.md) immediately gives zero for that loop.

**Why the domain matters.** On $U=\mathbb R^3\setminus\{(0,0,z):z\in\mathbb R\}$, the [smooth](../../../../../../smooth-function.md) [vector field](../../../../../../vector-field.md)

$$
\mathbf F=\left(-\frac y{x^2+y^2},\frac x{x^2+y^2},0\right)
$$

has zero [curl](../../../../../../curl.md), but its [line integral](../../../../../../line-integral.md) around the unit [circle](../../../../../../circle.md) in $z=0$ is $2\pi$, as in [ii](../../1/b/ii.md). No spanning surface for this loop can lie entirely in $U$. The literal claim without a condition on the domain therefore has this counterexample.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
