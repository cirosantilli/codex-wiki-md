<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a differentiable [convex function](../../../../../../convex-function.md) $F$ with $L$-[Lipschitz gradient](../../../../../../lipschitz-gradient.md) and a proper lower-semicontinuous [convex function](../../../../../../convex-function.md) $H$, the [proximal gradient method](../../../../../../proximal-gradient-method.md) is

$$
\boxed{z^{k+1}=\operatorname{prox}_{\tau H}(z^k-\tau\nabla F(z^k)),\qquad0<\tau\le1/L.}
$$

The [proximal operator](../../../../../../proximal-operator.md) is $\operatorname{prox}_{\tau H}(v)=\arg\min_z\{H(z)+\|z-v\|^2/(2\tau)\}$. To obtain an explicit iteration for [discrete isotropic total variation](../../../../../../discrete-isotropic-total-variation.md), let $D=\nabla$ with the printed zero boundary differences and

$$
\mathcal P=\{p\in X\times X:|p_{ij}|_2\le1\text{ for every }i,j\}.
$$

The dual is minimization of $F(p)=\tfrac12\|g-D^*p\|_2^2$ over $\mathcal P$, and the primal minimizer is $u_*=g-D^*p_*$. Here $D^*=-\operatorname{div}$ must be the exact [adjoint operator](../../../../../../adjoint-operator.md) of these differences. For example,

$$
((D_x^+)^*p^1)_{ij}=\begin{cases}
-p^1_{1j},&i=1<N,\\
p^1_{i-1,j}-p^1_{ij},&1<i<N,\\
p^1_{N-1,j},&i=N>1,
\end{cases}
$$

with the analogous formula in $j$ for $(D_y^+)^*$; for $N=1$ both operators are zero. Equivalently use $p^1_{0j}=p^1_{Nj}=p^2_{i0}=p^2_{iN}=0$ in the backward-difference expression, ignoring unused edge components.

The [gradient](../../../../../../gradient.md) of the dual objective is $D(D^*p-g)$, with Lipschitz constant $\|D\|^2\le8$. Taking $H$ to be the [indicator functional of a constraint set](../../../../../../indicator-functional-of-a-constraint-set.md) makes its [proximal operator](../../../../../../proximal-operator.md) the [Euclidean projection onto a convex set](../../../../../../euclidean-projection-onto-a-convex-set.md). Thus a valid explicit algorithm is

$$
v^k=p^k+\tau D(g-D^*p^k),\qquad
\boxed{p^{k+1}_{ij}=\frac{v^k_{ij}}{\max(1,|v^k_{ij}|_2)},\quad u^{k+1}=g-D^*p^{k+1},\quad0<\tau\le\tfrac18.}
$$

The bound follows by summing $(a-b)^2\le2a^2+2b^2$ over grid differences. Finite-dimensional [proximal gradient method](../../../../../../proximal-gradient-method.md) convergence gives a dual minimizer and convergence of the recovered $u^k$ to the unique primal minimizer. Projection is pointwise in the dual; applying pointwise [soft thresholding](../../../../../../soft-thresholding.md) directly to $Du$ would not compute the primal TV [proximal operator](../../../../../../proximal-operator.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
