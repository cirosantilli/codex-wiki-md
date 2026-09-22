<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

At each point, apply the indefinite-signature version of the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) to any local coframe, choosing one timelike and three spacelike one-forms. This produces an [orthonormal coframe in spacetime](../../../../../orthonormal-coframe-in-spacetime.md) $\{\theta^a\}$ satisfying

$$
g=\eta_{ab}\theta^a\otimes\theta^b,
\qquad \eta_{ab}=\operatorname{diag}(-1,1,1,1).
$$

It is unique only up to a local [Lorentz transformation](../../../../../lorentz-transformation.md). The torsion-free [connection 1-forms](../../../../../connection-1-form-split.md) are then determined by [Cartan's first structure equation](../../../../../cartan-s-first-structure-equation.md) and [metric compatibility](../../../../../metric-compatibility.md),

$$
d\theta^a+\omega^a{}_b\wedge\theta^b=0,
\qquad \omega_{ab}=-\omega_{ba}.
$$

[Cartan's second structure equation](../../../../../cartan-s-second-structure-equation.md) gives the [curvature 2-forms](../../../../../curvature-2-form.md)

$$
\mathcal R^a{}_b=d\omega^a{}_b+\omega^a{}_c\wedge\omega^c{}_b
=\frac12R^a{}_{bcd}\theta^c\wedge\theta^d,
$$

and contraction gives the [Ricci tensor](../../../../../ricci-tensor.md) $R_{bd}=R^a{}_{bad}$.

For the displayed metric, take

$$
\theta^0=dt,
\qquad \theta^i=e^{-t}dx^i
\quad(i=1,2,3).
$$

Then $d\theta^0=0$ and $d\theta^i=-\theta^0\wedge\theta^i$. The nonzero connection forms are therefore

$$
\boxed{\omega^i{}_0=-\theta^i,
\qquad \omega^0{}_i=-\theta^i},
$$

with $\omega^i{}_j=0$. A second application of the structure equations gives

$$
\mathcal R^i{}_0=\theta^0\wedge\theta^i,
\qquad
\mathcal R^0{}_i=\theta^0\wedge\theta^i,
\qquad
\mathcal R^i{}_j=\theta^i\wedge\theta^j.
$$

Equivalently,

$$
\boxed{\mathcal R^a{}_b=\theta^a\wedge\theta_b},
$$

so this is a [constant sectional curvature](../../../../../constant-sectional-curvature.md) spacetime with $K=1$. In four dimensions,

$$
R_{ab}=3g_{ab},
\qquad R=12,
\qquad G_{ab}=R_{ab}-\frac12Rg_{ab}=-3g_{ab}.
$$

The [Vacuum Einstein equations](../../../../../vacuum-einstein-equations.md) with a [cosmological constant](../../../../../cosmological-constant.md) are $G_{ab}+\Lambda g_{ab}=0$, and hence

$$
\boxed{\Lambda=3}.
$$

The metric is the contracting flat slicing of [de Sitter spacetime](../../../../../de-sitter-spacetime.md) with curvature radius one.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 309](../../paper-309-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
