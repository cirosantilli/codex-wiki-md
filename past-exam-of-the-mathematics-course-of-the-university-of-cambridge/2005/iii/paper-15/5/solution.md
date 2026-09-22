<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the standard boundaryless-manifold convention, so $M$ is a [closed manifold](../../../../../closed-manifold.md). Its orientation and [Riemannian metric](../../../../../riemannian-metric.md) determine a unique positive [Riemannian volume form](../../../../../riemannian-volume-form.md) $\mu_g$ taking value one on every positively oriented [orthonormal frame](../../../../../orthonormal-frame-in-spacetime.md). In an [oriented atlas](../../../../../oriented-atlas.md) it is

$$
\mu_g=\sqrt{\det(g_{ij})}\,dx^1\wedge\cdots\wedge dx^n.
$$

For the [coordinate invariance of the Riemannian volume form](../../../../../coordinate-invariance-of-the-riemannian-volume-form.md), on an overlap put $J=\partial y/\partial x$. Then $g_x=J^Tg_yJ$ and $dy^1\wedge\cdots\wedge dy^n=(\det J)dx^1\wedge\cdots\wedge dx^n$. The oriented transition has $\det J>0$, so the square root of the metric determinant and the coordinate volume transform together. The local forms therefore agree and define $\mu_g$ globally.

For real $r$-forms the [Hodge star operator](../../../../../hodge-star-operator.md) is defined by

$$
\alpha\wedge*\beta=\langle\alpha,\beta\rangle_g\mu_g.
$$

The pointwise wedge pairing is [nondegenerate](../../../../../nondegenerate-bilinear-form.md), so this uniquely defines a smooth map $*:\Omega^r(M)\to\Omega^{n-r}(M)$. On an oriented orthonormal coframe, it sends a basis wedge to the signed complementary wedge. Applying it twice gives

$$
*^2\alpha=(-1)^{r(n-r)}\alpha.
$$

For [Hodge star eigenvalues on graded differential forms](../../../../../hodge-star-eigenvalues-on-graded-differential-forms.md), extend $*$ complex-linearly to the direct sum of all form degrees. This interpretation matters: on a fixed degree it is an [endomorphism](../../../../../endomorphism.md) only in middle degree. In positive odd dimension, $r(n-r)$ is even for every $r$, so $*^2=I$ and only $\pm1$ can occur. Both occur, with eigenforms $1+\mu_g$ and $1-\mu_g$.

In positive even dimension, $*^2$ is $+I$ on even-degree forms and $-I$ on odd-degree forms. Hence $*^4=I$ and the only possible [eigenvalues](../../../../../eigenvalue.md) are $\pm1,\pm i$. The first two occur as above. For the latter, choose a smooth local [orthonormal frame](../../../../../orthonormal-frame-in-spacetime.md) and multiply its first dual [differential one-form](../../../../../one-form.md) by a nonzero [smooth bump function](../../../../../smooth-bump-function.md) supported in the chart. This gives a form $\eta$ for which $\eta$ and $*\eta$ are independent. For $\lambda=\pm i$,

$$
*\bigl(\eta+\lambda^{-1}*\eta\bigr)
=\lambda\bigl(\eta+\lambda^{-1}*\eta\bigr).
$$

Thus all four occur. Consequently, for $n\geq1$,

$$
\boxed{\operatorname{Spec}(*)=
\begin{cases}
\{1,-1\},&n\text{ odd},\\
\{1,-1,i,-i\},&n\text{ even}.
\end{cases}}
$$

On degree $m$ in dimension $2m$, the [Hodge star](../../../../../hodge-star-operator.md) has [eigenvalues](../../../../../eigenvalue.md) $\pm1$ for even $m$ and $\pm i$ for odd $m$; signed complementary middle-degree wedges show both occur for $m\geq1$. In zero dimensions it is multiplication by the signed unit volume at each point, so only the signs actually present occur.

For [Hodge integration by parts in arbitrary degree](../../../../../hodge-integration-by-parts-in-arbitrary-degree.md), let $\alpha\in\Omega^{r-1}(M)$ and $\beta\in\Omega^r(M)$. The [graded Leibniz rule](../../../../../graded-leibniz-rule.md) and [Stokes theorem](../../../../../stokes-theorem.md) on the closed manifold give

$$
0=\int_M d(\alpha\wedge*\beta)
=\int_Md\alpha\wedge*\beta+(-1)^{r-1}\int_M\alpha\wedge d*\beta.
$$

Using the given [codifferential](../../../../../codifferential.md) and the square of the [Hodge star](../../../../../hodge-star-operator.md),

$$
*\delta\beta
=(-1)^{n(r+1)+1+(n-r+1)(r-1)}d*\beta
=(-1)^r d*\beta.
$$

Therefore

$$
\boxed{\langle d\alpha,\beta\rangle_{L^2}
=\int_Md\alpha\wedge*\beta
=\int_M\alpha\wedge*\delta\beta
=\langle\alpha,\delta\beta\rangle_{L^2}},
$$

which proves that $\delta$ is the [formal adjoint](../../../../../formal-adjoint.md) of $d$. The complex version inserts conjugation in the usual [Hermitian inner product](../../../../../hermitian-form.md).

The [Hodge decomposition theorem](../../../../../hodge-decomposition-theorem.md) gives an $L^2$-orthogonal decomposition

$$
\Omega^k(M)=\mathcal H^k(M)\oplus d\Omega^{k-1}(M)\oplus\delta\Omega^{k+1}(M),
$$

where $\mathcal H^k(M)=\ker\Delta$ is finite dimensional and consists of the [harmonic differential forms](../../../../../harmonic-differential-form.md). Each [de Rham cohomology](../../../../../de-rham-cohomology.md) class has a unique harmonic representative. Equivalently, with harmonic projection $P_{\mathcal H}$ there is a smooth [Green operator of the Hodge Laplacian](../../../../../green-operator-of-the-hodge-laplacian.md) $G$ satisfying $\Delta G=G\Delta=I-P_{\mathcal H}$.

The [solvability condition for the Hodge Poisson equation](../../../../../solvability-condition-for-the-hodge-poisson-equation.md) is

$$
\boxed{\Delta\alpha=\beta\text{ is solvable}\quad\Longleftrightarrow\quad
\langle\beta,h\rangle_{L^2}=0\text{ for every }h\in\mathcal H^k(M)}.
$$

Necessity follows from $\langle\Delta\alpha,h\rangle=\langle\alpha,\Delta h\rangle=0$. Conversely the orthogonality condition gives $P_{\mathcal H}\beta=0$, so $\alpha_0=G\beta$ solves the [Poisson equation for differential forms](../../../../../poisson-equation-for-differential-forms.md).

The [nonnegativity of the Hodge Laplacian](../../../../../nonnegativity-of-the-hodge-laplacian.md) identity

$$
\langle\Delta\eta,\eta\rangle_{L^2}=\|d\eta\|_{L^2}^2+\|\delta\eta\|_{L^2}^2
$$

identifies its kernel with closed and coclosed forms. Thus the [affine space of solutions of the Hodge Poisson equation](../../../../../affine-space-of-solutions-of-the-hodge-poisson-equation.md) is

$$
\boxed{\alpha_0+\mathcal H^k(M)}.
$$

For completeness, if a closed form is decomposed as $\omega=h+d\xi+\delta\zeta$, then $d\delta\zeta=0$, and $\|\delta\zeta\|^2=\langle\zeta,d\delta\zeta\rangle=0$. Hence its cohomology class is represented by $h$. An exact harmonic form $h=d\xi$ must vanish, since $\|h\|^2=\langle\delta h,\xi\rangle=0$. This proves the canonical [isomorphism](../../../../../isomorphism.md) $\mathcal H^k(M)\cong H^k_{\mathrm{dR}}(M)$, so the solution set is an [affine space](../../../../../affine-space.md) whose translation [vector space](../../../../../vector-space-split.md) is isomorphic to the requested [de Rham cohomology](../../../../../de-rham-cohomology.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
