<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work over $\mathbb Q$. A closed connected [orientable surface](../../../../../orientable-surface.md) of [genus](../../../../../genus-of-a-surface.md) $g$ has [Betti numbers](../../../../../betti-number.md) $(1,2g,1)$; the [circle](../../../../../circle.md) has Betti numbers $(1,1)$. The [Künneth theorem](../../../../../kunneth-theorem.md) therefore gives

$$
(b_0,b_1,b_2,b_3)(S^1\times\Sigma_g)=(1,2g+1,2g+1,1).
$$

We use the following precise consequence of the [Morse handle-attachment theorem](../../../../../morse-handle-attachment-theorem.md): a closed [manifold](../../../../../topological-manifold.md) with a [Morse function](../../../../../morse-function.md) has the [homotopy type](../../../../../homotopy-type.md) of a finite [CW complex](../../../../../cw-complex.md) with one index-$j$ cell for each index-$j$ [critical point](../../../../../critical-point.md). Its degree-$j$ rational [cellular chain group](../../../../../cellular-chain-group.md) has dimension $c_j$, so its [homology](../../../../../homology-split.md) has dimension at most $c_j$. Consequently $c_j\geq b_j$, the weak [Morse inequalities](../../../../../morse-inequalities.md). Summing yields

$$
\boxed{\#\operatorname{Crit}(f)\geq1+(2g+1)+(2g+1)+1=4g+4.}
$$

This counts every critical point, regardless of whether some critical values coincide.

To attain the bound, construct a surface [Morse function](../../../../../morse-function.md) $h:\Sigma_g\to\mathbb R$ from the standard orientable [handle decomposition](../../../../../handle-decomposition.md): start with a disk, attach $2g$ orientable bands in the usual paired pattern forming the genus-$g$ surface with one boundary component, and cap that boundary with a disk. Give the first disk a minimum, each band one saddle with local form $-x^2+y^2$, and the final cap a maximum. Regular collar coordinates join successive levels without additional critical points. This constructs $h$ with counts $(1,2g,1)$.

On the product take

$$
F(\theta,x)=h(x)+\delta\cos\theta,\qquad\delta>0.
$$

Its [critical points](../../../../../critical-point.md) are exactly the pairs of a critical point of $h$ with $\theta=0,\pi$. The [Hessian matrix](../../../../../hessian-matrix.md) is block diagonal, with surface block $\operatorname{Hess}h$ and circle entry $-\delta\cos\theta$. It is nonsingular and its [Morse index](../../../../../morse-index.md) is the sum of the two factor indices. Thus this [product of Morse functions](../../../../../product-of-morse-functions.md) has counts

$$
(c_0,c_1,c_2,c_3)=(1,2g+1,2g+1,1),
$$

and exactly **$4g+4$ critical points**. If distinct critical values are desired, choose $\delta$ outside the finite set producing collisions after first choosing distinct critical values for $h$. The [minimal Morse critical count on a circle times an orientable surface](../../../../../minimal-morse-critical-count-on-a-circle-times-an-orientable-surface.md) is therefore attained for every $g\geq0$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
