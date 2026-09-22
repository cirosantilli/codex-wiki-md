<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $A_1=\operatorname{Div}_1$ and $A_2=\operatorname{Div}_2$, with Euclidean adjoints $A_1^*,A_2^*$ determined by the chosen discretization and boundary conditions. Take the usual positive [total generalized variation](../../../../../../total-generalized-variation.md) weights $\alpha_1,\alpha_2$. Introduce a primal variable $w\in\mathbb R^{n\times2}$ through

$$
-\delta_D(A_1v)=\inf_w\{\delta_D^*(w)-\langle w,A_1v\rangle\},\qquad
\delta_D^*(w)=\alpha_2\sum_i\|w_{i,\cdot}\|_2.
$$

The [support function](../../../../../../support-function.md) of the row-ball product is a sum of row norms. Convex duality gives the equivalent augmented saddle problem

$$
\min_{u,w}\max_v\left\{G(u,w)+\langle K(u,w),v\rangle-\delta_C(v)\right\},
\quad G(u,w)=\frac12\|u-g\|^2+\alpha_2\sum_i\|w_i\|_2,
\quad K(u,w)=A_2^*u-A_1^*w.
$$

The equality follows by dualizing the row-ball constraint. With positive radii, $v=0$ strictly satisfies both row constraints, supplying the finite-dimensional qualification for this splitting. The original feasible dual set is compact and nonempty, and the quadratic primal term is coercive; saddle points exist. The [TGV divergence splitting](../../../../../../tgv-divergence-splitting.md) avoids the difficult projection onto $\{v:v\in C,\ A_1v\in D\}$.

Use the [Chambolle–Pock algorithm](../../../../../../chambolle-pock-algorithm.md). Choose $\tau,\sigma>0$ with $\tau\sigma\|K\|^2<1$; the sufficient bound $\tau\sigma(\|A_2\|^2+\|A_1\|^2)<1$ is convenient. Initialize $u^0,w^0,v^0$ and $\bar u^0=u^0$, $\bar w^0=w^0$. For $k=0,1,\ldots$, compute

$$
\widetilde v=v^k+\sigma(A_2^*\bar u^k-A_1^*\bar w^k),\qquad
\boxed{v_i^{k+1}=\frac{\widetilde v_i}{\max(1,\|\widetilde v_i\|_2/\alpha_1)}},
$$



$$
\boxed{u^{k+1}=\frac{u^k-\tau A_2v^{k+1}+\tau g}{1+\tau}},\qquad
\widetilde w=w^k+\tau A_1v^{k+1},
$$



$$
\boxed{w_i^{k+1}=\begin{cases}
(1-\tau\alpha_2/\|\widetilde w_i\|_2)\widetilde w_i,&\|\widetilde w_i\|_2>\tau\alpha_2,\\
0,&\|\widetilde w_i\|_2\leq\tau\alpha_2,
\end{cases}}
\qquad
\bar u^{k+1}=2u^{k+1}-u^k,\quad\bar w^{k+1}=2w^{k+1}-w^k.
$$

The dual update is a [Euclidean projection onto a convex set](../../../../../../euclidean-projection-onto-a-convex-set.md) onto $C$; the two primal updates are the quadratic [proximal operator](../../../../../../proximal-operator.md) and [radial soft thresholding](../../../../../../radial-soft-thresholding.md). Their signs follow from $K^*v=(A_2v,-A_1v)$. All substeps are closed form, and the standard finite-dimensional primal-dual convergence result applies to this saddle problem with the stated step-size condition. The iterates $v^k$ satisfy $C$; the additional $D$ constraint is enforced through the splitting at convergence, not claimed for every intermediate iterate. If a weight is zero, the corresponding row projection or support-function proximal step is interpreted directly rather than by division by zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
