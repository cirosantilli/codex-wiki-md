<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Covariance of the fundamental [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) requires $D_\mu^{f\prime}(g\chi)=gD_\mu^f\chi$ for every column $\chi$. Expanding the left side and cancelling $g\partial_\mu\chi$ gives $(\partial_\mu g)+A'_\mu g=gA_\mu$. Therefore the necessary and sufficient [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md) is

$$
\boxed{A'_\mu=gA_\mu g^{-1}-(\partial_\mu g)g^{-1}.}
$$

In operator notation $D_\mu^{f\prime}=gD_\mu^fg^{-1}$. Expanding its [commutator](../../../../../commutator.md) on an arbitrary column shows $[D_\mu^f,D_\nu^f]\chi=F_{\mu\nu}\chi$: the second derivatives cancel, as do the terms containing a single derivative of $\chi$. Conjugating this identity proves the [gauge field strength](../../../../../gauge-field-strength.md) transformation

$$
\boxed{F'_{\mu\nu}=gF_{\mu\nu}g^{-1}.}
$$

Thus the [gauge field strength](../../../../../gauge-field-strength.md) transforms homogeneously even though the potential has an inhomogeneous derivative term.

For the [adjoint scalar field](../../../../../adjoint-scalar-field.md), write $B_\mu=(\partial_\mu g)g^{-1}$ and $\Phi'=g\Phi g^{-1}$. Differentiating the inverse matrix gives

$$
\partial_\mu\Phi'=g(\partial_\mu\Phi)g^{-1}+[B_\mu,\Phi'],\qquad [A'_\mu,\Phi']=g[A_\mu,\Phi]g^{-1}-[B_\mu,\Phi'].
$$

The extra terms cancel, proving **$D'_\mu\Phi'=g(D_\mu\Phi)g^{-1}$** for the [adjoint covariant derivative](../../../../../adjoint-covariant-derivative.md). Its curvature is obtained by another direct expansion:

$$
\begin{aligned}
[D_\mu,D_\nu]\Phi
&=[\partial_\mu A_\nu-\partial_\nu A_\mu,\Phi]
+[A_\mu,[A_\nu,\Phi]]-[A_\nu,[A_\mu,\Phi]]\\
&=[\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu],\Phi]
=\boxed{[F_{\mu\nu},\Phi]},
\end{aligned}
$$

where the [Jacobi identity](../../../../../jacobi-identity.md) combines the last two terms.

For the equations of motion take compactly supported variations, and assume $e\ne0$, as required by the Lagrangian coefficient. Invariance of the [Killing form](../../../../../killing-form.md) implies

$$
\partial_\mu\kappa(X,Y)=\kappa(D_\mu X,Y)+\kappa(X,D_\mu Y).
$$

Indeed, the two connection terms sum to $\kappa([A_\mu,X],Y)+\kappa(X,[A_\mu,Y])=0$. This is the [gauge-covariant integration by parts](../../../../../gauge-covariant-integration-by-parts.md) identity. The needed variations are

$$
\delta F_{\mu\nu}=D_\mu\delta A_\nu-D_\nu\delta A_\mu,\qquad
\delta(D_\mu\Phi)=D_\mu\delta\Phi+[\delta A_\mu,\Phi].
$$

Antisymmetry of the [gauge field strength](../../../../../gauge-field-strength.md) combines its two variation terms. Applying [gauge-covariant integration by parts](../../../../../gauge-covariant-integration-by-parts.md) to the action $S=\int\mathcal L\,d^4x$ gives

$$
\begin{aligned}
\delta S=\int d^4x\biggl\{&-\frac1{e^2}\kappa(\delta A_\nu,D_\mu F^{\mu\nu})
-\kappa(\delta A_\nu,[\Phi,D^\nu\Phi])\\
&+\kappa(\delta\Phi,D_\mu D^\mu\Phi)\biggr\}.
\end{aligned}
$$

Here $\kappa([\delta A_\nu,\Phi],D^\nu\Phi)=\kappa(\delta A_\nu,[\Phi,D^\nu\Phi])$ fixes the sign of the scalar current. Since the [Killing form](../../../../../killing-form.md) is nondegenerate on a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md), independent variations give the coupled [Yang-Mills equations](../../../../../yang-mills-equations.md) and scalar equation

$$
\boxed{D_\mu F^{\mu\nu}+e^2[\Phi,D^\nu\Phi]=0,\qquad D_\mu D^\mu\Phi=0.}
$$

Equivalently, $D_\mu F^{\mu\nu}=e^2[D^\nu\Phi,\Phi]$. These signs use the stated [Minkowski metric](../../../../../minkowski-metric.md), with upper spatial derivatives $D^i=-D_i$.

It remains to verify every equation for the static [Bogomolny equations](../../../../../bogomolny-equations.md). The hypotheses imply $F_{0i}=0$ and $D_0\Phi=0$, so the temporal gauge equation is automatically zero. The [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md)

$$
D_iF_{jk}+D_jF_{ki}+D_kF_{ij}=0
$$

follows, for example, from the [Jacobi identity](../../../../../jacobi-identity.md) for the fundamental [gauge covariant derivatives](../../../../../gauge-covariant-derivative.md), using their commutator $F_{ij}$. Define $B_i=\tfrac12\varepsilon_{ijk}F_{jk}$. Contracting the [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md) with $\varepsilon_{ijk}$ gives $D_iB_i=0$. The [Bogomolny equations](../../../../../bogomolny-equations.md) say $B_i=eD_i\Phi$, so $e\ne0$ implies $D_iD_i\Phi=0$. In the static configuration $D_\mu D^\mu\Phi=-D_iD_i\Phi$, verifying the scalar equation.

For the spatial gauge equation, use $F^{ij}=F_{ij}$ and $D^j\Phi=-D_j\Phi$. The [Bogomolny equations](../../../../../bogomolny-equations.md), the curvature commutator proved above, and the [contraction of two Levi-Civita symbols](../../../../../contraction-of-two-levi-civita-symbols.md) give

$$
\begin{aligned}
D_iF_{ij}&=e\varepsilon_{ijk}D_iD_k\Phi
=\frac e2\varepsilon_{ijk}[D_i,D_k]\Phi
=\frac e2\varepsilon_{ijk}[F_{ik},\Phi]\\
&=\frac{e^2}2\varepsilon_{ijk}\varepsilon_{ik\ell}[D_\ell\Phi,\Phi]
=-e^2[D_j\Phi,\Phi]=e^2[\Phi,D_j\Phi],
\end{aligned}
$$

since $\varepsilon_{ijk}\varepsilon_{ik\ell}=-2\delta_{j\ell}$. This is exactly $D_iF^{ij}+e^2[\Phi,D^j\Phi]=0$. Thus **the static first-order Bogomolny system satisfies all four gauge equations and the scalar equation**, with no extra ansatz or boundary assumption needed for this local implication. This is the mechanism by which [Bogomolny monopole equations imply Yang-Mills-Higgs equations](../../../../../bogomolny-monopole-equations-imply-yang-mills-higgs-equations.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
