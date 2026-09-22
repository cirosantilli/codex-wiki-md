<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

At a point $[X]\in\mathbf P^n$, the [complex tautological line bundle](../../../../../complex-tautological-line-bundle.md) has fiber $\mathbb CX\subseteq\mathbb C^{n+1}$. The [hyperplane line bundle](../../../../../hyperplane-line-bundle.md) is its dual, $[H]=\mathcal O(1)$, and $\mathcal O(m)=\mathcal O(1)^{\otimes m}$. On $U_i=\{X_i\ne0\}$ let $t_i=X/X_i$ be the tautological frame and $e_i$ its dual. On overlaps $e_j=(X_j/X_i)e_i$. The [sheaf of holomorphic sections of a vector bundle](../../../../../sheaf-of-holomorphic-sections-of-a-vector-bundle.md) of this dual bundle is the sheaf $\mathcal O_{\mathbf P^n}(1)$.

If a nonzero linear form $\ell$ cuts out the [projective hyperplane](../../../../../projective-hyperplane.md) $H$, it gives a [holomorphic section](../../../../../holomorphic-section.md) $s_H$ of $\mathcal O(1)$ with a simple zero along $H$. Dividing a local section $s$ by $s_H$ gives a [meromorphic function](../../../../../meromorphic-function.md) with no poles away from $H$ and at most a simple pole on $H$. Conversely multiplication by $s_H$ turns such a function into a [holomorphic section](../../../../../holomorphic-section.md). These mutually inverse local constructions agree on overlaps and prove the [holomorphic line bundle associated to a divisor](../../../../../holomorphic-line-bundle-associated-to-a-divisor.md) identification

$$
\boxed{\mathcal O(1)\cong\mathcal O(H).}
$$

The [nonnegative hyperplane twist cohomology by restriction](../../../../../nonnegative-hyperplane-twist-cohomology-by-restriction.md) calculation gives

$$
\boxed{h^r(\mathbf P^n,\mathcal O(m))=\begin{cases}\binom{n+m}{n},&r=0,\\0,&r>0.\end{cases}}
$$

To derive it from the permitted vanishing, use the [hyperplane exact sequence for twisting sheaves](../../../../../hyperplane-exact-sequence-for-twisting-sheaves.md)

$$
0\longrightarrow\mathcal O_{\mathbf P^n}(m-1)\xrightarrow{\,s_H\,}\mathcal O_{\mathbf P^n}(m)
\longrightarrow i_*\mathcal O_H(m)\longrightarrow0,
$$

where $i:H\hookrightarrow\mathbf P^n$ and $H\cong\mathbf P^{n-1}$. Local multiplication by a defining equation is injective, and restriction gives exactly its cokernel. Induct on $n$, starting from a point, and then on $m$. For $m=0$, higher [sheaf cohomology](../../../../../sheaf-cohomology.md) vanishes by assumption and global [holomorphic functions](../../../../../holomorphic-function.md) are constant by compactness and the maximum principle. For $m>0$, the [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md), the inductive vanishing for $\mathcal O(m-1)$ and the dimension induction on $H$ give vanishing in every positive degree and

$$
h^0(\mathbf P^n,\mathcal O(m))-h^0(\mathbf P^n,\mathcal O(m-1))=\binom{n-1+m}{n-1}.
$$

Summing this recurrence gives $\binom{n+m}{n}$. Homogeneous degree-$m$ monomials give that many independent sections, so they form a basis. The printed extra equality to zero cannot hold in degree zero, already because $h^0(\mathbf P^n,\mathcal O)=1$; the boxed calculation gives the intended dimensions.

For the [differential of the projective quotient map](../../../../../differential-of-the-projective-quotient-map.md), the [differential of a smooth map](../../../../../differential-of-a-smooth-map.md) is computed by applying a tangent vector to coordinate functions. Since $x_j=X_j/X_0$,

$$
\frac{\partial x_j}{\partial X_i}=\frac{\delta_{ij}}{a_0}\quad(i>0),\qquad
\frac{\partial x_j}{\partial X_0}=-\frac{a_j}{a_0^2}.
$$

Thus

$$
\boxed{\pi_*\left(\frac\partial{\partial X_i}\right)=\frac1{a_0}\frac\partial{\partial x_i}\ (i>0),\qquad
\pi_*\left(\frac\partial{\partial X_0}\right)=-\sum_{j=1}^n\frac{a_j}{a_0^2}\frac\partial{\partial x_j}.}
$$

Under replacing $X$ by $\lambda X$, $d\pi$ on a constant ambient tangent vector scales by $\lambda^{-1}$, while a homogeneous linear form $L$ scales by $\lambda$. Therefore $d\pi_X(L(X)\partial_{X_j})$ is independent of the representative. Its chart coefficients are holomorphic, so it is a global [holomorphic vector field](../../../../../holomorphic-vector-field.md). The radial [Euler vector field](../../../../../euler-vector-field.md) lies in the kernel of $d\pi$, either from the same formulas or because it differentiates a scaling orbit. Hence

$$
\boxed{\pi_*\left(\sum_{i=0}^nX_i\partial_{X_i}\right)=0.}
$$

Describe the [Euler sequence on complex projective space](../../../../../euler-sequence-on-complex-projective-space.md) fiberwise as well as in coordinates. At a line $\ell=\mathbb CX$, the middle bundle has fiber $\operatorname{Hom}(\ell,\mathbb C^{n+1})$ and the [holomorphic tangent bundle](../../../../../holomorphic-tangent-bundle.md) has fiber $\operatorname{Hom}(\ell,\mathbb C^{n+1}/\ell)$. Send a homomorphism to its composition with the quotient. The map from $\mathcal O$ sends a scalar to that scalar times the inclusion $\ell\hookrightarrow\mathbb C^{n+1}$. In homogeneous notation these maps are

$$
f\longmapsto(fX_0,\ldots,fX_n),\qquad
(s_0,\ldots,s_n)\longmapsto d\pi_X\left(\sum_js_j(X)\partial_{X_j}\right).
$$

A local section of $\mathcal O(1)$ is a local degree-one homogeneous function on the punctured cone, so the second expression is representative-independent. Quotienting is surjective, and its kernel consists exactly of scalar inclusion maps. This proves the short exact sequence of [locally free sheaves](../../../../../locally-free-sheaf.md)

$$
\boxed{0\to\mathcal O\to\mathcal O(1)^{\oplus(n+1)}\to\mathcal O(T')\to0.}
$$

Since it is locally split, dualizing and tensoring by $\mathcal O(1)$ preserves exactness and gives the [cotangent Euler sequence in homogeneous coordinates](../../../../../cotangent-euler-sequence-in-homogeneous-coordinates.md)

$$
0\to\Omega^1(1)\to\mathcal O^{\oplus(n+1)}\xrightarrow{(c_i)\mapsto\sum_i c_iX_i}\mathcal O(1)\to0.
$$

On global sections the last map identifies $\mathbb C^{n+1}$ with the basis of linear forms in $H^0(\mathcal O(1))$. Its kernel is zero. This proves the [vanishing of global sections of the once-twisted projective cotangent bundle](../../../../../vanishing-of-global-sections-of-the-once-twisted-projective-cotangent-bundle.md); left exactness gives **$\boxed{h^0(\mathbf P^n,\Omega^1(1))=0}$**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
