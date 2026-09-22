# Paper 52

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper52.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper52.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For a finite-dimensional [Lie algebra](../../../lie-algebra.md), the [Killing form](../../../lie-algebra.md#killing-form) is defined using the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) on the algebra itself, rather than the given [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) $d$:

$$
\kappa(X,Y)=\operatorname{Tr}_{\mathcal L}(\operatorname{ad}_X\operatorname{ad}_Y),\qquad \operatorname{ad}_X(Z)=[X,Z].
$$

The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives $\operatorname{ad}_{[X,Y]}=[\operatorname{ad}_X,\operatorname{ad}_Y]$. Using the [cyclic property of the trace](../../../linear-algebra.md#cyclic-property-of-the-trace),

$$
\begin{aligned}
\kappa([X,Y],Z)&=\operatorname{Tr}(\operatorname{ad}_X\operatorname{ad}_Y\operatorname{ad}_Z-\operatorname{ad}_Y\operatorname{ad}_X\operatorname{ad}_Z)\\
&=\operatorname{Tr}(\operatorname{ad}_X[\operatorname{ad}_Y,\operatorname{ad}_Z])=\kappa(X,[Y,Z]).
\end{aligned}
$$

The same trace identity makes the [Killing form](../../../lie-algebra.md#killing-form) symmetric. For a [basis](../../../vector-space.md#basis) $(t_a)$, the lowered [structure constants of a Lie algebra](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) are $c_{abc}=\kappa([t_a,t_b],t_c)$. Antisymmetry of the [Lie bracket](../../../lie-algebra.md#lie-bracket) gives $c_{abc}=-c_{bac}$, while invariance gives $c_{abc}=\kappa(t_a,[t_b,t_c])=-c_{acb}$. The two adjacent transpositions generate every permutation, proving the [antisymmetry of Killing-lowered structure constants](../../../lie-algebra.md#antisymmetry-of-killing-lowered-structure-constants): **$c_{abc}$ is totally antisymmetric**, even if the [Killing form](../../../lie-algebra.md#killing-form) is degenerate.

A [semisimple Lie algebra](../../../semisimple-lie-algebra.md) has no nonzero solvable ideal; equivalently, its [solvable radical](../../../lie-algebra.md#radical-of-a-lie-algebra) is zero, or, in characteristic zero, its [Killing form](../../../lie-algebra.md#killing-form) is nondegenerate. A real [compact Lie algebra](../../../lie-algebra.md#compact-lie-algebra) is the algebra of some [compact Lie group](../../../lie-theory.md#compact-lie-group), equivalently an algebra admitting a positive-definite [invariant bilinear form on a Lie algebra](../../../lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra). For a real [semisimple Lie algebra](../../../semisimple-lie-algebra.md) the [compactness criterion from the Killing form](../../../lie-algebra.md#compactness-criterion-from-the-killing-form) says precisely that $\kappa$ is negative-definite. A compact algebra with a nonzero abelian center has a degenerate [Killing form](../../../lie-algebra.md#killing-form), so the semisimplicity qualification matters.

For a [semisimple Lie algebra](../../../semisimple-lie-algebra.md), let $\kappa^{ab}$ denote the inverse matrix of $\kappa_{ab}=\kappa(t_a,t_b)$. Its [Casimir operator](../../../semisimple-lie-algebra.md#casimir-element) in $d$ is

$$
\boxed{C=\kappa^{ab}d(t_a)d(t_b).}
$$

This contraction is independent of the chosen [basis](../../../vector-space.md#basis). To prove centrality directly, put $[X,t_b]=A^a{}_b t_a$. Invariance gives $A^{\mathsf T}\kappa+\kappa A=0$, hence $A\kappa^{-1}+\kappa^{-1}A^{\mathsf T}=0$. The [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) property and the product rule for a [commutator](../../../lie-algebra.md#commutator) now give

$$
[d(X),C]=\kappa^{ab}\bigl(A^c{}_a d(t_c)d(t_b)+A^c{}_b d(t_a)d(t_c)\bigr)=0.
$$

Indeed, the coefficient of $d(t_c)d(t_b)$ in this expression is $(A\kappa^{-1}+\kappa^{-1}A^{\mathsf T})^{cb}$. Thus **$[d(X),C]=0$ for every $X$**. No irreducibility of $d$ is required.

The [matrix units](../../../vector-space.md#matrix-unit) obey $E_{ij}E_{pq}=\delta_{jp}E_{iq}$. Consequently the [general linear Lie algebra](../../../lie-algebra.md#general-linear-lie-algebra) $\mathcal M=\mathfrak{gl}_n(\mathbb R)$ has

$$
\boxed{[E_{ij},E_{pq}]=\delta_{jp}E_{iq}-\delta_{qi}E_{pj},\qquad c_{ij,pq}{}^{mn}=\delta_{jp}\delta_i^m\delta_q^n-\delta_{qi}\delta_p^m\delta_j^n.}
$$

For its [Killing form](../../../lie-algebra.md#killing-form), write $L_X(Z)=XZ$ and $R_X(Z)=ZX$, so that $\operatorname{ad}_X=L_X-R_X$. Left multiplication acts identically on each of the $n$ columns, and right multiplication identically on each of the $n$ rows. Thus $\operatorname{Tr}(L_XL_Y)=\operatorname{Tr}(R_XR_Y)=n\operatorname{tr}(XY)$. The diagonal coefficient of $L_XR_Y$ on $E_{ij}$ is $X_{ii}Y_{jj}$, giving $\operatorname{Tr}(L_XR_Y)=\operatorname{tr}X\operatorname{tr}Y$; the other mixed trace is identical. This proves the [Killing form of the general linear Lie algebra](../../../lie-algebra.md#killing-form-of-the-general-linear-lie-algebra):

$$
\kappa(X,Y)=2n\operatorname{tr}(XY)-2\operatorname{tr}X\operatorname{tr}Y,\qquad \boxed{\kappa_{ij,pq}=2n\delta_{jp}\delta_{iq}-2\delta_{ij}\delta_{pq}.}
$$

The scalar matrices form a nonzero central abelian ideal, so **$\mathcal M$ is not semisimple for any $n\ge1$**. More explicitly, the [radical of the Killing form](../../../lie-algebra.md#radical-of-the-killing-form) is $\mathbb RI$, since vanishing against every $Y$ forces $nX-(\operatorname{tr}X)I=0$ by nondegeneracy of the trace pairing. For $n\ge2$, take $H=E_{11}-E_{22}$. Then $\kappa(H,H)=4n>0$, whereas a positive-definite invariant inner product would make every adjoint map skew and hence give $\kappa(X,X)\le0$. Therefore **$\mathcal M$ is not compact when $n\ge2$**. For the allowed exceptional value $n=1$, the abstract abelian algebra $\mathbb R$ is a [compact Lie algebra](../../../lie-algebra.md#compact-lie-algebra), being isomorphic to the algebra of $U(1)$; the particular matrix group $GL_1(\mathbb R)$ is nevertheless noncompact. This distinguishes compactness of an algebra from that of a chosen group realizing it.

For the final algebra, the printed basis specifies [strictly upper triangular matrices](../../../linear-algebra.md#strictly-upper-triangular-matrix). If $i<j$ and $p<q$, the first term in $[E_{ij},E_{pq}]$ can be nonzero only when $i<j=p<q$, and then $E_{iq}$ is strictly upper triangular; the second can be nonzero only when $p<q=i<j$, and then $E_{pj}$ is strictly upper triangular. Bilinearity proves closure under the [Lie bracket](../../../lie-algebra.md#lie-bracket). To compute its own [Killing form](../../../lie-algebra.md#killing-form), grade $E_{ij}$ by the positive integer $j-i$. Bracketing with any basis element increases that degree whenever the result is nonzero. In a basis ordered by degree, all adjoint maps are strictly triangular, as are their products. Every such product has zero trace, so the [Killing form of a nilpotent Lie algebra vanishes](../../../lie-algebra.md#killing-form-of-a-nilpotent-lie-algebra-vanishes) here. Therefore the subspace denoted by a prime in the PDF is

$$
\boxed{\mathcal L'=\mathcal L,\qquad \dim\mathcal L'=\frac{n(n-1)}2.}
$$

This is the defined [radical of the Killing form](../../../lie-algebra.md#radical-of-the-killing-form), not the derived algebra; for $n=1$ both $\mathcal L$ and this radical are zero.

## 2

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) is a nonzero vector $v_0$ satisfying $J_3v_0=jv_0$ and $J_+v_0=0$; its eigenvalue $j$ is the [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation). Existence does not require the [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) to be antihermitian. Since $V$ is a nonzero finite-dimensional complex [vector space](../../../vector-space.md), $J_3$ has an eigenvector $v$ with some eigenvalue $\lambda$. The [commutator](../../../lie-algebra.md#commutator) with $J_+$ shows that each nonzero $J_+^kv$ has eigenvalue $\lambda+k$. Infinitely many such vectors would have distinct eigenvalues and be linearly independent, which is impossible. The last nonzero vector in this raising chain is therefore a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) $v_0$.

Put $v_\ell=J_-^\ell v_0$. The [ladder operator](../../../semisimple-lie-algebra.md#ladder-operator) relations give $J_3v_\ell=(j-\ell)v_\ell$. The raising coefficient follows by expanding the commutator of $J_+$ with a power of $J_-$:

$$
\begin{aligned}
J_+v_\ell&=[J_+,J_-^\ell]v_0
=\sum_{r=0}^{\ell-1}J_-^rJ_3J_-^{\ell-1-r}v_0\\
&=\sum_{r=0}^{\ell-1}(j-\ell+1+r)v_{\ell-1}
=\frac{\ell(2j-\ell+1)}2v_{\ell-1}.
\end{aligned}
$$

The factor $1/2$ is essential: these [ladder operators](../../../semisimple-lie-algebra.md#ladder-operator) have $[J_+,J_-]=J_3$, rather than the convention with $2J_3$. The same finite-dimensionality argument gives a last nonzero lowered vector $v_r$, with $J_-v_r=v_{r+1}=0$. Applying $J_+$ to $v_{r+1}=0$ yields

$$
0=\frac{(r+1)(2j-r)}2v_r,
$$

so **$2j=r\in\mathbb Z_{\ge0}$**. All $v_0,\ldots,v_r$ are nonzero and have distinct eigenvalues. Their span is invariant under $J_3,J_+,J_-$ and therefore under the original three generators. Irreducibility of the [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) makes this span equal to $V$. Hence

$$
\boxed{j\in\left\{0,\tfrac12,1,\ldots\right\},\quad \dim V=2j+1,\quad V=\operatorname{span}\{J_-^\ell|j,j\rangle:0\le\ell\le2j\}.}
$$

In particular, the initial construction produces the largest eigenvalue of $J_3$, since its full spectrum is now $j,j-1,\ldots,-j$. This establishes the [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) without assuming beforehand that all eigenvalues are real or that $J_3$ is diagonalizable.

For the additional antihermitian [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation), the given definitions imply $J_3^\dagger=J_3$ and $J_+^\dagger=J_-$. Thus distinct $J_3$ eigenvalues give orthogonal [weight vectors](../../../semisimple-lie-algebra.md#weight-vector). With $\|v_0\|=1$, write $N_\ell=\|v_\ell\|^2$. The adjoint relation and the raising coefficient give

$$
N_\ell=\langle v_{\ell-1},J_+J_-v_{\ell-1}\rangle
=\frac{\ell(2j-\ell+1)}2N_{\ell-1},\qquad N_0=1.
$$

Multiplying this recursion proves the [normalized highest-weight lowering formula](../../../quantum-mechanics.md#normalized-highest-weight-lowering-formula) in the present normalization:

$$
\boxed{N_\ell=\frac{(2j)!\,\ell!}{2^\ell(2j-\ell)!},\qquad |j,m\rangle=\frac{J_-^{j-m}|j,j\rangle}{\sqrt{N_{j-m}}}.}
$$

Every factorial argument is an integer, even for half-integral $j$. The displayed states have unit norm, mutually distinct eigenvalues, and span $V$, so they form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis). Their phase convention also fixes the positive ladder amplitudes

$$
J_\pm|j,m\rangle=\sqrt{\frac{(j\mp m)(j\pm m+1)}2}\,|j,m\pm1\rangle,
$$

with the endpoint actions interpreted as zero. These amplitudes will determine the [Clebsch-Gordan coefficients](../../../representation-theory.md#clebsch-gordan-coefficients).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [Clebsch-Gordan decomposition for SU2](../../../representation-theory.md#clebsch-gordan-decomposition-for-su2) is

$$
\boxed{V_{j_1}\otimes V_{j_2}\cong\bigoplus_{j=|j_1-j_2|}^{j_1+j_2}V_j,\qquad \dim V_j=2j+1,}
$$

where $j$ increases by one and every summand occurs once. The [tensor product of Lie algebra representations](../../../lie-algebra.md#tensor-product-of-lie-algebra-representations) is antihermitian for the product inner product, so an invariant subspace has an invariant orthogonal complement; this gives complete reducibility. To see the particular summands, suppose $j_1\ge j_2$. The product [weight diagram](../../../semisimple-lie-algebra.md#weight-diagram) has one state of weight $j_1+j_2$, two of weight $j_1+j_2-1$, and increasing multiplicities down to the plateau determined by $j_1-j_2$. Subtracting the weight string of $V_{j_1+j_2}$ leaves a single highest state of weight $j_1+j_2-1$. Repeating [highest-weight character subtraction](../../../semisimple-lie-algebra.md#highest-weight-character-subtraction) yields exactly the displayed sequence, down to $j_1-j_2$. Its dimensions exhaust the tensor product because

$$
\sum_{j=j_1-j_2}^{j_1+j_2}(2j+1)=(2j_1+1)(2j_2+1).
$$

The case $j_2\ge j_1$ is identical with the factors exchanged.

Let $C^j_m(m_1,m_2)=\langle m_1:m_2|j,m\rangle$ be the [Clebsch-Gordan coefficients](../../../representation-theory.md#clebsch-gordan-coefficients). Since the total $J_3$ is $J_3^{(1)}\otimes1+1\otimes J_3^{(2)}$, orthogonality of its [eigenspaces](../../../linear-operator-theory.md#eigenspace) gives the selection rule **$C^j_m(m_1,m_2)=0$ unless $m_1+m_2=m$**. Normalize the coupled states by lowering from a unit [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector), as in part (i); a common phase for an entire summand is immaterial. Then

$$
J_\mp|j,m\rangle=\sqrt{\frac{(j\pm m)(j\mp m+1)}2}|j,m\mp1\rangle.
$$

Take the inner product with $\langle m_1:m_2|$. On the other hand, the total [ladder operator](../../../semisimple-lie-algebra.md#ladder-operator) is $J_\mp^{(1)}\otimes1+1\otimes J_\mp^{(2)}$, and $J_\mp^\dagger=J_\pm$. Its action on the product bra is therefore

$$
\begin{aligned}
\langle m_1:m_2|J_\mp
&=\sqrt{\frac{(j_1\mp m_1)(j_1\pm m_1+1)}2}\langle m_1\pm1:m_2|\\
&\quad+\sqrt{\frac{(j_2\mp m_2)(j_2\pm m_2+1)}2}\langle m_1:m_2\pm1|.
\end{aligned}
$$

Equating the two evaluations and multiplying by $\sqrt2$ proves both signs of the [ladder recurrence for Clebsch-Gordan coefficients](../../../representation-theory.md#ladder-recurrence-for-clebsch-gordan-coefficients):

$$
\boxed{\begin{aligned}
\sqrt{(j\pm m)(j\mp m+1)}\,C^j_{m\mp1}(m_1,m_2)
&=\sqrt{(j_1\mp m_1)(j_1\pm m_1+1)}\,C^j_m(m_1\pm1,m_2)\\
&\quad+\sqrt{(j_2\mp m_2)(j_2\pm m_2+1)}\,C^j_m(m_1,m_2\pm1).
\end{aligned}}
$$

Terms with an index outside its allowed weight range are zero. Merely specifying eigenvectors of $J_3$ would allow unrelated phases for different $m$; the coherent positive-ladder convention above is what makes these recurrences hold with the displayed positive square roots.

## 3

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Covariance of the fundamental [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative) requires $D_\mu^{f\prime}(g\chi)=gD_\mu^f\chi$ for every column $\chi$. Expanding the left side and cancelling $g\partial_\mu\chi$ gives $(\partial_\mu g)+A'_\mu g=gA_\mu$. Therefore the necessary and sufficient [Yang-Mills gauge transformation](../../../relativistic-quantum-field.md#yang-mills-gauge-transformation) is

$$
\boxed{A'_\mu=gA_\mu g^{-1}-(\partial_\mu g)g^{-1}.}
$$

In operator notation $D_\mu^{f\prime}=gD_\mu^fg^{-1}$. Expanding its [commutator](../../../lie-algebra.md#commutator) on an arbitrary column shows $[D_\mu^f,D_\nu^f]\chi=F_{\mu\nu}\chi$: the second derivatives cancel, as do the terms containing a single derivative of $\chi$. Conjugating this identity proves the [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) transformation

$$
\boxed{F'_{\mu\nu}=gF_{\mu\nu}g^{-1}.}
$$

Thus the [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) transforms homogeneously even though the potential has an inhomogeneous derivative term.

For the [adjoint scalar field](../../../quantum-field-theory.md#adjoint-scalar-field), write $B_\mu=(\partial_\mu g)g^{-1}$ and $\Phi'=g\Phi g^{-1}$. Differentiating the inverse matrix gives

$$
\partial_\mu\Phi'=g(\partial_\mu\Phi)g^{-1}+[B_\mu,\Phi'],\qquad [A'_\mu,\Phi']=g[A_\mu,\Phi]g^{-1}-[B_\mu,\Phi'].
$$

The extra terms cancel, proving **$D'_\mu\Phi'=g(D_\mu\Phi)g^{-1}$** for the [adjoint covariant derivative](../../../relativistic-quantum-field.md#adjoint-covariant-derivative). Its curvature is obtained by another direct expansion:

$$
\begin{aligned}
[D_\mu,D_\nu]\Phi
&=[\partial_\mu A_\nu-\partial_\nu A_\mu,\Phi]
+[A_\mu,[A_\nu,\Phi]]-[A_\nu,[A_\mu,\Phi]]\\
&=[\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu],\Phi]
=\boxed{[F_{\mu\nu},\Phi]},
\end{aligned}
$$

where the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) combines the last two terms.

For the equations of motion take compactly supported variations, and assume $e\ne0$, as required by the Lagrangian coefficient. Invariance of the [Killing form](../../../lie-algebra.md#killing-form) implies

$$
\partial_\mu\kappa(X,Y)=\kappa(D_\mu X,Y)+\kappa(X,D_\mu Y).
$$

Indeed, the two connection terms sum to $\kappa([A_\mu,X],Y)+\kappa(X,[A_\mu,Y])=0$. This is the [gauge-covariant integration by parts](../../../relativistic-quantum-field.md#gauge-covariant-integration-by-parts) identity. The needed variations are

$$
\delta F_{\mu\nu}=D_\mu\delta A_\nu-D_\nu\delta A_\mu,\qquad
\delta(D_\mu\Phi)=D_\mu\delta\Phi+[\delta A_\mu,\Phi].
$$

Antisymmetry of the [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) combines its two variation terms. Applying [gauge-covariant integration by parts](../../../relativistic-quantum-field.md#gauge-covariant-integration-by-parts) to the action $S=\int\mathcal L\,d^4x$ gives

$$
\begin{aligned}
\delta S=\int d^4x\biggl\{&-\frac1{e^2}\kappa(\delta A_\nu,D_\mu F^{\mu\nu})
-\kappa(\delta A_\nu,[\Phi,D^\nu\Phi])\\
&+\kappa(\delta\Phi,D_\mu D^\mu\Phi)\biggr\}.
\end{aligned}
$$

Here $\kappa([\delta A_\nu,\Phi],D^\nu\Phi)=\kappa(\delta A_\nu,[\Phi,D^\nu\Phi])$ fixes the sign of the scalar current. Since the [Killing form](../../../lie-algebra.md#killing-form) is nondegenerate on a [semisimple Lie algebra](../../../semisimple-lie-algebra.md), independent variations give the coupled [Yang-Mills equations](../../../relativistic-quantum-field.md#yang-mills-equations) and scalar equation

$$
\boxed{D_\mu F^{\mu\nu}+e^2[\Phi,D^\nu\Phi]=0,\qquad D_\mu D^\mu\Phi=0.}
$$

Equivalently, $D_\mu F^{\mu\nu}=e^2[D^\nu\Phi,\Phi]$. These signs use the stated [Minkowski metric](../../../special-relativity.md#minkowski-metric), with upper spatial derivatives $D^i=-D_i$.

It remains to verify every equation for the static [Bogomolny equations](../../../quantum-field-theory.md#bogomolny-equations). The hypotheses imply $F_{0i}=0$ and $D_0\Phi=0$, so the temporal gauge equation is automatically zero. The [gauge-theory Bianchi identity](../../../relativistic-quantum-field.md#gauge-theory-bianchi-identity)

$$
D_iF_{jk}+D_jF_{ki}+D_kF_{ij}=0
$$

follows, for example, from the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) for the fundamental [gauge covariant derivatives](../../../relativistic-quantum-field.md#gauge-covariant-derivative), using their commutator $F_{ij}$. Define $B_i=\tfrac12\varepsilon_{ijk}F_{jk}$. Contracting the [gauge-theory Bianchi identity](../../../relativistic-quantum-field.md#gauge-theory-bianchi-identity) with $\varepsilon_{ijk}$ gives $D_iB_i=0$. The [Bogomolny equations](../../../quantum-field-theory.md#bogomolny-equations) say $B_i=eD_i\Phi$, so $e\ne0$ implies $D_iD_i\Phi=0$. In the static configuration $D_\mu D^\mu\Phi=-D_iD_i\Phi$, verifying the scalar equation.

For the spatial gauge equation, use $F^{ij}=F_{ij}$ and $D^j\Phi=-D_j\Phi$. The [Bogomolny equations](../../../quantum-field-theory.md#bogomolny-equations), the curvature commutator proved above, and the [contraction of two Levi-Civita symbols](../../../calculus.md#contraction-of-two-levi-civita-symbols) give

$$
\begin{aligned}
D_iF_{ij}&=e\varepsilon_{ijk}D_iD_k\Phi
=\frac e2\varepsilon_{ijk}[D_i,D_k]\Phi
=\frac e2\varepsilon_{ijk}[F_{ik},\Phi]\\
&=\frac{e^2}2\varepsilon_{ijk}\varepsilon_{ik\ell}[D_\ell\Phi,\Phi]
=-e^2[D_j\Phi,\Phi]=e^2[\Phi,D_j\Phi],
\end{aligned}
$$

since $\varepsilon_{ijk}\varepsilon_{ik\ell}=-2\delta_{j\ell}$. This is exactly $D_iF^{ij}+e^2[\Phi,D^j\Phi]=0$. Thus **the static first-order Bogomolny system satisfies all four gauge equations and the scalar equation**, with no extra ansatz or boundary assumption needed for this local implication. This is the mechanism by which [Bogomolny monopole equations imply Yang-Mills-Higgs equations](../../../classical-field-theory-soliton.md#bogomolny-monopole-equations-imply-yang-mills-higgs-equations).

## 4

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [SU(3) Lie algebra](../../../lie-algebra.md#su-3-lie-algebra) is the compact real algebra of traceless [skew-Hermitian matrices](../../../linear-operator-theory.md#skew-hermitian-matrix); its complexification is $\mathfrak{sl}_3(\mathbb C)$, a [special linear Lie algebra](../../../semisimple-lie-algebra.md#special-linear-lie-algebra). In an antihermitian [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation), the two commuting Cartan operators $H_1,H_2$ are [Hermitian matrices](../../../hilbert-space.md#hermitian-operator), and the root operators satisfy $(E_+^a)^\dagger=E_-^a$. Thus the [spectral theorem](../../../hilbert-space.md#spectral-theorem) gives an orthogonal [weight-space decomposition](../../../semisimple-lie-algebra.md#weight-space-decomposition)

$$
V=\bigoplus_\mu V_\mu,\qquad H_rv=\mu_rv\quad(v\in V_\mu),\qquad \mu=(\mu_1,\mu_2)\in\mathbb R^2.
$$

A [weight diagram](../../../semisimple-lie-algebra.md#weight-diagram) plots the pairs $\mu$, recording the [weight multiplicity](../../../semisimple-lie-algebra.md#weight-multiplicity) $\dim V_\mu$ at each position. One point need not represent only one state. The commutators with $H_1,H_2$ give the [roots of a root system](../../../semisimple-lie-algebra.md#root-of-a-root-system)

$$
\alpha_1=(1,0),\qquad \alpha_2=\left(-\frac12,\frac{\sqrt3}2\right),\qquad \alpha_3=\alpha_1+\alpha_2.
$$

The [raising operators](../../../semisimple-lie-algebra.md#raising-operator) $E_+^a$ move a nonzero [weight vector](../../../semisimple-lie-algebra.md#weight-vector) by $+\alpha_a$ and the [lowering operators](../../../semisimple-lie-algebra.md#lowering-operator) move it by $-\alpha_a$. These six root directions form the [A2 root system](../../../semisimple-lie-algebra.md#a2-root-system). Each root and its negative generate an [SU(2) representation](../../../representation-theory.md#representation-theory-of-su-2) ladder; in particular the pairs with Cartan operators $H_1$ and $-H_1/2+\sqrt3H_2/2$ constrain the two simple-root strings.

Choose a linear functional positive on the three positive roots. A maximal [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) for this ordering is killed by every [raising operator](../../../semisimple-lie-algebra.md#raising-operator). In an [Irreducible Lie algebra representation](../../../lie-algebra.md#irreducible-lie-algebra-representation) it generates the entire representation by lowering, and its [weight space](../../../semisimple-lie-algebra.md#weight-space) has dimension one. The two [SU(2) representation](../../../representation-theory.md#representation-theory-of-su-2) strings show that its [Dynkin labels](../../../semisimple-lie-algebra.md#dynkin-label) are nonnegative integers:

$$
p=2\lambda_1,\qquad q=-\lambda_1+\sqrt3\lambda_2,\qquad p,q\in\mathbb Z_{\ge0}.
$$

Conversely, each such pair specifies exactly one finite-dimensional irreducible [highest-weight representation](../../../semisimple-lie-algebra.md#highest-weight-representation). Write it as $R(p,q)$. The [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight) in these Cartesian coordinates are $\omega_1=(1/2,1/(2\sqrt3))$ and $\omega_2=(0,1/\sqrt3)$, so

$$
\lambda=p\omega_1+q\omega_2=\left(\frac p2,\frac{p+2q}{2\sqrt3}\right),\qquad
\boxed{\dim R(p,q)=\frac{(p+1)(q+1)(p+q+2)}2.}
$$

The dimension follows from the three positive-root factors in the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula): $p+1$, $q+1$, and $(p+q+2)/2$. The complex conjugate representation is $R(q,p)$, with every [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) negated. The [SU(3) highest-weight coordinates](../../../semisimple-lie-algebra.md#su-3-highest-weight-coordinates) here use $(p,q)$ as Dynkin labels, not as the plotted Cartesian coordinates.

The [weight diagram](../../../semisimple-lie-algebra.md#weight-diagram) is invariant under the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group), generated by reflections perpendicular to the two simple roots; its convex hull is the orbit polygon of the [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation). For $p=q=0$ it is a point, the trivial representation. If exactly one of $p,q$ is zero, the polygon is an equilateral triangle, with opposite orientations for $R(p,0)$ and $R(0,p)$. Its edge has $p$ root steps. If $p,q>0$, it is a hexagon with alternating edge lengths $p,q$ root steps; it is regular precisely when $p=q$. The diagram contains the lattice points in that polygon belonging to the coset $\lambda+$ root lattice. A point in a different [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice) coset is not a weight merely because it lies inside the polygon.

The [shell multiplicities in an SU(3) weight diagram](../../../semisimple-lie-algebra.md#shell-multiplicities-in-an-su-3-weight-diagram) can be stated geometrically. The outer boundary has [weight multiplicity](../../../semisimple-lie-algebra.md#weight-multiplicity) one. Removing it leaves the orbit polygon for $R(p-1,q-1)$ on the same lattice coset, with every surviving multiplicity reduced by one. Repeating increases the actual [weight multiplicity](../../../semisimple-lie-algebra.md#weight-multiplicity) by one at each inward layer until the smaller label reaches zero. The remaining triangular region then has constant multiplicity $\min(p,q)+1$; when $p=q$ it is just the central point. A triangular [weight diagram](../../../semisimple-lie-algebra.md#weight-diagram) has multiplicity one everywhere. Thus $R(1,1)=\mathbf8$, the [adjoint representation of SU(3)](../../../lie-algebra.md#adjoint-representation-of-su-3), has six root weights of multiplicity one and two independent zero-weight states; $R(2,1)=\mathbf{15}$ has an outer shell of multiplicity one and an inner triangle of multiplicity two; $R(2,2)=\mathbf{27}$ has twelve outer states, six positions of multiplicity two, and a central position of multiplicity three. The total is $12+6\cdot2+3=27$. The [dominant weight multiplicity formula for sl3](../../../semisimple-lie-algebra.md#dominant-weight-multiplicity-formula-for-sl3) is an algebraic expression of the same rule.

<a id="4/image-triangular-and-hexagonal-su-3-weight-diagrams-with-each-weight-space-dimension-shown-at-its-point"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-52-su3-weights.png)

**[Figure 1](#4/image-triangular-and-hexagonal-su-3-weight-diagrams-with-each-weight-space-dimension-shown-at-its-point). Triangular and hexagonal SU(3) weight diagrams, with each weight-space dimension shown at its point**.

For a [tensor product of Lie algebra representations](../../../lie-algebra.md#tensor-product-of-lie-algebra-representations), the Cartan operators add. Consequently its [tensor-product weight diagram](../../../semisimple-lie-algebra.md#tensor-product-weight-diagram) has [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $\mu+\nu$ and multiplicities

$$
m_{V\otimes W}(\rho)=\sum_{\mu+\nu=\rho}m_V(\mu)m_W(\nu).
$$

Geometrically, place a copy of the second [weight diagram](../../../semisimple-lie-algebra.md#weight-diagram) at every weight of the first, multiplying and adding coincident multiplicities. Because the representation is antihermitian, invariant subspaces have invariant orthogonal complements. To decompose the product, select a maximal remaining [dominant weight](../../../semisimple-lie-algebra.md#dominant-weight), identify its irreducible [highest-weight representation](../../../semisimple-lie-algebra.md#highest-weight-representation), subtract that representation's whole diagram with its [weight multiplicities](../../../semisimple-lie-algebra.md#weight-multiplicity), and repeat. This [highest-weight character subtraction](../../../semisimple-lie-algebra.md#highest-weight-character-subtraction) must exhaust every weight, not merely the corners. Unlike the [Clebsch-Gordan decomposition for SU2](../../../representation-theory.md#clebsch-gordan-decomposition-for-su2), an SU(3) product may contain repeated copies of an irreducible representation.

The two three-dimensional [Fundamental representations of sl3](../../../semisimple-lie-algebra.md#fundamental-representations-of-sl3) are $\mathbf3=R(1,0)$ and $\overline{\mathbf3}=R(0,1)$. In $\mathbf3\otimes\mathbf3$, the largest weight is $2\omega_1$, giving the six-dimensional triangle $R(2,0)$; subtracting it leaves the reversed three-dimensional triangle $R(0,1)$. The first summand consists of symmetric tensors and the second of antisymmetric tensors. In $\mathbf3\otimes\overline{\mathbf3}$, the weight sums give the six roots once and weight zero three times. Subtracting the octet, whose zero weight has multiplicity two, leaves a singlet. Hence the [octet and singlet in a fundamental SU3 tensor product](../../../representation-theory.md#octet-and-singlet-in-a-fundamental-su3-tensor-product) and the two-quark product are

$$
\boxed{\mathbf3\otimes\mathbf3=\mathbf6\oplus\overline{\mathbf3},\qquad
\mathbf3\otimes\overline{\mathbf3}=\mathbf8\oplus\mathbf1.}
$$

The first dimensions are $9=6+3$, and the second are $9=8+1$. Next $\mathbf6\otimes\mathbf3$ has highest weight $3\omega_1$, giving $R(3,0)=\mathbf{10}$. Subtraction leaves one $R(1,1)=\mathbf8$. Together with $\overline{\mathbf3}\otimes\mathbf3=\mathbf8\oplus\mathbf1$, this proves the [tensor cube of the defining SU(3) representation](../../../semisimple-lie-algebra.md#tensor-cube-of-the-defining-su-3-representation):

$$
\boxed{\mathbf3^{\otimes3}=\mathbf{10}\oplus\mathbf8\oplus\mathbf8\oplus\mathbf1,\qquad 27=10+8+8+1.}
$$

The decuplet is fully symmetric in the three factors, the singlet fully antisymmetric, and the two octets have mixed permutation symmetry.

For the [quark model](../../../physics.md#quark-model), the relevant approximate [flavour symmetry](../../../standard-model.md#flavor-symmetry) rotates the three light [quarks](../../../standard-model.md#quark) $u,d,s$ in the fundamental $\mathbf3$. The [up quark](../../../standard-model.md#up-quark), [down quark](../../../standard-model.md#down-quark), and [strange quark](../../../standard-model.md#strange-quark) basis states have the [weight diagram of the defining SU(3) representation](../../../semisimple-lie-algebra.md#weight-diagram-of-the-defining-su-3-representation). In physical coordinates define [isospin](../../../standard-model.md#isospin) $I_3=H_1$ and [flavor hypercharge](../../../standard-model.md#flavor-hypercharge) $Y=2H_2/\sqrt3$. Then

$$
\begin{array}{c|ccc}
 &u&d&s\\\hline
I_3&1/2&-1/2&0\\
Y&1/3&1/3&-2/3\\
Q&2/3&-1/3&-1/3
\end{array}
$$

The last row follows from the [Gell-Mann--Nishijima formula](../../../standard-model.md#gell-mann-nishijima-formula) $Q=I_3+Y/2$, in units of the positive elementary [electric charge](../../../electromagnetism.md#electric-charge). The [antiquarks](../../../standard-model.md#antiquark) transform in $\overline{\mathbf3}$ and have the negatives of these additive quantum numbers. Each [quark](../../../standard-model.md#quark) has [baryon number](../../../standard-model.md#baryon-number) $B=1/3$; the [strange quark](../../../standard-model.md#strange-quark) has [strangeness](../../../standard-model.md#strangeness) $S=-1$, while $u,d$ have $S=0$. Thus $Y=B+S$, distinguishing [flavor hypercharge](../../../standard-model.md#flavor-hypercharge) from electroweak hypercharge. The [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) geometry is equilateral in $(H_1,H_2)$; using $(I_3,Y)$ rescales the vertical coordinate.

A conventional [meson](../../../physics.md#meson) has valence content $q\bar q$, so its [flavour symmetry](../../../standard-model.md#flavor-symmetry) gives a [meson octet](../../../standard-model.md#meson-octet) and a singlet. For the light [pseudoscalar mesons](../../../physics.md#pseudoscalar-meson), the octet contains the [pions](../../../standard-model.md#pion) $\pi^+,\pi^0,\pi^-$ at $Y=0$ with [isospin](../../../standard-model.md#isospin) $I=1$, the [kaons](../../../physics.md#kaon) $K^+=u\bar s,K^0=d\bar s$ at $Y=1$, their antiparticles at $Y=-1$, and the $I=0,Y=0$ [Eta octet state](../../../standard-model.md#eta-octet-state). The central [weight multiplicity](../../../semisimple-lie-algebra.md#weight-multiplicity) two is realized by

$$
\pi^0=\frac{u\bar u-d\bar d}{\sqrt2},\qquad
\eta_8=\frac{u\bar u+d\bar d-2s\bar s}{\sqrt6}.
$$

The orthogonal [eta singlet state](../../../physics.md#eta-singlet-state) is $\eta_1=(u\bar u+d\bar d+s\bar s)/\sqrt3$. The [eta and eta prime mesons](../../../physics.md#eta-and-eta-prime-mesons) are mixtures of $\eta_8,\eta_1$, rather than exact octet and singlet mass eigenstates; this gives the [pseudoscalar meson nonet](../../../physics.md#pseudoscalar-meson-nonet). A different spin coupling of the same flavour product gives the [vector mesons](../../../physics.md#vector-meson), again an octet and singlet, including the $\rho$, $K^*$, and neutral $\omega,\phi$ mixtures. The lowest orbital states have $J^P=0^-$ and $1^-$ respectively.

A conventional [baryon](../../../physics.md#baryon) has three valence [quarks](../../../standard-model.md#quark), so the tensor-cube decomposition supplies the flavour possibilities. The observed lowest [baryon octet](../../../standard-model.md#baryon-octet) has spin $1/2$ and positive [parity](../../../quantum-mechanics.md#parity). Its [isospin](../../../standard-model.md#isospin) rows are $(Y,I)=(1,1/2),(0,1),(0,0),(-1,1/2)$: the [nucleons](../../../physics.md#nucleon) $p,n$, the three [Sigma baryons](../../../physics.md#sigma-baryon), the [Lambda baryon](../../../physics.md#lambda-baryon), and the two [Xi baryons](../../../physics.md#xi-baryon). The central states $\Sigma^0$ and $\Lambda$ have the same [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $(I_3,Y)=(0,0)$ but different total [isospin](../../../standard-model.md#isospin); this is the physical meaning of the octet's central multiplicity two. The spin-$3/2$, positive-parity [baryon decuplet](../../../standard-model.md#baryon-decuplet) is the triangle with rows

$$
\begin{array}{c|c|c}
Y&I&\text{states}\\\hline
1&3/2&\Delta^{++},\Delta^+,\Delta^0,\Delta^-\\
0&1&\Sigma^{*+},\Sigma^{*0},\Sigma^{*-}\\
-1&1/2&\Xi^{*0},\Xi^{*-}\\
-2&0&\Omega^-
\end{array}
$$

The [Delta baryons](../../../physics.md#delta-baryon) form its top row, and the [Omega baryon](../../../physics.md#omega-baryon) is the bottom $sss$ state. All ten [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) have multiplicity one. Their [electric charges](../../../electromagnetism.md#electric-charge) follow directly from the [Gell-Mann--Nishijima formula](../../../standard-model.md#gell-mann-nishijima-formula); for example $\Delta^{++}$ has $I_3=3/2,Y=1$, so $Q=2$, and $\Omega^-$ has $I_3=0,Y=-2$, so $Q=-1$.

<a id="4/image-light-pseudoscalar-meson-octet-spin-one-half-baryon-octet-and-spin-three-halves-baryon-decuplet-in-isospin-and-flavour-hypercharge-coordinates"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-52-hadron-multiplets.png)

**[Figure 2](#4/image-light-pseudoscalar-meson-octet-spin-one-half-baryon-octet-and-spin-three-halves-baryon-decuplet-in-isospin-and-flavour-hypercharge-coordinates). Light pseudoscalar meson octet, spin-one-half baryon octet, and spin-three-halves baryon decuplet in isospin and flavour-hypercharge coordinates**.

The two algebraic octets do not mean that two independent ground-state octets must occur. A [three-quark colour singlet](../../../physics.md#three-quark-colour-singlet) has a completely antisymmetric colour wavefunction. For a symmetric spatial ground state, the [Pauli exclusion principle](../../../quantum-mechanics.md#pauli-exclusion-principle) therefore requires a symmetric combined spin-flavour wavefunction. The symmetric flavour decuplet pairs with symmetric spin $3/2$; mixed flavour octets pair with mixed spin $1/2$ in one symmetric combination. Equivalently, the [symmetric spin-flavour SU6 representation](../../../physics.md#symmetric-spin-flavour-su6-representation) has

$$
\operatorname{Sym}^3(\mathbb C^3\otimes\mathbb C^2)
\cong(\mathbf{10},\mathbf4)\oplus(\mathbf8,\mathbf2),\qquad 56=10\cdot4+8\cdot2.
$$

The [three-quark flavour singlet](../../../standard-model.md#three-quark-flavour-singlet) is the antisymmetric $uds$ combination. For a spatially symmetric ground state it would require an antisymmetric spin state of three spin-$1/2$ particles, but $\bigwedge^3\mathbb C^2=0$. The [Pauli constraint on three-quark flavour multiplets](../../../physics.md#pauli-constraint-on-three-quark-flavour-multiplets) thus excludes it from this ground-state sector; orbital excitation permits other multiplets.

Finally, this [flavour symmetry](../../../standard-model.md#flavor-symmetry) is approximate: the unequal light-quark masses, especially the larger strange-quark mass, and electromagnetic interactions split masses within the multiplets and permit octet-singlet mixing. The [weight diagrams](../../../semisimple-lie-algebra.md#weight-diagram) classify flavour states, rather than asserting exact equality of their masses. Colour [SU(3)](../../../topological-group.md#su-3-group) is a separate gauge action on each flavour and supplies the colour-singlet constraint; it is not the approximate flavour action used in the [eightfold way](../../../standard-model.md#eightfold-way). **The light conventional mesons organize into flavour octets and singlets, while the spatial ground-state three-quark baryons form one spin-$1/2$ octet and one spin-$3/2$ decuplet.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
