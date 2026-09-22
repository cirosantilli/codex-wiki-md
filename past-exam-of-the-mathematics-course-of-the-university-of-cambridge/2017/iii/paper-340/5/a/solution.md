<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $D=\nabla$ and use the real pixelwise [inner products](../../../../../../inner-product.md). Let $D^*$ be the [adjoint operator](../../../../../../adjoint-operator.md), defined by $\langle Du,p\rangle=\langle u,D^*p\rangle$. For each nontrivial grid direction its one-dimensional formula is

$$
(D_x^{+*}p^1)_{i,j}=\begin{cases}-p^1_{1,j},&i=1,\\p^1_{i-1,j}-p^1_{i,j},&1<i<N,\\p^1_{N-1,j},&i=N,\end{cases}
$$

with the analogous formula in $j$ for $D_y^{+*}p^2$. Their sum is $D^*p$; unused components $p^1_{N,j}$ and $p^2_{i,N}$ do not contribute. For $N=1$, $D=D^*=0$. If discrete divergence is defined, its sign convention is $\operatorname{div}=-D^*$, as in the [adjoint of a discrete forward gradient](../../../../../../adjoint-of-a-discrete-forward-gradient.md).

Define the [compact](../../../../../../compact-space.md) [convex set](../../../../../../convex-set.md) $P_\lambda=\{p\in X^2:|p_{i,j}|_2\le\lambda\}$ and its image $C=D^*P_\lambda$. The image is [compact](../../../../../../compact-space.md) and [convex](../../../../../../convex-function.md), hence closed, and contains zero. The finite-dimensional Euclidean duality formula $\lambda|a|_2=\max_{|p|_2\le\lambda}a\cdot p$, applied independently at every pixel, gives

$$
\lambda\|Du\|_{2,1}=\max_{p\in P_\lambda}\langle Du,p\rangle=\max_{w\in C}\langle u,w\rangle=\sigma_C(u).
$$

Thus the penalty is the [support function](../../../../../../support-function.md) $\sigma_C$. Its [convex conjugate](../../../../../../convex-conjugate.md) is the [indicator functional of a constraint set](../../../../../../indicator-functional-of-a-constraint-set.md) $\iota_C$, equal to zero on $C$ and infinity elsewhere. For $w\in C$, the conjugate supremum is zero; for $w\notin C$, the separation theorem supplies a direction $u$ with $\langle u,w\rangle>\sigma_C(u)$, and scaling that direction makes the supremum infinite.

The [proximal operator](../../../../../../proximal-operator.md) is $\operatorname{prox}_{\sigma_C}(g)=\arg\min_u\{\sigma_C(u)+\tfrac12\|u-g\|_2^2\}$. It exists uniquely because the objective is [continuous](../../../../../../continuous-function.md), coercive and [strictly convex](../../../../../../strictly-convex-function.md). The [Moreau decomposition](../../../../../../moreau-decomposition.md) for a proper closed [convex function](../../../../../../convex-function.md) gives $\operatorname{prox}_{\sigma_C}(g)+\operatorname{prox}_{\iota_C}(g)=g$. The second term is the [Euclidean projection onto a convex set](../../../../../../euclidean-projection-onto-a-convex-set.md), so the [projection residual for discrete total variation](../../../../../../projection-residual-for-discrete-total-variation.md) is

$$
\boxed{u=g-P_Cg,\qquad C=D^*\{p:|p_{i,j}|_2\le\lambda\}.}
$$

Alternatively, the [variational characterization of convex projection](../../../../../../variational-characterization-of-convex-projection.md) says $w=P_Cg$ exactly when $\langle g-w,z-w\rangle\le0$ for every $z\in C$. Hence $w$ attains the [support function](../../../../../../support-function.md) at $u=g-w$, giving $w\in\partial\sigma_C(u)$ and the same optimality condition. This supplies a direct verification of the [Moreau decomposition](../../../../../../moreau-decomposition.md) step in this instance.

**The printed wording needs “the residual after a projection”, rather than “the projection itself”.** In general this denoising map is not a projection onto any fixed closed [convex set](../../../../../../convex-set.md). A [metric projection onto a closed convex set](../../../../../../euclidean-projection-onto-a-convex-set.md) is idempotent, while denoising a sufficiently large jump twice shrinks it twice. Concretely, for $N=2$ and data with rows $(0,0)$ and $(6\lambda,6\lambda)$, the minimizer has rows $(\lambda,\lambda)$ and $(5\lambda,5\lambda)$. Reapplying the map gives rows $(2\lambda,2\lambda)$ and $(4\lambda,4\lambda)$, so it is not idempotent. These formulas have a global certificate: take $p^1_{1,j}=\lambda$, all other dual entries zero, giving $D^*p$ with rows $(-\lambda,-\lambda)$ and $(\lambda,\lambda)$; it saturates every positive row difference and yields the primal optimality condition. The qualification is therefore not merely a consequence of a restricted two-level ansatz.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
