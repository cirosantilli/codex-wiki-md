<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

A subgroup of the [Möbius group](../../../../../mobius-group.md) $\operatorname{PSL}_2(\mathbb C)$ is a [discrete subgroup](../../../../../discrete-subgroup.md) when the identity is isolated in its induced topology, equivalently every group element is isolated. We prove the compact-set criterion for a [properly discontinuous group action](../../../../../properly-discontinuous-group-action.md): for every compact $K\subset\mathbb H^3$, only finitely many $g\in G$ satisfy $gK\cap K\ne\varnothing$.

Fix an origin $o$ and take $K\subseteq\overline B(o,R)$. If $x\in K$ and $gx\in K$, the triangle inequality and invariance of hyperbolic distance give

$$
d(o,go)\leq d(o,gx)+d(gx,go)=d(o,gx)+d(x,o)\leq2R.
$$

The set of Möbius isometries with $d(o,go)\leq2R$ is compact. To see this explicitly, represent an [isometry](../../../../../isometry.md) by a determinant-one complex matrix and use singular-value decomposition:

$$
g=k_1\begin{pmatrix}e^{s/2}&0\\0&e^{-s/2}\end{pmatrix}k_2,\qquad
k_1,k_2\in\operatorname{SU}(2),\quad s\geq0.
$$

The compact factors fix $o$, and the diagonal factor moves it hyperbolic distance $s$, as seen from the vertical dilation by $e^s$ in upper half-space. Thus the bounded-displacement set is the continuous image of $\operatorname{SU}(2)\times[0,2R]\times\operatorname{SU}(2)$, modulo central signs.

By the allowed closedness fact, its intersection with $G$ is a closed discrete subset of a compact space, hence finite. Otherwise an infinite sequence would accumulate in that intersection, contradicting isolation of its limit point. This proves **every discrete Möbius subgroup acts properly discontinuously on hyperbolic three-space**. Finite stabilizers are allowed; discreteness alone does not imply a free action.

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
