<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $d_i(u)=((G^{(1)}u)_i,(G^{(2)}u)_i)$. The image penalty is [discrete isotropic total variation](../../../../../../discrete-isotropic-total-variation.md) $\sum_i\|d_i(u)\|_2$; the fidelity term is the [L1 norm](../../../../../../l1-norm.md) $\|u-f\|_1$. Introduce scalars $v_i,t_i$ and minimize the linear objective

$$
\boxed{\sum_{i=1}^n v_i+\lambda\sum_{i=1}^n t_i}
$$

subject to the following affine residuals being cone-feasible:

$$
\boxed{\begin{aligned}
v_i-u_i+f_i&\geq0,\\
v_i+u_i-f_i&\geq0,\\
u_i&\geq0,\qquad 1-u_i\geq0,\\
(t_i,(G^{(1)}u)_i,(G^{(2)}u)_i)&\in\mathcal L_3,
\qquad i=1,\ldots,n,
\end{aligned}}
$$

where $\mathcal L_3=\{(t,a,b):t\geq\sqrt{a^2+b^2}\}$ is the [Lorentz cone](../../../../../../second-order-cone.md). Every component displayed is affine in $(u,v,t)$, so stacking them gives exactly the requested $Ax-b\in K$ form, with

$$
\boxed{K=\mathbb R_+^{4n}\times\mathcal L_3^n.}
$$

The first two inequalities imply $v_i\geq|u_i-f_i|$, so separate nonnegativity constraints for $v_i$ are unnecessary. The cone constraints imply $t_i\geq\|d_i(u)\|_2$. Every lifted feasible objective bounds the original objective from above; choosing $v_i=|u_i-f_i|$ and $t_i=\|d_i(u)\|_2$ gives equality. Since both objective weights are positive, an optimum uses these tight values. Thus **the lift is an exact [second-order cone program](../../../../../../second-order-cone-programming.md) for [box-constrained TV-L1 denoising](../../../../../../box-constrained-tv-l1-denoising.md).**

The product cone is proper, closed, convex and self-dual. The stacked $A$ has full column rank: the box rows recover $u$, the fidelity rows then recover $v$, and the first coordinates of the Lorentz blocks recover $t$. Strict feasibility is also explicit: choose $u_i=1/2$, then take $v_i>|u_i-f_i|$ and $t_i>\|d_i(u)\|_2$.

For generic cone slack $(r,q)$, a canonical barrier is

$$
\boxed{F_K(r,q)=-\sum_{j=1}^{4n}\log r_j
-\sum_{i=1}^n\log(q_{i0}^2-q_{i1}^2-q_{i2}^2),}
$$

on $r_j>0$ and $q_{i0}>\sqrt{q_{i1}^2+q_{i2}^2}$. The positive sheet condition matters: positivity of the quadratic expression alone would also include the wrong Lorentz nappe.

Composing the barrier with the affine residual map gives

$$
\boxed{\begin{aligned}
\Phi(u,v,t)={}&-\sum_i\bigl[
\log(v_i-u_i+f_i)+\log(v_i+u_i-f_i)
+\log u_i+\log(1-u_i)\bigr]\\
&-\sum_i\log\!\left[t_i^2-(G^{(1)}u)_i^2-(G^{(2)}u)_i^2\right].
\end{aligned}}
$$

Its domain includes the strict inequalities above. Each orthant coordinate contributes one to the [self-concordant barrier](../../../../../../self-concordant-barrier.md) parameter and each Lorentz block contributes two. Therefore the product-cone [logarithmically homogeneous barrier](../../../../../../logarithmically-homogeneous-barrier.md) has

$$
\boxed{\nu=4n+2n=6n.}
$$

The affine composition $\Phi$ is the barrier used in the primal variables; it need not itself be logarithmically homogeneous in $(u,v,t)$ because the image data and box offsets are affine constants.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
