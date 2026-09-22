# Paper 2

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2001/PaperIB_2.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2001/PaperIB_2.pdf)

**Table of contents**

- [1A](#1a)
  - [Solution](#1a/solution)
- [2G](#2g)
  - [Solution](#2g/solution)
- [3D](#3d)
  - [Solution](#3d/solution)
- [4B](#4b)
  - [Solution](#4b/solution)
- [5E](#5e)
  - [Solution](#5e/solution)
- [6C](#6c)
  - [Solution](#6c/solution)
- [7E](#7e)
  - [Solution](#7e/solution)
- [8B](#8b)
  - [Solution](#8b/solution)
- [9F](#9f)
  - [Solution](#9f/solution)
- [10A](#10a)
  - [Solution](#10a/solution)
- [11G](#11g)
  - [Solution](#11g/solution)
- [12D](#12d)
  - [Solution](#12d/solution)
- [13A](#13a)
  - [Solution](#13a/solution)
  - [i](#13a/i)
    - [Solution](#13a/i/solution)
  - [ii](#13a/ii)
    - [Solution](#13a/ii/solution)
- [14E](#14e)
  - [a](#14e/a)
    - [Solution](#14e/a/solution)
  - [b](#14e/b)
    - [Solution](#14e/b/solution)
- [15C](#15c)
  - [Solution](#15c/solution)
- [16E](#16e)
  - [Solution](#16e/solution)
- [17B](#17b)
  - [Solution](#17b/solution)
- [18F](#18f)
  - [a](#18f/a)
    - [Solution](#18f/a/solution)
  - [b](#18f/b)
    - [Solution](#18f/b/solution)

## 1A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1a/solution">Solution</h3>

↑ **Parent:** [1A](#1a)

The [contraction mapping theorem](../../../analysis.md#contraction-mapping-theorem) states that a self-map $f$ of a nonempty [complete metric space](../../../topological-analysis.md#complete-metric-space) $(X,d)$ satisfying $d(fu,fv)\le qd(u,v)$ for a fixed $0\le q<1$ has a unique [fixed point](../../../function.md#fixed-point). Its iterates converge to that point from every starting point.

To prove it, set $u_{n+1}=f(u_n)$. Induction gives $d(u_{n+1},u_n)\le q^n d(u_1,u_0)$. Hence for $m>n$, the [triangle inequality](../../../topological-analysis.md#triangle-inequality) yields

$$
d(u_m,u_n)\le\sum_{j=n}^{m-1}q^j d(u_1,u_0)\le\frac{q^n}{1-q}d(u_1,u_0).
$$

Thus the iterates are a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence), with limit $u$ by completeness. The contraction inequality gives $d(fu,u)\le qd(u,u_n)+d(u_{n+1},u)\to0$, so $f(u)=u$. For any two fixed points $u,v$, $d(u,v)\le qd(u,v)$ forces equality of the points. This proves existence, uniqueness and convergence; passing $m\to\infty$ also gives the displayed error bound.

For the three-point example, positivity and symmetry of $d'$ are immediate. For three distinct points, the largest side has length two, no more than the sum of the other two; repeated-point triangle inequalities are trivial. Thus $d'$ is a [metric](../../../topological-analysis.md#metric). The [discrete metric](../../../topological-analysis.md#discrete-metric) satisfies

$$
\boxed{d\le d'\le2d,}
$$

which proves [bilipschitz equivalence](../../../geometric-group-theory.md#bilipschitz-equivalence) of the two metrics. Define

$$
\boxed{f(x)=y,\qquad f(y)=f(z)=z.}
$$

The ratios of output to input distances for the three distinct pairs are $1/2,1/2,0$ in $d'$, so it is a contraction with $q=1/2$. In $d$, the pair $(x,y)$ has input and output distance one, precluding any $q<1$. This illustrates the [contraction property under equivalent metrics](../../../analysis.md#contraction-property-under-equivalent-metrics).

## 2G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2g/solution">Solution</h3>

↑ **Parent:** [2G](#2g)

For a [Cartesian second-rank tensor](../../../linear-algebra.md#cartesian-second-rank-tensor), write $S_{ij}=(A_{ij}+A_{ji})/2$ and $W_{ij}=(A_{ij}-A_{ji})/2$. Under an orthogonal change of frame,

$$
A'_{ij}=R_{ik}R_{jl}A_{kl},\qquad
S'_{ij}=R_{ik}R_{jl}S_{kl},\qquad W'_{ij}=R_{ik}R_{jl}W_{kl},
$$

where the last two equalities follow by interchanging the dummy indices in $A'_{ji}$. Thus the symmetric and antisymmetric parts obey the same tensor transformation law. If $A=S+W$ with $S^T=S$, $W^T=-W$, adding or subtracting its transpose forces $S=(A+A^T)/2$ and $W=(A-A^T)/2$. This also proves uniqueness.

For the given matrix, the scalar part is $a=\operatorname{Tr}(A)/3=3$. The symmetric part is $S=\begin{pmatrix}1&3&2\\3&5&4\\2&4&3\end{pmatrix}$, so the [traceless second-rank tensor](../../../linear-algebra.md#traceless-second-rank-tensor) is $B=S-3I$. The skew part is $W=\begin{pmatrix}0&-1&1\\1&0&2\\-1&-2&0\end{pmatrix}$. Comparing with the [cross product](../../../vector-space.md#cross-product) matrix $[p]_\times=\begin{pmatrix}0&-p_3&p_2\\p_3&0&-p_1\\-p_2&p_1&0\end{pmatrix}$ gives

$$
\boxed{a=3,\qquad p=(-2,1,1)^T,\qquad B=\begin{pmatrix}-2&3&2\\3&2&4\\2&4&0\end{pmatrix}.}
$$

Then $A=aI+[p]_\times+B$ proves the decomposition for every vector. The vector dual to the antisymmetric tensor is an [axial vector](../../../vector-space.md#pseudovector) under reflections, and an ordinary vector under proper rotations.

## 3D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3d/solution">Solution</h3>

↑ **Parent:** [3D](#3d)

For an observed $x\ge0$, the [continuous uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) likelihood is $p(x\mid\theta)=\theta^{-1}1_{\{\theta\ge x\}}$, with $\theta>0$. Multiplying by the stated prior cancels the factor $\theta$, giving $e^{-\theta}1_{\{\theta\ge x\}}$. Its integral over the permitted parameter values is $e^{-x}$. Hence the [posterior distribution](../../../statistical-inference.md#bayesian-posterior) is

$$
\boxed{p(\theta\mid x)=e^{-(\theta-x)}1_{\{\theta\ge x\}},\qquad \theta\mid x\sim x+\operatorname{Exp}(1).}
$$

This is the [exponential posterior for a uniform endpoint](../../../statistical-inference.md#exponential-posterior-for-a-uniform-endpoint). Its posterior mean is $x+1$ and its variance is one. The posterior expected [squared-error loss](../../../statistical-inference.md#squared-error-loss) decomposes as

$$
E[c(\theta-a)^2\mid x]=c\operatorname{Var}(\theta\mid x)+c(a-E[\theta\mid x])^2=c+c(a-x-1)^2.
$$

Since $c>0$, its unique minimum occurs at **the Bayes estimate** $\boxed{\widehat\theta_B=x+1}$. The positive loss multiplier changes the risk, not the optimizing action.

## 4B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4b/solution">Solution</h3>

↑ **Parent:** [4B](#4b)

A [connected space](../../../geometry-and-topology.md#connected-space) admits no separation into two disjoint nonempty open subsets whose union is the space. A [path-connected space](../../../geometry-and-topology.md#path-connected-space) has, for every pair of points, a continuous path from $[0,1]$ joining them. If a path-connected space had a separation $U,V$, choose its endpoints in different pieces. Their inverse images under the path would separate the connected interval $[0,1]$, a contradiction. Thus **path connectedness implies connectedness**.

For the specified subspace, first consider $Y=I\cup\bigcup_{n\ge1}J_n$. Every point of a tooth $J_n$ can move vertically to its base in $I$, then horizontally to the origin; points already on $I$ use only the horizontal segment. Concatenating these paths shows that $Y$ is [path-connected](../../../geometry-and-topology.md#path-connected-space) and hence connected.

Every point $(0,t)$ of $A$ is a limit of $(1/n,t)\in Y$. Consequently $Y$ is dense in $X=Y\cup A$ in the [subspace topology](../../../topology.md#subspace-topology). To prove $X$ connected, suppose $X=U\cup V$ were a separation. Restricting to the connected $Y$ puts all of $Y$ in one piece, say $U$. But the other nonempty relatively open piece $V$ must meet dense $Y$, a contradiction. Therefore **$\boxed{X\text{ is connected}}$**. This uses density, not an unproved path from the added vertical segment to the teeth.

## 5E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5e/solution">Solution</h3>

↑ **Parent:** [5E](#5e)

Gaussian elimination uses first-column multipliers $-2,2,-3$, second-column multiplier $2$ in the last row, and third-column multiplier $1$ there. Recording these in a unit lower-triangular matrix gives the [LU decomposition](../../../numerical-analysis.md#lu-decomposition)

$$
\boxed{L=\begin{pmatrix}1&0&0&0\\-2&1&0&0\\2&0&1&0\\-3&2&1&1\end{pmatrix},\qquad
U=\begin{pmatrix}2&-1&3&2\\0&1&2&2\\0&0&-3&2\\0&0&0&1\end{pmatrix},\qquad A=LU.}
$$

Forward substitution in $Ly=b$ gives $y=(-2,-2,8,1)^T$. Back substitution gives $x_4=1$, $-3x_3+2x_4=8$, $x_2+2x_3+2x_4=-2$, and $2x_1-x_2+3x_3+2x_4=-2$. Hence **the solution is**

$$
\boxed{x=(1,0,-2,1)^T.}
$$

## 6C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6c/solution">Solution</h3>

↑ **Parent:** [6C](#6c)

Right multiplication is linear because $(sX+tY)A=sXA+tYA$. In the supplied row-entry [basis](../../../vector-space.md#basis), write $X=\begin{pmatrix}x_1&x_2\\x_3&x_4\end{pmatrix}$. Multiplying on the right gives coordinates $(ax_1+cx_2,bx_1+dx_2,ax_3+cx_4,bx_3+dx_4)^T$. Therefore

$$
\boxed{[\rho_A]=\begin{pmatrix}a&c&0&0\\b&d&0&0\\0&0&a&c\\0&0&b&d\end{pmatrix}=\operatorname{diag}(A^T,A^T).}
$$

The transpose is ordinary, with no complex conjugation. Block determinants and invariance of determinant under transpose prove

$$
\boxed{\chi_{\rho_A}(t)=\det(tI_2-A^T)^2=\chi_A(t)^2.}
$$

For every polynomial $p$, powers of right multiplication give $p(\rho_A)(X)=Xp(A)$. If $p(A)=0$ then $p(\rho_A)=0$; if $p(\rho_A)=0$, take $X=I$ to infer $p(A)=0$. They have identical annihilating polynomials, so their unique monic least-degree annihilator, the [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial), is the same. Thus **$m_{\rho_A}=m_A$**, as in the [characteristic and minimal polynomials of right multiplication](../../../linear-operator-theory.md#characteristic-and-minimal-polynomials-of-right-multiplication) result.

## 7E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7e/solution">Solution</h3>

↑ **Parent:** [7E](#7e)

At a point $z_0=x+iy$, [complex differentiability](../../../complex-analysis.md#complex-differentiability) means that

$$
f'(z_0)=\lim_{h\to0,\ h\in\mathbb C\setminus\{0\}}\frac{f(z_0+h)-f(z_0)}h
$$

exists and is independent of the direction of approach. Write $f=u+iv$. Restricting to real $h$ gives $f'=u_x+iv_x$. Restricting to $h=it$, with real $t\to0$, gives

$$
f'=\frac{u_y+iv_y}{i}=v_y-iu_y.
$$

These directional limits establish existence of the displayed partial derivatives. Equating their real and imaginary parts gives **the Cauchy-Riemann equations**

$$
\boxed{u_x=v_y,\qquad u_y=-v_x.}
$$

The argument applies at every point of the given open domain; it does not assume continuity of the partial derivatives beforehand.

## 8B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8b/solution">Solution</h3>

↑ **Parent:** [8B](#8b)

For a [bilinear form](../../../linear-algebra.md#bilinear-form) $\phi$, define $F_\phi:V\to V^*$ by $F_\phi(v)(u)=\phi(u,v)$. Bilinearity makes $F_\phi(v)$ a linear functional and makes $F_\phi$ linear in $v$. Conversely, every linear $F:V\to V^*$ defines a bilinear form by $\phi_F(u,v)=F(v)(u)$. These constructions undo each other, giving the desired bijective correspondence.

For a [nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form), $F_\phi$ has zero kernel and is an isomorphism because $V$ and its [dual space](../../../linear-algebra.md#dual-space) have the same finite dimension. For the two forms, put

$$
\boxed{\alpha=F_{\phi_1}^{-1}F_{\phi_2}.}
$$

It is an isomorphism and satisfies $\phi_1(u,\alpha v)=F_{\phi_1}(\alpha v)(u)=F_{\phi_2}(v)(u)=\phi_2(u,v)$ for all $u,v$. This is the [representation of a bilinear form relative to a nondegenerate bilinear form](../../../linear-algebra.md#representation-of-a-bilinear-form-relative-to-a-nondegenerate-bilinear-form).

If both forms are symmetric, then

$$
\phi_1(u,\alpha v)=\phi_2(u,v)=\phi_2(v,u)=\phi_1(v,\alpha u)=\phi_1(\alpha u,v).
$$

Nondegeneracy makes the adjoint with respect to $\phi_1$ unique; this equality proves **$\boxed{\alpha^\dagger=\alpha}$** in that bilinear-form sense. No positivity or Hermitian conjugation is assumed over the arbitrary field.

## 9F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9f/solution">Solution</h3>

↑ **Parent:** [9F](#9f)

For $H=p^2/(2m)+V(x)$ and a time-independent operator $O$, differentiate its [expectation value](../../../quantum-mechanics.md#expectation-value) and use the [Schrödinger equation](../../../physics.md#schrodinger-equation) and its adjoint. Moving $H$ across the inner product by integration by parts gives

$$
\frac{d}{dt}\langle O\rangle=\frac{i}{\hbar}\langle HO-OH\rangle=\frac{i}{\hbar}\langle[H,O]\rangle.
$$

Work with wavefunctions in the displayed operators' domains; the vanishing at infinity removes the associated boundary terms. This is the [Ehrenfest theorem](../../../quantum-mechanics.md#ehrenfest-theorem) derived from time evolution.

The [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation) follows directly from differentiating $x\psi$: $[p,x]\psi=-i\hbar\psi$. Thus $[p^2,x]=p[p,x]+[p,x]p=-2i\hbar p$, while $[V(x),x]=0$. It follows that

$$
\boxed{\frac{d}{dt}\langle x\rangle=\frac{\langle p\rangle}{m}.}
$$

For the momentum equation, apply both products to a test wavefunction:

$$
[V,p]\psi=-i\hbar V\psi'+i\hbar(V\psi)'=i\hbar V'\psi.
$$

The kinetic term commutes with $p$, so $[H,p]=i\hbar V'$. Therefore

$$
\boxed{\frac{d}{dt}\langle p\rangle=-\langle V'(x)\rangle.}
$$

These are the [classical equations from Ehrenfest theorem](../../../quantum-mechanics.md#classical-equations-from-ehrenfest-theorem) for position and momentum expectations; the force expectation need not equal the force evaluated at the expected position.

## 10A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10a/solution">Solution</h3>

↑ **Parent:** [10A](#10a)

A metric space is [totally bounded](../../../topological-analysis.md#totally-bounded-space) if, for every $\epsilon>0$, finitely many open balls of radius $\epsilon$ cover it. The Bolzano-Weierstrass property here means that every sequence has a subsequence converging to a point of the space, namely [sequential compactness](../../../geometry-and-topology.md#sequentially-compact-space).

First suppose that property holds. A [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) has a convergent subsequence with limit $x$ in the space. Given $\epsilon>0$, choose an index after which all sequence terms lie within $\epsilon/2$ of each other, and a subsequence term beyond that index within $\epsilon/2$ of $x$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) then puts every subsequent term within $\epsilon$ of $x$. Thus the whole Cauchy sequence converges, proving completeness.

If total boundedness failed, some $\epsilon>0$ would admit no finite ball cover. Choose points inductively outside the union of the $\epsilon$-balls about previously chosen points. Distinct sequence terms then have distance at least $\epsilon$. No subsequence can be Cauchy, and therefore none can converge, a contradiction. This proves total boundedness.

Conversely, suppose the space is complete and totally bounded. For any sequence, cover the space by finitely many radius-$2^{-1}$ balls and retain the infinitely many indices in one ball. Within those indices, a finite cover by radius-$2^{-2}$ balls retains an infinite subset in one smaller ball. Repeat with radii $2^{-k}$ to obtain nested infinite index sets $I_k$. Choose increasing indices $n_k\in I_k$. For $l,j\ge k$, both terms lie in the ball selected at step $k$, so

$$
d(x_{n_l},x_{n_j})<2^{1-k}.
$$

The subsequence is Cauchy and completeness makes it converge within the space. Hence **the Bolzano-Weierstrass property is equivalent to completeness plus total boundedness**.

## 11G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11g/solution">Solution</h3>

↑ **Parent:** [11G](#11g)

An [isotropic tensor](../../../linear-algebra.md#isotropic-tensor) has unchanged components under every rotation: for rank four, $A_{ijkl}=R_{ia}R_{jb}R_{kc}R_{ld}A_{abcd}$. Orthogonality gives $R_{ia}R_{ja}=\delta_{ij}$, so each product of paired [Kronecker deltas](../../../linear-algebra.md#kronecker-delta) is invariant. Every linear combination of $\delta_{ij}\delta_{kl}$, $\delta_{ik}\delta_{jl}$ and $\delta_{il}\delta_{jk}$ is therefore isotropic, for arbitrary coefficients.

For the integral, differentiation away from the origin gives

$$
\partial_k\partial_l\frac1r=\frac{3x_kx_l}{r^5}-\frac{\delta_{kl}}{r^3}.
$$

After multiplication by $x_ix_j$, this behaves as $O(r^{-1})$ and is locally integrable in three dimensions. Interpret the integral as the limit with a small central ball removed. A rotation preserves the integration ball and the radial kernel, so the resulting $B$ is an [isotropic tensor integral](../../../geometry-and-topology.md#isotropic-tensor-integral). The symmetries $i\leftrightarrow j$ and $k\leftrightarrow l$ force the two cross-pair coefficients equal:

$$
B_{ijkl}=A\delta_{ij}\delta_{kl}+B(\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}).
$$

Taking the trace in $k,l$ uses $\nabla^2(r^{-1})=0$ off the origin and gives $3A+2B=0$. For the other contraction, the displayed Hessian gives $\sum_{ij}x_ix_j\partial_i\partial_j(r^{-1})=2/r$. Thus

$$
3A+12B=\int_{r<a}\frac2r\,dV=8\pi\int_0^a r\,dr=4\pi a^2.
$$

Solving gives $B=2\pi a^2/5$ and $A=-4\pi a^2/15$. Therefore **the requested tensor is**

$$
\boxed{B_{ijkl}=\frac{2\pi a^2}{15}\left(-2\delta_{ij}\delta_{kl}+3\delta_{ik}\delta_{jl}+3\delta_{il}\delta_{jk}\right).}
$$

This is the [quadratically weighted inverse-radius Hessian integral](../../../geometry-and-topology.md#quadratically-weighted-inverse-radius-hessian-integral). The origin creates no extra contribution to this weighted integral; even the distributional point term in the unweighted Hessian is annihilated by $x_ix_j$.

## 12D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12d/solution">Solution</h3>

↑ **Parent:** [12D](#12d)

For a [generalized likelihood-ratio test](../../../statistical-modelling.md#generalized-likelihood-ratio-test), maximize the [likelihood](../../../statistical-modelling.md#likelihood-function) separately over the null parameter space and the unrestricted space. Define $\Lambda=\sup_{H_0}L/\sup L\le1$, and reject for small $\Lambda$, equivalently large $T=-2\log\Lambda$. Choose the rejection threshold to achieve the desired null significance level, using an exact distribution when available or a justified asymptotic calibration; nuisance parameters are fitted under the respective restrictions.

For independent [Poisson distributions](../../../discrete-probability-distribution.md#poisson-distribution), the likelihood is $L=\prod_i e^{-\lambda_i}\lambda_i^{X_i}/X_i!$. The unrestricted maximizers are $\widehat\lambda_i=X_i$, allowing zero as a boundary value. Under the common-mean null, maximizing $e^{-n\lambda}\lambda^{\sum_iX_i}$ gives $\widehat\lambda=\bar X$. The exponential and factorial factors cancel in the ratio, yielding

$$
\boxed{\Lambda=\prod_{i:X_i>0}\left(\frac{\bar X}{X_i}\right)^{X_i},\qquad T=-2\log\Lambda=2\sum_{i:X_i>0}X_i\log\frac{X_i}{\bar X}.}
$$

If all counts are zero, set $\Lambda=1$ and $T=0$; no division by $\bar X$ is then needed.

For positive $\bar X$, put $X_i=\bar X+\delta_i$, so $\sum_i\delta_i=0$. Expanding the logarithm gives

$$
(\bar X+\delta_i)\log(1+\delta_i/\bar X)=\delta_i+\frac{\delta_i^2}{2\bar X}+O(|\delta_i|^3/\bar X^2).
$$

Consequently

$$
\boxed{T=\frac1{\bar X}\sum_i(X_i-\bar X)^2+O\!\left(\frac{\sum_i|X_i-\bar X|^3}{\bar X^2}\right).}
$$

It is the [quadratic Pearson approximation to the Poisson deviance](../../../statistical-modelling.md#quadratic-pearson-approximation-to-the-poisson-deviance). The approximated statistic is the logarithmic ratio $T$, not the bounded raw ratio $\Lambda$.

Under the null in the large-common-count regime, this statistic has an approximate [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with $n-1$ degrees of freedom: fitting the common mean removes one independent residual direction. For $n=7$, use six degrees of freedom. At $T=27.3$, the upper-tail probability in that approximation is

$$
P(\chi_6^2\ge27.3)=e^{-13.65}\left(1+13.65+\frac{13.65^2}{2}\right)\simeq1.27\times10^{-4}.
$$

Thus **reject the equal-mean null at conventional 5% or 1% significance levels**, provided the expected counts justify the chi-square approximation. No particular significance level or common count was supplied, so the numerical decision is stated with those assumptions.

## 13A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="13a/solution">Solution</h3>

↑ **Parent:** [13A](#13a)

The [Liouville theorem](../../../complex-analysis.md#liouville-theorem) states that every bounded [entire function](../../../complex-analysis.md#entire-function) is constant. Let $|f(z)|\le M$ and choose distinct $a,b$. For $R>\max(|a|,|b|)$, partial fractions and the [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula) give

$$
I_R=\int_{|z|=R}\frac{f(z)}{(z-a)(z-b)}\,dz
=\frac{2\pi i}{a-b}[f(a)-f(b)],
$$

with the circle traversed anticlockwise. On that circle,

$$
|I_R|\le\frac{2\pi RM}{(R-|a|)(R-|b|)}\longrightarrow0.
$$

The displayed difference is independent of $R$, so $f(a)=f(b)$. Since $a,b$ were arbitrary, **$f$ is constant**. This proves the theorem with the requested two-pole contour rather than assuming it.

<h3 id="13a/i">i</h3>

↑ **Parent:** [13A](#13a)

<h4 id="13a/i/solution">Solution</h4>

↑ **Parent:** [I](#13a/i)

Set $F(z)=\exp[-(1-i)g(z)]$. It is entire, and $\operatorname{Re}[(1-i)g]=u+v$ makes $|F|=e^{-(u+v)}\le1$. By the just-proved [Liouville theorem](../../../complex-analysis.md#liouville-theorem), $F$ is constant. Differentiation gives $0=F'=-(1-i)g'F$. The exponential never vanishes, so $g'=0$ everywhere and **$g$ is constant**. This is the [entire function confined to a half-plane is constant](../../../complex-analysis.md#entire-function-confined-to-a-half-plane-is-constant) principle.

<h3 id="13a/ii">ii</h3>

↑ **Parent:** [13A](#13a)

<h4 id="13a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#13a/ii)

Set $F(z)=\exp(ig(z)^2)$. Since $\operatorname{Im}(g^2)=2uv$, its modulus is $e^{-2uv}\le1$. The [Liouville theorem](../../../complex-analysis.md#liouville-theorem) again makes $F$ constant, and $F'=2igg'F=0$ implies $(g^2)'=0$. Hence $g^2$ is a constant $c$. If $c=0$, then $g=0$. If $c\ne0$, then $g$ never vanishes and $gg'=0$ implies $g'=0$. In either case **$g$ is constant**. This is also an application of the [one-sided product bound for an entire function](../../../complex-analysis.md#one-sided-product-bound-for-an-entire-function) after rotating $g$ by $i$.

## 14E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="14e/a">a</h3>

↑ **Parent:** [14E](#14e)

<h4 id="14e/a/solution">Solution</h4>

↑ **Parent:** [A](#14e/a)

For a real [symmetric positive-definite matrix](../../../linear-algebra.md#symmetric-positive-definite-matrix), the [Cholesky decomposition](../../../linear-algebra.md#cholesky-decomposition) is $B=R^TR$, where $R$ is upper triangular with positive diagonal; equivalently $B=LL^T$ with $L=R^T$ lower triangular.

Existence can be proved by induction. Write $B=\begin{pmatrix}b&v^T\\v&C\end{pmatrix}$, where $b>0$. For a nonzero vector $z$, evaluate the quadratic form at $(-v^Tz/b,z)^T$ to obtain $z^T(C-vv^T/b)z>0$. The [Schur complement](../../../linear-algebra.md#schur-complement) is therefore positive definite. By induction it has factor $R_0^TR_0$, and

$$
R=\begin{pmatrix}\sqrt b&v^T/\sqrt b\\0&R_0\end{pmatrix}
$$

has $R^TR=B$. The one-dimensional starting case is the positive square root.

For uniqueness, if $R_1^TR_1=R_2^TR_2=B$, then $U=R_2R_1^{-1}$ is upper triangular and satisfies $U^TU=I$. Since $U^{-1}$ is upper triangular and equals $U^T$, which is lower triangular, $U$ is diagonal. Orthogonality makes its diagonal entries $\pm1$, and positivity of the diagonals of $R_1,R_2$ forces $+1$. Hence $U=I$ and **$\boxed{R_1=R_2}$**.

<h3 id="14e/b">b</h3>

↑ **Parent:** [14E](#14e)

<h4 id="14e/b/solution">Solution</h4>

↑ **Parent:** [B](#14e/b)

Full column rank makes $B=A^TA$ positive definite: for nonzero $v$, $v^TBv=\|Av\|^2>0$. Let $B=R^TR$ be its unique upper-triangular [Cholesky decomposition](../../../linear-algebra.md#cholesky-decomposition) with positive diagonal. Defining $Q=AR^{-1}$ gives

$$
Q^TQ=R^{-T}A^TAR^{-1}=I,\qquad A=QR.
$$

Thus the skinny [QR decomposition](../../../linear-algebra.md#qr-decomposition) exists. If $A=\widetilde Q\widetilde R$ is another such decomposition, orthonormality gives $A^TA=\widetilde R^T\widetilde R$. Cholesky uniqueness forces $\widetilde R=R$, and then $\widetilde Q=AR^{-1}=Q$. Therefore **the skinny factorization with positive diagonal is unique**. This is the [thin QR factorization from Cholesky decomposition](../../../linear-algebra.md#thin-qr-factorization-from-cholesky-decomposition); no inverse of the rectangular $Q$ is assumed.

## 15C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="15c/solution">Solution</h3>

↑ **Parent:** [15C](#15c)

The algebraic [dual space](../../../linear-algebra.md#dual-space) is $V^*=\operatorname{Hom}_k(V,k)$, the vector space of linear functionals. For an ordered [basis](../../../vector-space.md#basis) $v_1,\ldots,v_n$, define the [dual basis](../../../linear-algebra.md#dual-basis) by $v^i(v_j)=\delta_{ij}$, equivalently $v^i(\sum_jx_jv_j)=x_i$. Every functional satisfies $\ell=\sum_i\ell(v_i)v^i$, proving spanning. Evaluating a zero linear combination on each $v_j$ forces every coefficient to vanish, proving independence.

For a [linear map](../../../vector-space.md#linear-map) $\alpha:V\to W$, its [dual map](../../../linear-algebra.md#transpose-of-a-linear-map) is $\alpha^*:W^*\to V^*$, $\alpha^*(\ell)=\ell\circ\alpha$. Suppose the matrix of $\alpha$ satisfies $\alpha(v_i)=\sum_jA_{ji}w_j$. Then

$$
\alpha^*(w^j)(v_i)=w^j(\alpha(v_i))=A_{ji}.
$$

These are the $i$th coordinates of $\alpha^*(w^j)$ in the dual basis, so **the dual matrix is** $\boxed{A^T}$. For complex vector spaces this is still an ordinary transpose, because the algebraic dual uses linear functionals, not conjugate-linear ones.

To prove equality of ranks directly, $\ker\alpha^*$ consists precisely of functionals on $W$ vanishing on $\operatorname{im}\alpha$, its [annihilator](../../../module-theory.md#annihilator-ring-theory). A basis of the image extends to a basis of $W$; such functionals have zero values on the image basis and arbitrary values on the remaining $\dim W-\operatorname{rank}\alpha$ vectors. Thus $\dim\ker\alpha^*=\dim W-\operatorname{rank}\alpha$. The [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) gives

$$
\boxed{\operatorname{rank}\alpha^*=\operatorname{rank}\alpha.}
$$

Finally, if $\alpha$ is invertible, for every $\ell\in V^*$ the two compositions give $(\ell\circ\alpha^{-1})\circ\alpha=\ell$ and $(\ell\circ\alpha)\circ\alpha^{-1}=\ell$. Hence the two dual maps are mutual inverses and

$$
\boxed{(\alpha^*)^{-1}=(\alpha^{-1})^*.}
$$

## 16E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="16e/solution">Solution</h3>

↑ **Parent:** [16E](#16e)

For a [rational function](../../../isolated-singularity.md#rational-function), the stipulated decay implies $R(z)=O(|z|^{-2})$ at infinity, unless it vanishes identically. Thus its real-line integral converges absolutely. Close the segment $[-T,T]$ with an upper semicircle, choosing $T$ beyond all finite poles. The arc contribution has modulus at most $\pi T\sup_{|z|=T}|R(z)|=O(T^{-1})$, tending to zero. The [residue theorem](../../../analysis.md#residue-theorem) therefore gives

$$
\boxed{\int_{-\infty}^{\infty}R(x)\,dx=2\pi i\sum_{\operatorname{Im}z_j>0}\operatorname{Res}_{z=z_j}R(z).}
$$

There are no real poles requiring indentations.

Apply this to $R(z)=1/(1+z^{2n})$. Its upper-half-plane poles are $\zeta_k=e^{i(2k+1)\pi/(2n)}$, $k=0,\ldots,n-1$, all simple. Since $\zeta_k^{2n}=-1$, their residues are

$$
\operatorname{Res}_{\zeta_k}R=\frac1{2n\zeta_k^{2n-1}}=-\frac{\zeta_k}{2n}.
$$

For $\theta=\pi/(2n)$, the finite [geometric series](../../../real-analysis.md#geometric-series) gives

$$
\sum_{k=0}^{n-1}\zeta_k=e^{i\theta}\frac{1-e^{i\pi}}{1-e^{2i\theta}}=\frac{i}{\sin\theta}.
$$

The full real-line integral is consequently $\pi/[n\sin(\pi/(2n))]$. Its integrand is even, so **the requested half-line integral is**

$$
\boxed{\int_0^\infty\frac{dx}{1+x^{2n}}=\frac{\pi}{2n}\csc\frac{\pi}{2n}.}
$$

## 17B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="17b/solution">Solution</h3>

↑ **Parent:** [17B](#17b)

The [Legendre symbol](../../../number-theory.md#legendre-symbol) $(a/p)$ is $+1$ when $a$ is a nonzero square modulo the odd prime $p$, $-1$ when it is not a square, and $0$ when $p\mid a$. For the coprime case, [Euler's criterion](../../../number-theory.md#euler-s-criterion) states

$$
\boxed{a^{(p-1)/2}\equiv\left(\frac ap\right)\pmod p.}
$$

Write $h=(p-1)/2$. For $1\le j\le h$, the balanced residues $r_j$ are nonzero and their absolute values lie in $\{1,\ldots,h\}$. If $|r_j|=|r_k|$, then $aj\equiv\pm ak\pmod p$. Cancel $a$. The plus sign forces $j=k$; the minus sign would require $j+k=p$, impossible because $j+k\le p-1$. Thus the absolute residues form a permutation of $1,\ldots,h$. If exactly $l$ are negative, multiplying gives

$$
a^h h!\equiv\prod_{j=1}^h r_j=(-1)^l h!\pmod p.
$$

Since $p$ does not divide $h!$, cancellation and [Euler's criterion](../../../number-theory.md#euler-s-criterion) prove [Gauss's lemma](../../../number-theory.md#gauss-s-lemma-number-theory):

$$
\boxed{\left(\frac ap\right)=(-1)^l.}
$$

The two signs are distinct modulo the odd prime, so this congruence identifies the integer symbol itself.

For $a=2$, the balanced representative of $2j$ is negative precisely when $j>p/4$, giving $l=(p-1)/2-\lfloor p/4\rfloor$. Checking the four odd residue classes modulo eight gives even $l$ for $p\equiv1,7$ and odd $l$ for $p\equiv3,5$. Hence

$$
\boxed{2\text{ is a quadratic residue modulo }p\iff p\equiv1\text{ or }7\pmod8.}
$$

This is the [quadratic character of two](../../../number-theory.md#second-supplementary-law-for-quadratic-reciprocity) obtained from the lemma.

Let $P=p_1\cdots p_m$ and $N=8P^2-1$. If a prime $q$ divides $N$, then $q$ is odd and cannot divide $P$. Moreover

$$
(4P)^2=16P^2=2(N+1)\equiv2\pmod q,
$$

so $2$ has an explicit nonzero square root modulo $q$. The criterion just proved forces every prime divisor of $N$ into the classes $1$ or $7$ modulo eight. But $N\equiv7\pmod8$: if all its prime factors were $1$ modulo eight, their product, with multiplicities, would also be $1$. Thus at least one prime divisor is $7$ modulo eight. No listed $p_i$ divides $N$, because $N\equiv-1\pmod{p_i}$. This always produces another such prime, proving **infinitely many primes are congruent to seven modulo eight**, the [Euclid proof for infinitely many primes congruent to seven modulo eight](../../../number-theory.md#euclid-proof-for-infinitely-many-primes-congruent-to-seven-modulo-eight).

## 18F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="18f/a">a</h3>

↑ **Parent:** [18F](#18f)

<h4 id="18f/a/solution">Solution</h4>

↑ **Parent:** [A](#18f/a)

The [orbital angular momentum](../../../quantum-mechanics.md#orbital-angular-momentum) operators are

$$
\boxed{L_1=x_2p_3-x_3p_2,\qquad L_2=x_3p_1-x_1p_3,\qquad L_3=x_1p_2-x_2p_1.}
$$

On smooth wavefunctions, $[x_i,p_j]=i\hbar\delta_{ij}$, while position operators commute with each other and momentum operators commute with each other. Applying the product rule for [commutators](../../../lie-algebra.md#commutator) gives

$$
[x_ip_j,x_kp_l]=-i\hbar\delta_{jk}x_ip_l+i\hbar\delta_{il}x_kp_j.
$$

Use it on the four terms in $[L_1,L_2]$: only $[x_2p_3,x_3p_1]=-i\hbar x_2p_1$ and $[x_3p_2,x_1p_3]=i\hbar x_1p_2$ survive, with the latter entering positively from the two minus signs. Therefore

$$
\boxed{[L_1,L_2]=i\hbar L_3.}
$$

The cyclic versions similarly give $[L_3,L_1]=i\hbar L_2$ and $[L_3,L_2]=-i\hbar L_1$. Thus, for $L_\pm=L_1\pm iL_2$,

$$
\boxed{[L_3,L_\pm]=\pm\hbar L_\pm.}
$$

Now define $L^2=L_1^2+L_2^2+L_3^2$. For each $i$,

$$
[L^2,L_i]=i\hbar\sum_{j,k}\epsilon_{jik}(L_jL_k+L_kL_j)=0,
$$

because the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) is antisymmetric in $j,k$ and the operator pair is symmetric. Linearity then gives **$\boxed{[L^2,L_\pm]=0}$**. The PDF superscript here is the squared total angular momentum, not the component $L_2$.

<h3 id="18f/b">b</h3>

↑ **Parent:** [18F](#18f)

<h4 id="18f/b/solution">Solution</h4>

↑ **Parent:** [B](#18f/b)

Every [orbital angular momentum](../../../quantum-mechanics.md#orbital-angular-momentum) operator annihilates a radial function: substituting $\partial_i f(r)=f'(r)x_i/r$ makes the two terms cancel. It also annihilates $r^2$. Thus the radial factor can be carried through the angular operators. Since $x_3^2$ is independent of $x_1,x_2$, $L_3\psi=0$ for every value of $a$.

Direct differentiation gives

$$
L_1^2x_3^2=2\hbar^2(x_3^2-x_2^2),\qquad
L_2^2x_3^2=2\hbar^2(x_3^2-x_1^2),\qquad L_3^2x_3^2=0.
$$

Consequently $L^2x_3^2=\hbar^2(6x_3^2-2r^2)$ and $L^2r^2=0$. For a nonzero admissible radial factor, comparison with $\lambda(x_3^2+ar^2)f(r)$ forces $\lambda=6\hbar^2$ and $6a=-2$. Therefore **the simultaneous eigenfunction occurs at**

$$
\boxed{a=-\frac13,\qquad L^2\psi=6\hbar^2\psi,\qquad L_3\psi=0.}
$$

It is the [axially symmetric quadratic orbital eigenfunction](../../../quantum-mechanics.md#axially-symmetric-quadratic-orbital-eigenfunction), with quantum numbers $l=2$, $m=0$ and angular dependence proportional to the [spherical harmonic](../../../analysis.md#spherical-harmonic) $Y_{20}$. The subtraction of $r^2/3$ removes its rotationally invariant scalar component.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
