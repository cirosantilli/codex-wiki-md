<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\Gamma_0=\Delta(7,7,7)$ be the orientation-preserving [hyperbolic triangle group](../../../../../hyperbolic-triangle-group.md), acting on the [hyperbolic plane](../../../../../hyperbolic-plane.md) with presentation

$$
\Gamma_0=\langle a,b,c:a^7=b^7=c^7=abc=1\rangle.
$$

Its quotient is a topological [sphere](../../../../../sphere.md) with three cone points of order seven. Define the surjective [group homomorphism](../../../../../group-homomorphism.md)

$$
\phi:\Gamma_0\longrightarrow T,\qquad
\phi(a)=A,\quad\phi(b)=B,\quad\phi(c)=(AB)^{-1}.
$$

The stated order conditions make this well defined, and the generation hypothesis makes it surjective. Set $K=\ker\phi$. Every finite-order element of a [hyperbolic triangle group](../../../../../hyperbolic-triangle-group.md) is conjugate to a power of a cone-point generator. None of its nontrivial such powers lies in $K$, since all three images have order seven. Therefore $K$ is torsion free, and $X=K\backslash\mathbb H^2$ is a closed oriented [hyperbolic surface](../../../../../hyperbolic-surface.md) carrying an isometric action of $T=\Gamma_0/K$.

The [orbifold Euler characteristic](../../../../../orbifold-euler-characteristic.md) of the base is

$$
\chi_{\mathrm{orb}}=2-3\left(1-\frac17\right)=-\frac47.
$$

The covering degree is $168$, so $\chi(X)=168(-4/7)=-96$ and $X$ has genus $49$. The subgroups have order $|U_i|=168/7=24$. Point stabilizers for the $T$ action are trivial or cyclic of order seven. Since seven does not divide $24$, each $U_i$ acts freely. Thus

$$
S_i=U_i\backslash X=\phi^{-1}(U_i)\backslash\mathbb H^2
$$

are smooth closed [hyperbolic surfaces](../../../../../hyperbolic-surface.md), and

$$
\boxed{\chi(S_i)=\frac{-96}{24}=-4,\qquad g(S_i)=3.}
$$

Equivalently, each $S_i$ is a seven-sheeted orbifold cover of the base with three branch values, and the [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) gives the same genus.

[Gassmann equivalence](../../../../../gassmann-equivalence.md) means that $U_1,U_2$ meet each [conjugacy class](../../../../../conjugacy-class.md) of $T$ in the same number of elements. To prove isospectrality directly, let $E_\lambda(X)$ be a [Laplacian eigenfunction](../../../../../laplacian-eigenfunction.md) space on $X$, viewed as a representation of $T$. Pullback identifies $E_\lambda(S_i)$ with its $U_i$-invariant subspace. Averaging over $U_i$ is the projection onto this subspace, and hence

$$
\dim E_\lambda(S_i)=\frac1{|U_i|}\sum_{u\in U_i}\operatorname{tr}\big(u\mid E_\lambda(X)\big).
$$

The [character of a representation](../../../../../character-of-a-representation.md) in this sum is constant on [conjugacy classes](../../../../../conjugacy-class.md). The sums are equal by [Gassmann equivalence](../../../../../gassmann-equivalence.md), so the [eigenvalues](../../../../../eigenvalue.md) and their multiplicities agree. This is the mechanism of the [Sunada theorem](../../../../../sunada-theorem.md). **The constructed genus-three hyperbolic surfaces are isospectral.**

Nonconjugacy of $U_1,U_2$ in $T$ does not prove nonisometry. For example, an [isometry](../../../../../isometry.md) of $X$ outside the given subgroup $T$ might conjugate $U_1$ to $U_2$ and descend to an [isometry](../../../../../isometry.md) of the quotients. More generally, an [isometry](../../../../../isometry.md) between the quotients lifts to an [isometry](../../../../../isometry.md) of $\mathbb H^2$ conjugating the two groups $\phi^{-1}(U_i)$; there is no requirement that this lift come from an element of $T$. Additional symmetries of the three-cone-point construction are a possible source of this coincidence.

One can prevent this by modifying the common metric, while keeping the $T$ action isometric. Here is a geometric way to make that step precise. On the regular part of the base orbifold $O=\Gamma_0\backslash\mathbb H^2$, choose a sufficiently small smooth [conformal rescaling of a Riemannian metric](../../../../../conformal-rescaling-of-a-riemannian-metric.md) of its metric whose local geometry distinguishes base points and local directions. One may use a generic smooth conformal factor with separate curvature features on a countable collection of small disks. Let these disks approach the cone points, with amplitudes decaying sufficiently rapidly that the lifted conformal factor and all its derivatives vanish at their centres. This gives smooth metrics on the covering surface, without retaining an open homogeneous region near a cone point. The purpose is to ensure that a local [isometry](../../../../../isometry.md) in the regular part covering a quotient is the identity on the base: the curvature features identify its base point and local frame. Pull the metric back to $X$ and then descend it to both $S_i$. The only points with the cone-point rotational symmetry in their metric germs are the lifts of the cone points; the perturbation removes such symmetries in the regular part. Any quotient isometry must therefore preserve this finite distinguished set.

If the perturbed quotients were isometric, their local maps on the dense regular part would preserve the projection to $O$. They would therefore give equivalent connected covers of the punctured base; the correspondence between connected [covering spaces](../../../../../covering-space.md) and subgroups would conjugate $\phi^{-1}(U_1)$ to $\phi^{-1}(U_2)$ inside $\Gamma_0$. Applying $\phi$ would conjugate $U_1,U_2$ inside $T$, contrary to hypothesis. Thus the perturbed quotients are nonisometric. The same averaging argument still proves isospectrality, because it requires a common $T$-invariant [Riemannian metric](../../../../../riemannian-metric.md), not constant curvature. The [genus](../../../../../genus-of-a-surface.md) remains three.

**This last step produces nonisometric isospectral metrics of variable curvature on genus-three surfaces.** An oriented metric defines a [Riemann surface](../../../../../riemann-surfaces.md) through its conformal structure; using a conformal perturbation even preserves the original conformal structures. If “Riemann surface” means specifically its canonical curvature $-1$ metric, the last step should instead be described as producing Riemannian surfaces. The $\Delta(7,7,7)$ orbifold has no hyperbolic deformation parameters: uniformizing the perturbed metrics does not preserve their [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) spectra, and cannot be used to claim nonisometric hyperbolic examples from this argument.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 117](../../paper-117-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
