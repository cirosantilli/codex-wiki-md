# Paper 1

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2025/paperib_1_2025.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2025/paperib_1_2025.pdf)

**Table of contents**

- [1F](#1f)
  - [Solution](#1f/solution)
- [2F](#2f)
  - [Solution](#2f/solution)
- [3](#3)
  - [3.1G](#3/3-1g)
    - [Solution](#3/3-1g/solution)
  - [3.2A](#3/3-2a)
    - [a](#3/3-2a/a)
      - [Solution](#3/3-2a/a/solution)
    - [b](#3/3-2a/b)
      - [Solution](#3/3-2a/b/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5A](#5a)
  - [a](#5a/a)
    - [Solution](#5a/a/solution)
  - [b](#5a/b)
    - [Solution](#5a/b/solution)
- [6H](#6h)
  - [Solution](#6h/solution)
- [7H](#7h)
  - [a](#7h/a)
    - [Solution](#7h/a/solution)
  - [b](#7h/b)
    - [Solution](#7h/b/solution)
- [8F](#8f)
  - [Solution](#8f/solution)
- [9E](#9e)
  - [a](#9e/a)
    - [Solution](#9e/a/solution)
  - [b](#9e/b)
    - [Solution](#9e/b/solution)
  - [c](#9e/c)
    - [i](#9e/c/i)
      - [Solution](#9e/c/i/solution)
    - [ii](#9e/c/ii)
      - [Solution](#9e/c/ii/solution)
- [10G](#10g)
  - [Solution](#10g/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12](#12)
  - [12.1G](#12/12-1g)
    - [Solution](#12/12-1g/solution)
    - [i](#12/12-1g/i)
      - [Solution](#12/12-1g/i/solution)
    - [ii](#12/12-1g/ii)
      - [Solution](#12/12-1g/ii/solution)
  - [12.2A](#12/12-2a)
    - [a](#12/12-2a/a)
      - [Solution](#12/12-2a/a/solution)
    - [b](#12/12-2a/b)
      - [i](#12/12-2a/b/i)
        - [Solution](#12/12-2a/b/i/solution)
      - [ii](#12/12-2a/b/ii)
        - [Solution](#12/12-2a/b/ii/solution)
- [13B](#13b)
  - [a](#13b/a)
    - [Solution](#13b/a/solution)
  - [b](#13b/b)
    - [Solution](#13b/b/solution)
- [14C](#14c)
  - [Solution](#14c/solution)
- [15B](#15b)
  - [Solution](#15b/solution)
- [16D](#16d)
  - [Solution](#16d/solution)
  - [i](#16d/i)
    - [Solution](#16d/i/solution)
  - [ii](#16d/ii)
    - [Solution](#16d/ii/solution)
- [17A](#17a)
  - [a](#17a/a)
    - [Solution](#17a/a/solution)
  - [b](#17a/b)
    - [Solution](#17a/b/solution)
  - [c](#17a/c)
    - [Solution](#17a/c/solution)
  - [d](#17a/d)
    - [Solution](#17a/d/solution)
- [18H](#18h)
  - [a](#18h/a)
    - [Solution](#18h/a/solution)
  - [b](#18h/b)
    - [Solution](#18h/b/solution)
  - [c](#18h/c)
    - [Solution](#18h/c/solution)
  - [d](#18h/d)
    - [Solution](#18h/d/solution)
- [19H](#19h)
  - [a](#19h/a)
    - [Solution](#19h/a/solution)
  - [b](#19h/b)
    - [Solution](#19h/b/solution)
  - [c](#19h/c)
    - [Solution](#19h/c/solution)
  - [d](#19h/d)
    - [Solution](#19h/d/solution)

## 1F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1f/solution">Solution</h3>

↑ **Parent:** [1F](#1f)

The Leibniz definition is

$$
\det A=\sum_{\pi\in S_n}\operatorname{sgn}(\pi)\prod_{i=1}^nA_{i,\pi(i)}.
$$

The adjugate is the transpose of the cofactor [matrix](../../../vector-space.md#matrix). Cofactor expansion gives

$$
A\operatorname{adj}(A)=\operatorname{adj}(A)A=(\det A)I.
$$

For the displayed tridiagonal [matrix](../../../vector-space.md#matrix), expansion along the last row gives $D_n=2D_{n-1}-D_{n-2}$, with $D_1=2,D_2=3$. Induction yields

$$
\boxed{\det A_n=D_n=n+1.}
$$

## 2F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2f/solution">Solution</h3>

↑ **Parent:** [2F](#2f)

In local coordinates $u=(u^1,u^2)$ with metric $g_{ij}=\partial_i\sigma\cdot\partial_j\sigma$, the energy is

$$
E(\gamma)=\frac12\int_a^b g_{ij}(u)\dot u^i\dot u^j\,dt.
$$

The Euler–Lagrange equations are equivalently

$$
\ddot u^k+\Gamma^k_{ij}\dot u^i\dot u^j=0,
$$

where $\Gamma^k_{ij}=\tfrac12g^{k\ell}(\partial_i g_{j\ell}+\partial_jg_{i\ell}-\partial_\ell g_{ij})$.

For the plane-section curve $\eta$, constant speed gives $\eta''\perp\eta'$. Both $\eta''$ and the surface normal lie in $P$, while $P$ is spanned by $\eta'$ and that normal along the intersection. Hence $\eta''$ is normal to the surface. Its tangential [acceleration](../../../classical-mechanics.md#acceleration) vanishes, which is the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation).

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/3-1g">3.1G</h3>

↑ **Parent:** [3](#3)

<h4 id="3/3-1g/solution">Solution</h4>

↑ **Parent:** [3.1G](#3/3-1g)

Jordan's lemma states that if $f$ is holomorphic in the upper half-plane apart from finitely many poles and $|f(z)|\le M/|z|$ on sufficiently large upper semicircles, then for $a>0$ the [integral](../../../calculus.md#integral) of $e^{iaz}f(z)$ over those arcs tends to zero. Indeed, split the arc away from its endpoints, where exponential decay is uniform, and bound the two short endpoint arcs using $|e^{iaRe^{i\theta}}|=e^{-aR\sin\theta}$ and $\sin\theta\ge2\theta/\pi$ on $[0,\pi/2]$.

Apply the upper semicircle to $ze^{iz}/(1+z^2)$. The sole enclosed pole is $i$, with residue $e^{-1}/2$. Therefore the contour [integral](../../../calculus.md#integral) is $\pi i/e$; taking imaginary parts gives

$$
\boxed{\int_{-\infty}^{\infty}\frac{x\sin x}{1+x^2}\,dx=\frac\pi e.}
$$

<h3 id="3/3-2a">3.2A</h3>

↑ **Parent:** [3](#3)

<h4 id="3/3-2a/a">a</h4>

↑ **Parent:** [3.2A](#3/3-2a)

<h5 id="3/3-2a/a/solution">Solution</h5>

↑ **Parent:** [A](#3/3-2a/a)

If $f$ is meromorphic inside and on a positively oriented simple closed contour $C$, with no pole on $C$, then

$$
\boxed{\oint_Cf(z)\,dz=2\pi i\sum_{a\text{ inside }C}\operatorname{Res}(f,a).}
$$

<h4 id="3/3-2a/b">b</h4>

↑ **Parent:** [3.2A](#3/3-2a)

<h5 id="3/3-2a/b/solution">Solution</h5>

↑ **Parent:** [B](#3/3-2a/b)

Integrate $e^{inz}/(z^4+1)$ over the upper semicircle. Jordan's lemma removes the arc and the upper poles are $e^{i\pi/4}$ and $e^{3i\pi/4}$. Summing their residues and taking real parts gives

$$
\boxed{\int_{-\infty}^{\infty}\frac{\cos(nx)}{x^4+1}\,dx
=\frac\pi{\sqrt2}e^{-n/\sqrt2}\left(\cos\frac n{\sqrt2}+\sin\frac n{\sqrt2}\right).}
$$

## 4C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

For every [tangent vector](../../../differential-geometry.md#tangent-vector) $v\perp x_0$, stationarity of $Q$ on the sphere gives $2v^TAx_0=0$. Hence $Ax_0$ is parallel to $x_0$, say $Ax_0=Ex_0$. Taking the [inner product](../../../linear-algebra.md#inner-product) with $x_0$ gives $E=Q(x_0)$. The spectral theorem shows that this is the largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue).

For $A=\begin{pmatrix}1&t\\t&1\end{pmatrix}$ the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $1\pm t$, so

$$
E(t)=1+|t|.
$$

Its graph is a V translated upward and is convex.

## 5A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5a/a">a</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/a/solution">Solution</h4>

↑ **Parent:** [A](#5a/a)

The [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem) says that a consistent linear multistep method is convergent exactly when it is zero-stable.

<h3 id="5a/b">b</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/b/solution">Solution</h4>

↑ **Parent:** [B](#5a/b)

The first characteristic [polynomial](../../../polynomial.md) factors as

$$
\rho(z)=z^3+(2\alpha-3)(z^2-z)-1
=(z-1)\{z^2+(2\alpha-2)z+1\}.
$$

The root condition holds precisely for $0<\alpha<2$: in this range the two reciprocal roots are distinct and on the unit circle; at either endpoint a unit root is repeated, and outside it one root has [modulus](../../../complex-analysis.md#modulus) greater than one. Consistency is given, so these and only these values are convergent. The exceptional order-three value $\alpha=6$ is outside this interval; consequently every convergent case has order two.

## 6H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6h/solution">Solution</h3>

↑ **Parent:** [6H](#6h)

The Neyman–Pearson lemma says that among tests of size at most $\alpha$ for two simple hypotheses, a [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) rejecting where $p(x;\theta_1)/p(x;\theta_0)>k$ is most powerful, with boundary randomisation if required. If $\varphi$ is that test and $\psi$ any competing test, choose $k$ so the sizes agree. Pointwise,

$$
(\varphi-\psi)(p_1-kp_0)\ge0.
$$

Integration and the size inequality yield $E_1\varphi\ge E_1\psi$.

Here

$$
\frac{p(x;\theta_1)}{p(x;\theta_0)}=\frac{\theta_1}{\theta_0}e^{-(\theta_1-\theta_0)|x|},
$$

which decreases with $|x|$. Thus reject for $|X|\le c$, where

$$
\boxed{\alpha=P_{\theta_0}(|X|\le c)=1-e^{-\theta_0c},\qquad
c=-\frac1{\theta_0}\log(1-\alpha).}
$$

## 7H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7h/a">a</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/a/solution">Solution</h4>

↑ **Parent:** [A](#7h/a)

Multiplying $Ax\le b$ by $y\ge0$ gives the upper bound $c^Tx\le y^TAx\le y^Tb$ whenever $A^Ty\ge c$. Minimising the bound yields the dual

$$
\boxed{\text{minimise }b^Ty\quad\text{subject to }A^Ty\ge c, y\ge0.}
$$

<h3 id="7h/b">b</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/b/solution">Solution</h4>

↑ **Parent:** [B](#7h/b)

The primal point $x=(1/2,1/2,0)$ is feasible and has value $5/2$. The dual point $y=(1/2,3/2)$ is feasible because

$$
A^Ty=(2,3,13/2)^T\ge(2,3,4)^T,
$$

and has value $2(1/2)+3/2=5/2$. Weak duality proves both are optimal. Thus the requested optimal primal solution is

$$
\boxed{x_1=x_2=\frac12,\qquad x_3=0.}
$$

## 8F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8f/solution">Solution</h3>

↑ **Parent:** [8F](#8f)

For a [linear map](../../../vector-space.md#linear-map) $T:V\to W$ with $V$ finite-dimensional,

$$
\dim V=\operatorname{rk}T+\dim\ker T.
$$

Now

$$
\operatorname{rk}(\alpha\beta)=\dim\operatorname{im}\beta-dim(\ker\alpha\cap\operatorname{im}\beta)
\ge\operatorname{rk}\beta-\dim\ker\alpha,
$$

which is the required inequality after rank-nullity for $\alpha$.

If $X$ and $Y$ represent the same map, then $Y=C^{-1}XB$, where $B$ changes new domain coordinates to old ones and $C$ does the same in the codomain.

Invertible block row and column operations reduce

$$
\begin{pmatrix}P&Q\\R&S\end{pmatrix}
$$

to $\operatorname{diag}(P,S-RP^{-1}Q)$, proving the rank formula. Apply it to $\begin{pmatrix}I_n&Q\\R&I_m\end{pmatrix}$ first with the upper-left block and then with the lower-right block. Equating the results gives

$$
\boxed{\operatorname{rk}(I_n-QR)=\operatorname{rk}(I_m-RQ)+n-m.}
$$

## 9E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9e/a">a</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/a/solution">Solution</h4>

↑ **Parent:** [A](#9e/a)

Let $k=|G/H|$. The [coset action](../../../group-theory.md#coset-action) gives a nontrivial homomorphism $G\to S_k$ whose kernel is normal. Simplicity makes it injective. The sign map is trivial on the nonabelian simple image, so $G$ embeds in $A_k$. For $k\le4$, $A_k$ is solvable, as are its [subgroups](../../../group.md#subgroup), whereas a nonabelian simple [group](../../../group.md) is not. Hence $k\ge5$.

<h3 id="9e/b">b</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/b/solution">Solution</h4>

↑ **Parent:** [B](#9e/b)

Let $S$ act by conjugation on the Sylow $p$-subgroups. The only fixed point is $S$: if $S$ normalizes another $T$, then $ST$ is a $p$-subgroup, forcing $S=T$. For $T=gSg^{-1}\ne S$, a stabilizer element in $S$ normalizes $T$, hence lies in $T$ by the same argument; the hypothesis then makes it trivial. Every nontrivial orbit therefore has size $|S|$, so

$$
\boxed{n_p\equiv1\pmod{|S|}.}
$$

<h3 id="9e/c">c</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/c/i">i</h4>

↑ **Parent:** [C](#9e/c)

<h5 id="9e/c/i/solution">Solution</h5>

↑ **Parent:** [I](#9e/c/i)

Sylow gives $n_7\mid24$ and $n_7\equiv1\pmod7$. Simplicity excludes $n_7=1$, so $n_7=8$. Distinct order-seven [subgroups](../../../group.md#subgroup) intersect trivially, hence there are

$$
8(7-1)=48
$$

elements of order seven.

<h4 id="9e/c/ii">ii</h4>

↑ **Parent:** [C](#9e/c)

<h5 id="9e/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9e/c/ii)

If all distinct Sylow 2-subgroups met trivially, part (b) would give $n_2\equiv1\pmod8$. But Sylow gives $n_2\mid21$ and $n_2$ odd, so $n_2\in\{3,7,21\}$ after excluding normality, none congruent to one modulo eight. Thus some distinct pair has nontrivial intersection. That intersection is a nontrivial finite 2-group, so Cauchy's theorem supplies an element of order two.

## 10G

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10g/solution">Solution</h3>

↑ **Parent:** [10G](#10g)

Uniform continuity means that for every $\varepsilon>0$ there is a single $\delta>0$ such that $d(x,y)<\delta$ implies $|f(x)-f(y)|<\varepsilon$ for all $x,y$. A $d'$-Cauchy [sequence](../../../real-analysis.md#sequence) converges uniformly pointwise to a [bounded function](../../../function.md#bounded-function); passing a uniform-continuity estimate through a sufficiently close member proves that the [limit](../../../calculus.md#limit-of-a-function) is uniformly continuous. Thus $C_{b,u}(X)$ is complete.

If $f\in C_0(\mathbb R^n)$, decay at infinity and compactness of a ball make it bounded. Uniform continuity on a sufficiently large compact ball, together with small values outside it, proves global uniform continuity. Hence $C_0\subset C_{b,u}$.

A [uniform limit](../../../real-analysis.md#uniform-limit) of [functions](../../../function.md) vanishing at infinity also vanishes at infinity, so $C_0$ is closed. It is not compact: translate a fixed compactly supported bump of height one so that the supports are disjoint. The resulting [sequence](../../../real-analysis.md#sequence) has pairwise sup distance one and no convergent subsequence.

## 11F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

An allowable parametrisation is a smooth homeomorphism from an open subset of $\mathbb R^2$ onto an open subset of $S$, with [derivative](../../../calculus.md#derivative) of rank two. Away from the axis, the rotation orbit has nonzero tangent. A transverse curve supplied by the submanifold theorem, followed by the rotation action, gives

$$
\sigma(u,v)=(f(u)\cos v,f(u)\sin v,g(u)),
$$

with $|v|<\pi$ and $(f',g')\ne(0,0)$.

For a ruled parametrisation, regularity is exactly

$$
\psi_s\times\psi_t=(a'+tb')\times b\ne0.
$$

Rotate and translate along the axis so the specified ruling is

$$
L(t)=(d,st,ct),\qquad d>0.
$$

Here $s\ne0$ because the line is not parallel to the axis, and $c\ne0$: if $c=0$, rotating the horizontal tangent line makes the ruled parametrisation singular at its closest point. Rotating $L$ gives

$$
x^2+y^2=d^2+\frac{s^2}{c^2}z^2,
$$

a [one-sheet hyperboloid](../../../differential-geometry.md#one-sheet-hyperboloid). Rotation invariance puts this whole surface in $\Sigma$. Connectedness and the fact that a complete embedded hyperboloid cannot be a proper subset of another connected embedded surface force equality. Rescaling radial and axial coordinates gives a diffeomorphism with $x^2+y^2=1+z^2$.

## 12

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12/12-1g">12.1G</h3>

↑ **Parent:** [12](#12)

<h4 id="12/12-1g/solution">Solution</h4>

↑ **Parent:** [12.1G](#12/12-1g)

For any circle $|\zeta|=\rho$ with $r<\rho<R$, Cauchy's formula applied inside and outside the circle gives the locally uniformly convergent Laurent expansion

$$
f(z)=\sum_{n=-\infty}^{\infty}a_nz^n,\qquad
a_n=\frac1{2\pi i}\oint_{|\zeta|=\rho}\frac{f(\zeta)}{\zeta^{n+1}}\,d\zeta.
$$

At zero, the singularity is removable exactly when all $a_n$ with $n<0$ vanish; it is a pole of order $k$ when $a_{-k}\ne0$ and $a_n=0$ for $n<-k$; it is essential when infinitely many negative coefficients are nonzero.

<h4 id="12/12-1g/i">i</h4>

↑ **Parent:** [12.1G](#12/12-1g)

<h5 id="12/12-1g/i/solution">Solution</h5>

↑ **Parent:** [I](#12/12-1g/i)

Since $\csc^2z=z^{-2}+1/3+O(z^2)$, the principal parts cancel and $f_1=-1/3+O(z^2)$. The singularity is removable.

<h4 id="12/12-1g/ii">ii</h4>

↑ **Parent:** [12.1G](#12/12-1g)

<h5 id="12/12-1g/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#12/12-1g/ii)

Termwise integration of the exponential [series](../../../real-analysis.md#series-mathematics) gives

$$
f_2(z)=2\sum_{n=0}^{\infty}\frac{(-1)^n}{n!(2n+1)}z^{-2n}.
$$

There are infinitely many negative Laurent coefficients, so zero is an [essential singularity](../../../isolated-singularity.md#essential-singularity).

<h3 id="12/12-2a">12.2A</h3>

↑ **Parent:** [12](#12)

<h4 id="12/12-2a/a">a</h4>

↑ **Parent:** [12.2A](#12/12-2a)

<h5 id="12/12-2a/a/solution">Solution</h5>

↑ **Parent:** [A](#12/12-2a/a)

For distinct $z,w$ in the convex disc, integrate along the segment:

$$
f(z)-f(w)=f'(z_0)(z-w)+\int_w^z(f'(\zeta)-f'(z_0))\,d\zeta.
$$

The second term has [modulus](../../../complex-analysis.md#modulus) strictly below $|f'(z_0)||z-w|$, so the sum cannot vanish. Thus $f$ is one-to-one.

<h4 id="12/12-2a/b">b</h4>

↑ **Parent:** [12.2A](#12/12-2a)

<h5 id="12/12-2a/b/i">i</h5>

↑ **Parent:** [B](#12/12-2a/b)

<h6 id="12/12-2a/b/i/solution">Solution</h6>

↑ **Parent:** [I](#12/12-2a/b/i)

Harmonic means twice continuously [differentiable](../../../analysis.md#differentiable-function) with $u_{xx}+u_{yy}=0$. On the simply connected plane, choose an entire [harmonic conjugate](../../../partial-differential-equation.md#harmonic-conjugate) so $F=u+iv$ is entire. If $u\ge0$, then $e^{-F}$ is bounded; Liouville's theorem makes it, and hence $u$, constant.

<h5 id="12/12-2a/b/ii">ii</h5>

↑ **Parent:** [B](#12/12-2a/b)

<h6 id="12/12-2a/b/ii/solution">Solution</h6>

↑ **Parent:** [Ii](#12/12-2a/b/ii)

Choose an entire $F$ with real part $u$. The bound implies that $e^F$ has at most [polynomial](../../../polynomial.md) growth, so Cauchy's estimates make it a [polynomial](../../../polynomial.md). It has no zeros, hence that [polynomial](../../../polynomial.md) is constant. Therefore $F$, and in particular $u$, is constant.

## 13B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="13b/a">a</h3>

↑ **Parent:** [13B](#13b)

<h4 id="13b/a/solution">Solution</h4>

↑ **Parent:** [A](#13b/a)

Legendre's equation is

$$
-\frac d{dx}\left((1-x^2)y'\right)=\lambda y.
$$

With $\langle f,g\rangle=\int_{-1}^1f\bar g\,dx$, integration by parts has no endpoint term because $1-x^2=0$ there, so the operator is self-adjoint. Sturm–Liouville [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are real, can be ordered increasingly, and their eigenfunctions are orthogonal and complete under standard regularity assumptions.

Substitution of $y=\sum a_nx^n$ gives

$$
\frac{a_{n+2}}{a_n}=\frac{n(n+1)-\lambda}{(n+1)(n+2)}.
$$

The [series](../../../real-analysis.md#series-mathematics) terminates at degree $\ell$ when $\lambda=\ell(\ell+1)$. Normalizing at one gives

$$
\boxed{P_1(x)=x,\qquad P_3(x)=\frac12(5x^3-3x).}
$$

<h3 id="13b/b">b</h3>

↑ **Parent:** [13B](#13b)

<h4 id="13b/b/solution">Solution</h4>

↑ **Parent:** [B](#13b/b)

The separated axisymmetric solution is

$$
\Phi(r,x)=\sum_{\ell=0}^{\infty}(A_\ell r^\ell+B_\ell r^{-\ell-1})P_\ell(x).
$$

Since $x(1-x^2)=\tfrac25(P_1-P_3)$, regularity at the origin and the [boundary condition](../../../differential-equation.md#boundary-condition) give

$$
\boxed{\Phi(r,x)=\frac25\left[\frac rR P_1(x)-\left(\frac rR\right)^3P_3(x)\right].}
$$

## 14C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="14c/solution">Solution</h3>

↑ **Parent:** [14C](#14c)

Write $E=-\hbar^2\kappa^2/(2m)$. An even [bound state](../../../quantum-mechanics.md#bound-state) is proportional to $\cos(kx)$ inside the well and to $e^{-\kappa|x|}$ outside, where

$$
k^2=\frac{m}{a\hbar^2}-\kappa^2.
$$

Continuity of the logarithmic [derivative](../../../calculus.md#derivative) at $a$ gives

$$
\kappa=k\tan(ka).
$$

For sufficiently small $a$, $ka$ lies in the first monotone branch, so this equation has exactly one positive root and the even state is unique up to scale.

As $a\downarrow0$, $\kappa\sim k^2a\to m/\hbar^2$. Hence

$$
E_0=-\frac{m}{2\hbar^2}.
$$

The wells converge distributionally to $V_0(x)=-\delta(x)$, whose normalized even [bound state](../../../quantum-mechanics.md#bound-state) is

$$
\psi_0(x)=\sqrt{\frac m{\hbar^2}}e^{-m|x|/\hbar^2}.
$$

Its [derivative](../../../calculus.md#derivative) jump is precisely the one imposed by the [delta potential](../../../quantum-mechanics.md#delta-potential).

## 15B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="15b/solution">Solution</h3>

↑ **Parent:** [15B](#15b)

Using $\rho=\varepsilon_0\nabla\cdot E$, $E=-\nabla\phi$, integration by parts, and $\phi=0$ on the boundary gives

$$
U=\frac{\varepsilon_0}{2}\int_V|E|^2\,d^3x.
$$

Put $C=q/(4\pi\varepsilon_0)$. [Gauss's law](../../../electromagnetism.md#gauss-s-law) gives the radial field

$$
E_r=\begin{cases}0,&r<R,\\C/r^2,&R<r<2R,\\-C/r^2,&2R<r<3R,\\0,&r>3R.\end{cases}
$$

Taking zero potential outside,

$$
\phi=\begin{cases}C/(3R),&r<R,\\C(1/r-2/(3R)),&R<r<2R,\\C(1/(3R)-1/r),&2R<r<3R,\\0,&r>3R.\end{cases}
$$

The charge formula gives

$$
U=\frac12\sum_iQ_i\phi(r_i)=\frac{q^2}{12\pi\varepsilon_0R}.
$$

The field formula gives the same result after integrating $4\pi r^2E_r^2$ over the two nonzero annuli.

## 16D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="16d/solution">Solution</h3>

↑ **Parent:** [16D](#16d)

For steady inviscid flow, Bernoulli's equation along a [streamline](../../../fluid-mechanics.md#streamline) is

$$
p+\frac12\rho|u|^2+\chi=\text{constant}.
$$

Writing steady Euler flow in divergence form and integrating over $V$ gives

$$
\int_{\partial V}(\rho(u\cdot n)u+pn+\chi n)\,dS=0
$$

by incompressibility and the divergence theorem.

<h3 id="16d/i">i</h3>

↑ **Parent:** [16D](#16d)

<h4 id="16d/i/solution">Solution</h4>

↑ **Parent:** [I](#16d/i)

The speeds are $U=q/A$ upstream and $v=q/(2a)$ in either daughter vessel. Bernoulli therefore gives

$$
\boxed{p_{\rm up}-p_{\rm down}=\frac\rho2(v^2-U^2)
=\frac{\rho q^2}{2}\left(\frac1{4a^2}-\frac1{A^2}\right).}
$$

<h3 id="16d/ii">ii</h3>

↑ **Parent:** [16D](#16d)

<h4 id="16d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#16d/ii)

Take the downstream tissue [pressure](../../../thermodynamics.md#pressure) as gauge zero. The two transverse [momentum](../../../classical-mechanics.md#momentum) fluxes cancel. The force of the fluid on the junction is axial and equals

$$
F=\left[A(p_{\rm up}-p_{\rm down})+\rho q(U-v\cos\alpha)\right]e_x,
$$

where $U=q/A$, $v=q/(2a)$ and the [pressure](../../../thermodynamics.md#pressure) difference is that in part (i).

## 17A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="17a/a">a</h3>

↑ **Parent:** [17A](#17a)

<h4 id="17a/a/solution">Solution</h4>

↑ **Parent:** [A](#17a/a)

For a unit [vector](../../../vector-space.md#vector) $v$, a [Householder reflection](../../../linear-algebra.md#householder-transformation) is $H=I-2vv^T$. Clearly $H^T=H$, and $H^TH=(I-2vv^T)^2=I$.

<h3 id="17a/b">b</h3>

↑ **Parent:** [17A](#17a)

<h4 id="17a/b/solution">Solution</h4>

↑ **Parent:** [B](#17a/b)

The [vector](../../../vector-space.md#vector) $v$ has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $-1$, while every [vector](../../../vector-space.md#vector) in $v^\perp$ has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $1$. Their multiplicities are one and $n-1$, respectively.

<h3 id="17a/c">c</h3>

↑ **Parent:** [17A](#17a)

<h4 id="17a/c/solution">Solution</h4>

↑ **Parent:** [C](#17a/c)

At step $k$, choose a Householder reflection acting only on coordinates $k,\ldots,n$ that maps the trailing part of column $k$ to a multiple of the first coordinate in that block. It zeros every entry below the diagonal without changing earlier columns. Induction produces $H_n\cdots H_1A=R$ upper triangular.

<h3 id="17a/d">d</h3>

↑ **Parent:** [17A](#17a)

<h4 id="17a/d/solution">Solution</h4>

↑ **Parent:** [D](#17a/d)

For symmetric $A$, apply at stage $k$ the same reflection on both sides, choosing it to zero entries below the first subdiagonal in column $k$. [Orthogonal similarity](../../../linear-algebra.md#orthogonal-similarity) preserves symmetry, so the corresponding row entries vanish too and previous zeros remain. After finitely many stages $Q A Q^T$ is symmetric tridiagonal. Constructing each reflector uses only arithmetic and one square root.

## 18H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="18h/a">a</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/a/solution">Solution</h4>

↑ **Parent:** [A](#18h/a)

Let $S_{xx}=\sum X_i^2$. The likelihood equations give

$$
\hat\beta=\frac{\sum X_iY_i}{S_{xx}},\qquad
\hat\sigma^2=\frac1n\sum(Y_i-X_i\hat\beta)^2.
$$

These are orthogonal projections of a Gaussian [vector](../../../vector-space.md#vector) onto the span of $X$ and its orthogonal complement, hence are independent.

<h3 id="18h/b">b</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/b/solution">Solution</h4>

↑ **Parent:** [B](#18h/b)

With $s^2=\sum(Y_i-X_i\hat\beta)^2/(n-1)$,

$$
\frac{\hat\beta-\beta}{s/\sqrt{S_{xx}}}\sim t_{n-1}.
$$

Thus the interval is

$$
\boxed{\hat\beta\ \pm\ t_{n-1,1-\alpha/2}\frac{s}{\sqrt{S_{xx}}}.}
$$

<h3 id="18h/c">c</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/c/solution">Solution</h4>

↑ **Parent:** [C](#18h/c)

Unbiasedness requires $\sum c_iX_i=1$. Cauchy–Schwarz gives $1\le(\sum c_i^2)S_{xx}$, so

$$
\operatorname{Var}(\tilde\beta)=\sigma^2\sum c_i^2\ge\frac{\sigma^2}{S_{xx}}.
$$

Equality holds exactly for $c_i=X_i/S_{xx}$.

<h3 id="18h/d">d</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/d/solution">Solution</h4>

↑ **Parent:** [D](#18h/d)

The reverse-regression estimate is $\hat b=\sum X_iY_i/\sum Y_i^2$. Therefore

$$
\hat b\hat\beta=\frac{(\sum X_iY_i)^2}{(\sum X_i^2)(\sum Y_i^2)}\le1
$$

by Cauchy–Schwarz. Equality means the two data [vectors](../../../vector-space.md#vector) are proportional, which is exactly when both fitted residual sums, and hence both variance MLEs, vanish.

## 19H

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="19h/a">a</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/a/solution">Solution</h4>

↑ **Parent:** [A](#19h/a)

A chain is reversible with respect to $\pi$ when $\pi_iP_{ij}=\pi_jP_{ji}$ for all states. For random walk on a finite connected undirected graph, $\pi_i=\deg(i)/(2|E|)$ satisfies this because both sides equal $1/(2|E|)$ on an edge and zero otherwise.

<h3 id="19h/b">b</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/b/solution">Solution</h4>

↑ **Parent:** [B](#19h/b)

The graph has six edges, and $A$ has degree one. Hence $\pi_A=1/12$. Kac's return-time formula gives

$$
\boxed{\mathbb E_A T_A^+=\frac1{\pi_A}=12.}
$$

<h3 id="19h/c">c</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/c/solution">Solution</h4>

↑ **Parent:** [C](#19h/c)

After the forced first step $A\to B$, let $h_i=P_i(T_A<T_F)$. Symmetry gives $h_C=h_D=x$, while

$$
h_B=(1+2x)/3,\quad x=(h_B+h_E)/2,\quad h_E=2x/3.
$$

Solving gives $h_B=2/3$. Thus the requested probability is $2/3$.

<h3 id="19h/d">d</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/d/solution">Solution</h4>

↑ **Parent:** [D](#19h/d)

Let $g_i=E_i[T_A\mathbf1_{\{T_A<T_F\}}]$ for the chain absorbed at $A$ or $F$. With $g_C=g_D=y$, [First-step analysis](../../../analysis.md#first-step-analysis) gives

$$
g_B=(2+2y)/3,\qquad g_E=(1+2y)/3,\qquad y=(1+g_B+g_E)/2.
$$

Thus $y=3$ and $g_B=8/3$. Including the initial step from $A$, the conditional mean is

$$
\boxed{1+\frac{g_B}{h_B}=1+\frac{8/3}{2/3}=5.}
$$

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
