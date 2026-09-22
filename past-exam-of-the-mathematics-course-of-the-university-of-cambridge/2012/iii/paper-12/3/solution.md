<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take $N$ to be a closed compact [Riemannian manifold](../../../../../riemannian-manifold.md) and use the [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md). Its [Riemannian heat kernel](../../../../../riemannian-heat-kernel.md) $K_N(t,x,y)$ is the integral kernel of $e^{-t\Delta_N}$:

$$
(e^{-t\Delta_N}f)(x)=\int_NK_N(t,x,y)f(y)\,dV(y).
$$

It solves $(\partial_t+\Delta_x)K_N=0$ for $t>0$ and tends to the identity kernel as $t\downarrow0$. For an [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md), the [spectral expansion of the Riemannian heat kernel](../../../../../spectral-expansion-of-the-riemannian-heat-kernel.md) is

$$
K_N(t,x,y)=\sum_j e^{-t\lambda_j}\phi_j(x)\overline{\phi_j(y)}.
$$

The bar is required for a complex basis. With boundary, a specified invariant [boundary condition](../../../../../boundary-condition.md) must also be included in this definition.

For the quotient formula use the covering-space interpretation: $U$ acts freely and properly discontinuously by [Riemannian isometries](../../../../../riemannian-isometry.md). On compact $N$ such a discrete group is finite. Freeness alone, without this covering hypothesis, does not justify the image sum: an infinite dense [subgroup](../../../../../subgroup.md) of circle rotations, for example, acts freely but has no manifold quotient. Positive-dimensional group actions require a different quotient analysis.

For lifts $x,y$ of $\bar x,\bar y\in M$, the [heat kernel on a finite isometric quotient](../../../../../heat-kernel-on-a-finite-isometric-quotient.md) is

$$
\boxed{K_M(t,\bar x,\bar y)=\sum_{u\in U}K_N(t,x,uy).}
$$

Invariance of $K_N$ under simultaneous [Riemannian isometries](../../../../../riemannian-isometry.md) and reindexing the sum show that this is independent of both lifts. A local isometry commutes with the Laplacian, so the sum satisfies the quotient [heat equation](../../../../../heat-equation.md). For its initial condition, integrate over a fundamental domain $F\subset N$ against a lifted function. The terms combine into the integral over all of $N$, whose initial limit is $f(x)$. Uniqueness of the heat evolution proves the formula. **There is no factor $1/|U|$ in this kernel formula.**

On the diagonal the sum is $U$-invariant. Its integral over $F$ is therefore $1/|U|$ times its integral over $N$, giving the [heat trace](../../../../../heat-trace.md)

$$
\boxed{Z_M(t)=\operatorname{Tr}(e^{-t\Delta_M})
=\frac1{|U|}\sum_{u\in U}\int_NK_N(t,x,ux)\,dV(x).}
$$

Thus the normalization factor appears in the trace, not the kernel. Put $F_t(g)=\int_NK_N(t,x,gx)\,dV(x)$. For any finite isometry group $T$, changing variables $x=hy$ proves $F_t(hgh^{-1})=F_t(g)$: it is a [class function](../../../../../class-function.md) on $T$.

For [Gassmann equivalent](../../../../../gassmann-equivalence.md) [subgroups](../../../../../subgroup.md) $U_1,U_2\leq T$, their intersections with each [conjugacy class](../../../../../conjugacy-class.md) have equal size, and their orders are equal. If both act freely, the [heat traces](../../../../../heat-trace.md) of their quotients satisfy

$$
Z_{U_i\backslash N}(t)=\frac1{|U_i|}\sum_{\mathcal C}|U_i\cap\mathcal C|F_t(\mathcal C),
$$

so they agree for every $t>0$. Since $Z_M(t)=\sum_\lambda m(\lambda)e^{-t\lambda}$, equality determines the [spectrum](../../../../../spectrum-functional-analysis.md) with multiplicities: take $t\to\infty$ to recover the smallest [eigenvalue](../../../../../eigenvalue.md) and its multiplicity, subtract that term, and repeat. This proves [Sunada theorem](../../../../../sunada-theorem.md). Equivalently, projection onto $U_i$-invariant functions averages the group action, and the quotient [eigenvalue](../../../../../eigenvalue.md) multiplicity is $|U_i|^{-1}\sum_{u\in U_i}\chi_\lambda(u)$, with $\chi_\lambda$ the [eigenspace](../../../../../eigenspace.md) [character of a representation](../../../../../character-of-a-representation.md). Almost conjugacy equalizes these averages.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
