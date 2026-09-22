# Paper 3

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2025/paperia_3_2025.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2025/paperia_3_2025.pdf)

**Table of contents**

- [1D](#1d)
  - [Solution](#1d/solution)
- [2D](#2d)
  - [i](#2d/i)
    - [Solution](#2d/i/solution)
  - [ii](#2d/ii)
    - [Solution](#2d/ii/solution)
  - [iii](#2d/iii)
    - [Solution](#2d/iii/solution)
- [3A](#3a)
  - [Solution](#3a/solution)
  - [i](#3a/i)
    - [Solution](#3a/i/solution)
  - [ii](#3a/ii)
    - [Solution](#3a/ii/solution)
- [4A](#4a)
  - [Solution](#4a/solution)
  - [i](#4a/i)
    - [Solution](#4a/i/solution)
  - [ii](#4a/ii)
    - [Solution](#4a/ii/solution)
  - [iii](#4a/iii)
    - [Solution](#4a/iii/solution)
- [5D](#5d)
  - [a](#5d/a)
    - [i](#5d/a/i)
      - [Solution](#5d/a/i/solution)
    - [ii](#5d/a/ii)
      - [Solution](#5d/a/ii/solution)
  - [b](#5d/b)
    - [Solution](#5d/b/solution)
  - [c](#5d/c)
    - [Solution](#5d/c/solution)
- [6D](#6d)
  - [a](#6d/a)
    - [Solution](#6d/a/solution)
  - [b](#6d/b)
    - [Solution](#6d/b/solution)
  - [c](#6d/c)
    - [Solution](#6d/c/solution)
  - [d](#6d/d)
    - [i](#6d/d/i)
      - [Solution](#6d/d/i/solution)
    - [ii](#6d/d/ii)
      - [Solution](#6d/d/ii/solution)
- [7D](#7d)
  - [Solution](#7d/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
- [9A](#9a)
  - [a](#9a/a)
    - [Solution](#9a/a/solution)
  - [b](#9a/b)
    - [Solution](#9a/b/solution)
  - [c](#9a/c)
    - [Solution](#9a/c/solution)
- [10A](#10a)
  - [a](#10a/a)
    - [Solution](#10a/a/solution)
  - [b](#10a/b)
    - [i](#10a/b/i)
      - [Solution](#10a/b/i/solution)
    - [ii](#10a/b/ii)
      - [Solution](#10a/b/ii/solution)
    - [iii](#10a/b/iii)
      - [Solution](#10a/b/iii/solution)
  - [c](#10a/c)
    - [i](#10a/c/i)
      - [Solution](#10a/c/i/solution)
    - [ii](#10a/c/ii)
      - [Solution](#10a/c/ii/solution)
- [11A](#11a)
  - [Solution](#11a/solution)
  - [i](#11a/i)
    - [Solution](#11a/i/solution)
  - [ii](#11a/ii)
    - [Solution](#11a/ii/solution)
  - [iii](#11a/iii)
    - [Solution](#11a/iii/solution)
- [12A](#12a)
  - [Solution](#12a/solution)

## 1D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1d/solution">Solution</h3>

↑ **Parent:** [1D](#1d)

The centre is

$$
Z(G)=\{z\in G:zg=gz\text{ for every }g\in G\}.
$$

Every [subgroup](../../../group.md#subgroup) $H\le Z(G)$ is normal, since $ghg^{-1}=h$ for all $g\in G$ and $h\in H$.

Write $D_{2n}=\langle r,s:r^n=s^2=1, srs=r^{-1}\rangle$. A central rotation must satisfy $r^k=r^{-k}$, and no reflection is central for $n\ge3$. Hence

$$
Z(D_{2n})=\begin{cases}\{1\},&n\text{ odd},\\\{1,r^{n/2}\},&n\text{ even}.\end{cases}
$$

## 2D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2d/i">i</h3>

↑ **Parent:** [2D](#2d)

<h4 id="2d/i/solution">Solution</h4>

↑ **Parent:** [I](#2d/i)

**False.** A finite cyclic [group](../../../group.md) has nonidentity torsion, whereas $\mathbb Z$ is torsion-free, so an injective homomorphism cannot exist.

<h3 id="2d/ii">ii</h3>

↑ **Parent:** [2D](#2d)

<h4 id="2d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2d/ii)

**False.** A surjection $C_n\to C_m$ exists exactly when $m$ divides $n$; for example there is none from $C_3$ to $C_2$.

<h3 id="2d/iii">iii</h3>

↑ **Parent:** [2D](#2d)

<h4 id="2d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2d/iii)

**False.** The proper [subgroup](../../../group.md#subgroup) $2\mathbb Z\times2\mathbb Z$ of $\mathbb Z^2$ is isomorphic to $\mathbb Z^2$ and is not cyclic.

## 3A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3a/solution">Solution</h3>

↑ **Parent:** [3A](#3a)

The parametrisation $r(x,y)=(x,y,F(x,y))$ has area factor

$$
|r_x\times r_y|=\sqrt{1+F_x^2+F_y^2},
$$

so $\operatorname{area}(S)=\iint_D\sqrt{1+F_x^2+F_y^2}\,dx\,dy$.

For the unbounded saddle $F=(x^2-y^2)/2$, this factor is $\sqrt{1+x^2+y^2}$. Thus the requested [integral](../../../calculus.md#integral) is

$$
2\pi\int_0^\infty\frac{r\,dr}{(1+r^2)^{3/2}}=2\pi,
$$

which converges because its radial tail is $O(r^{-2})$.

<h3 id="3a/i">i</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/i/solution">Solution</h4>

↑ **Parent:** [I](#3a/i)

Here the area factor is $\sqrt{1+2^2+3^2}=\sqrt{14}$ and the triangular base has area $3$. The surface area is therefore $3\sqrt{14}$.

<h3 id="3a/ii">ii</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3a/ii)

Write the upper cap as $z=\sqrt{1-x^2-y^2}$. Its area factor is $(1-r^2)^{-1/2}$, and the projected disc has radius $\sqrt a$. Therefore

$$
\boxed{\operatorname{area}(S)=2\pi\int_0^{\sqrt a}\frac r{\sqrt{1-r^2}}\,dr=2\pi(1-\sqrt{1-a}).}
$$

## 4A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4a/solution">Solution</h3>

↑ **Parent:** [4A](#4a)

Green's theorem states, for a positively oriented simple boundary $C=\partial R$,

$$
\oint_C(P\,dx+Q\,dy)=\iint_R(Q_x-P_y)\,dA.
$$

The defining [polynomial](../../../polynomial.md) becomes

$$
r^2(r^2-2r\cos\theta-\sin^2\theta),
$$

so the region is the [cardioid](../../../calculus.md#cardioid)

$$
\boxed{0\le r\le1+\cos\theta,\qquad-\pi\le\theta\le\pi.}
$$

<h3 id="4a/i">i</h3>

↑ **Parent:** [4A](#4a)

<h4 id="4a/i/solution">Solution</h4>

↑ **Parent:** [I](#4a/i)

The field is $e_\theta$, so on the polar boundary $F\cdot dr=r\,d\theta$. Hence

$$
\boxed{\oint_CF\cdot dr=\int_{-\pi}^{\pi}(1+\cos\theta)\,d\theta=2\pi.}
$$

<h3 id="4a/ii">ii</h3>

↑ **Parent:** [4A](#4a)

<h4 id="4a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4a/ii)

Here $Q_x-P_y=y-2y=-y$. Green's theorem gives the [integral](../../../calculus.md#integral) of $-y$ over a region symmetric about the $x$ axis, hence the answer is $0$.

<h3 id="4a/iii">iii</h3>

↑ **Parent:** [4A](#4a)

<h4 id="4a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4a/iii)

On the boundary the [integral](../../../calculus.md#integral) is $\int_{-\pi}^{\pi}\theta\,dy$. [Integration by parts](../../../calculus.md#integration-by-parts) has zero endpoint term and leaves

$$
\boxed{-\int_{-\pi}^{\pi}y\,d\theta=-\int_{-\pi}^{\pi}(1+\cos\theta)\sin\theta\,d\theta=0.}
$$

## 5D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5d/a">a</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/a/i">i</h4>

↑ **Parent:** [A](#5d/a)

<h5 id="5d/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5d/a/i)

The orbit and stabiliser are

$$
Gx=\{gx:g\in G\},\qquad \operatorname{Stab}_G(x)=\{g\in G:gx=x\}.
$$

Such an action can be faithful: the natural action of $S_3$ on three points is faithful, although every point stabiliser has order two.

<h4 id="5d/a/ii">ii</h4>

↑ **Parent:** [A](#5d/a)

<h5 id="5d/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5d/a/ii)

If $y=gx$, then

$$
\operatorname{Stab}_G(y)=g\operatorname{Stab}_G(x)g^{-1}.
$$

Indeed, $h$ fixes $x$ exactly when $ghg^{-1}$ fixes $gx$. Conjugation by $g$ is therefore the required isomorphism.

<h3 id="5d/b">b</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/b/solution">Solution</h4>

↑ **Parent:** [B](#5d/b)

For $1\le k<n$, any nonidentity permutation moves some $k$-subset: choose a moved point and complete a subset so that it contains that point but not its image. Thus the kernel is trivial. For $k=n$ the action is trivial, so it is faithful only in the degenerate case $n=1$.

<h3 id="5d/c">c</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/c/solution">Solution</h4>

↑ **Parent:** [C](#5d/c)

If $N\triangleleft S_n$, then $N\cap A_n\triangleleft A_n$, hence the intersection is either $1$ or $A_n$. In the latter case $N$ is $A_n$ or $S_n$. In the former, $N$ injects into $S_n/A_n\cong C_2$, so $|N|\le2$. A [normal subgroup](../../../group-theory.md#normal-subgroup) of order two would be central, but $Z(S_n)=1$ for $n\ge3$. Therefore the normal [subgroups](../../../group.md#subgroup) are

$$
\boxed{1,\quad A_n,\quad S_n.}
$$

## 6D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6d/a">a</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/a/solution">Solution</h4>

↑ **Parent:** [A](#6d/a)

With $D_8=\langle r,s:r^4=s^2=1, srs=r^{-1}\rangle$, its normal [subgroups](../../../group.md#subgroup) are

$$
1,\qquad\langle r^2\rangle,\qquad\langle r\rangle,\qquad
\langle r^2,s\rangle,\qquad\langle r^2,rs\rangle,\qquad D_8.
$$

The last three proper nontrivial examples have index two; the four individual reflection [subgroups](../../../group.md#subgroup) are not normal.

<h3 id="6d/b">b</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/b/solution">Solution</h4>

↑ **Parent:** [B](#6d/b)

If $K\triangleleft G$, the quotient map $G\to G/K$ is surjective with kernel $K$. Conversely, every kernel is normal because $\phi(gkg^{-1})=\phi(g)1\phi(g)^{-1}=1$.

<h3 id="6d/c">c</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/c/solution">Solution</h4>

↑ **Parent:** [C](#6d/c)

**False.** The [quaternion group](../../../finite-group-theory.md#quaternion-group) $Q_8$ is nonabelian, but each of its [subgroups](../../../group.md#subgroup) is normal: its nontrivial proper [subgroups](../../../group.md#subgroup) are its centre $\{\pm1\}$ and the three cyclic [subgroups](../../../group.md#subgroup) of order four, all of index two.

<h3 id="6d/d">d</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/d/i">i</h4>

↑ **Parent:** [D](#6d/d)

<h5 id="6d/d/i/solution">Solution</h5>

↑ **Parent:** [I](#6d/d/i)

For $g\in G$ and $x\in\phi^{-1}(N)$,

$$
\phi(gxg^{-1})=\phi(g)\phi(x)\phi(g)^{-1}\in N,
$$

so the preimage is normal.

<h4 id="6d/d/ii">ii</h4>

↑ **Parent:** [D](#6d/d)

<h5 id="6d/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6d/d/ii)

Given $h\in H$, choose $g\in G$ with $\phi(g)=h$. For $k\in K$,

$$
h\phi(k)h^{-1}=\phi(gkg^{-1})\in\phi(K),
$$

because $K$ is normal. Thus $\phi(K)\triangleleft H$.

## 7D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7d/solution">Solution</h3>

↑ **Parent:** [7D](#7d)

For $f(z)=(az+b)/(cz+d)$, finite fixed points obey

$$
cz^2+(d-a)z-b=0,
$$

with the point at infinity included in the usual way when appropriate. The fundamental theorem of algebra on the Riemann sphere gives at least one fixed point. Unless $f$ is the identity, the equation is nonzero of degree at most two, so there are one or two distinct fixed points.

Let $\zeta$ be a primitive $m$th root of unity. For every $u\in\mathbb C$,

$$
f_u(z)=u+\zeta(z-u)
$$

has order $m$, and these transformations are distinct as $u$ varies.

Projectivising [matrices](../../../vector-space.md#matrix) is a homomorphism. Thus $B=CAC^{-1}$ in $SL_2(\mathbb C)$ implies $g=[C]f[C]^{-1}$ in the Möbius [group](../../../group.md).

The converse as stated is false because [matrix](../../../vector-space.md#matrix) representatives may be rescaled: $A=I$ and $B=2I$ define the same Möbius transformation, while neither $B$ nor $-B$ is conjugate to $A$ (their traces differ).

## 8D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

Invertible [matrices](../../../vector-space.md#matrix) are closed under multiplication, contain $I$, have associative multiplication, and have inverses by the adjugate formula over the field $\mathbb F_p$. The first column can be any nonzero [vector](../../../vector-space.md#vector) and the second any [vector](../../../vector-space.md#vector) outside its span, so

$$
|GL_2(\mathbb F_p)|=(p^2-1)(p^2-p).
$$

For $p=2$, the [matrix](../../../vector-space.md#matrix) $\begin{pmatrix}0&1\\1&1\end{pmatrix}$ has order three. There is no element of order six: $GL_2(\mathbb F_2)\cong S_3$, whose element orders are $1,2,3$.

For $p>2$, $SL_2(\mathbb F_p)=\ker\det$ is a proper normal [subgroup](../../../group.md#subgroup). For $p=2$, the order-three [subgroup](../../../group.md#subgroup) in the copy of $S_3$ is proper and normal.

In $GL_2(\mathbb F_{11})$, take

$$
H=\left\{\begin{pmatrix}a&b\\0&1\end{pmatrix}:a\in A, b\in\mathbb F_{11}\right\},
$$

where $A\le\mathbb F_{11}^{\times}$ is the [subgroup](../../../group.md#subgroup) of order five. This [semidirect product](../../../group-theory.md#semidirect-product) has order $55$ and is nonabelian because a nontrivial diagonal element does not commute with translations.

## 9A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9a/a">a</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/a/solution">Solution</h4>

↑ **Parent:** [A](#9a/a)

The [divergence theorem](../../../calculus.md#divergence-theorem) is $\iint_{\partial V}F\cdot n\,dS=\iiint_V\nabla\cdot F\,dV$. Here $\nabla\cdot F=3z+2yz$. The $y$ term integrates to zero by symmetry, while the ellipse has area $\pi/\sqrt{ab}$. Hence the flux is

$$
\boxed{\frac\pi{\sqrt{ab}}\int_0^3 3z\,dz=\frac{27\pi}{2\sqrt{ab}}.}
$$

<h3 id="9a/b">b</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/b/solution">Solution</h4>

↑ **Parent:** [B](#9a/b)

The top and bottom fluxes cancel because $F_z=x^2+y^2$ is independent of $z$. Parametrise the side by $(\cos\theta/\sqrt a,\sin\theta/\sqrt b,z)$; its outward [vector](../../../vector-space.md#vector) area is

$$
\left(\frac{\cos\theta}{\sqrt b},\frac{\sin\theta}{\sqrt a},0\right)d\theta\,dz.
$$

The term involving $y^2z$ integrates to zero, and the remaining [integral](../../../calculus.md#integral) is

$$
\int_0^3\int_0^{2\pi}\frac{3z\cos^2\theta}{\sqrt{ab}}\,d\theta\,dz
=\frac{27\pi}{2\sqrt{ab}},
$$

confirming part (a).

<h3 id="9a/c">c</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/c/solution">Solution</h4>

↑ **Parent:** [C](#9a/c)

The curl is $(2y-y^2,x,0)$, so the field is not conservative. On $C$, $z=1$ and $dz=0$, giving

$$
\boxed{\oint_C(3x\,dx+y^2\,dy)=\oint_Cd\left(\frac32x^2+\frac13y^3\right)=0.}
$$

## 10A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10a/a">a</h3>

↑ **Parent:** [10A](#10a)

<h4 id="10a/a/solution">Solution</h4>

↑ **Parent:** [A](#10a/a)

Write $p=\sum_{j=0}^na_jx^{n-j}y^j$. Equating the coefficient of $x^{n-j-2}y^j$ in $\nabla^2p$ gives

$$
(n-j)(n-j-1)a_j+(j+2)(j+1)a_{j+2}=0.
$$

**Thus all even coefficients are determined by $a_0$ and all odd coefficients by $a_1$, with no further constraints. These two choices give two independent harmonic homogeneous [polynomials](../../../polynomial.md).**

<h3 id="10a/b">b</h3>

↑ **Parent:** [10A](#10a)

<h4 id="10a/b/i">i</h4>

↑ **Parent:** [B](#10a/b)

<h5 id="10a/b/i/solution">Solution</h5>

↑ **Parent:** [I](#10a/b/i)

For radial [functions](../../../function.md), $\nabla^2h=h''+2h'/r$. Since $\nabla^2e^{-r}=e^{-r}-2e^{-r}/r$ and $\nabla^2r^{-4}=12r^{-6}$, decay and the boundary value give

$$
\boxed{u=e^{-r}+r^{-4}-\frac{e^{-1}}r.}
$$

<h4 id="10a/b/ii">ii</h4>

↑ **Parent:** [B](#10a/b)

<h5 id="10a/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10a/b/ii)

The angular Laplacian sends $\sin\theta$ to $\cos(2\theta)/\sin\theta$, while $1/r$ is radially harmonic. Therefore

$$
\boxed{u=\frac{\sin\theta}{r}.}
$$

<h4 id="10a/b/iii">iii</h4>

↑ **Parent:** [B](#10a/b)

<h5 id="10a/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#10a/b/iii)

The $\phi$ part contributes $-\sin\phi/(r^2\sin^2\theta)$, and again $1/r$ is radially harmonic. Hence

$$
\boxed{u=\frac{\sin\phi}{r}.}
$$

<h3 id="10a/c">c</h3>

↑ **Parent:** [10A](#10a)

<h4 id="10a/c/i">i</h4>

↑ **Parent:** [C](#10a/c)

<h5 id="10a/c/i/solution">Solution</h5>

↑ **Parent:** [I](#10a/c/i)

Set $A=x(1-x)$, $B=y(1-y)$ and $C=z(1-z)$. The forcing is $AB+AC+BC$, while $\nabla^2(ABC)=-2(AB+AC+BC)$. Thus

$$
u=-\frac12x(1-x)y(1-y)z(1-z),
$$

which vanishes on every face.

<h4 id="10a/c/ii">ii</h4>

↑ **Parent:** [C](#10a/c)

<h5 id="10a/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10a/c/ii)

Each sine product is a Dirichlet eigenfunction. The squared wave-number sums are $24\pi^2$ and $30\pi^2$, respectively, so

$$
\boxed{u=-\frac{\sin(2\pi x)\sin(2\pi y)\sin(4\pi z)}{24\pi^2}
+\frac{\sin(2\pi x)\sin(\pi y)\sin(5\pi z)}{30\pi^2}.}
$$

## 11A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11a/solution">Solution</h3>

↑ **Parent:** [11A](#11a)

For coordinates $x=x(q)$, the Jacobian is $J_{ij}=\partial x_i/\partial q_j$. Expanding after separating $x_1=r\cos\theta_1$ from the remaining coordinates gives

$$
|J_n|=r\sin^{n-2}\theta_1\,|J_{n-1}|.
$$

Consequently

$$
dV=r^{n-1}\prod_{j=1}^{n-2}\sin^{n-1-j}\theta_j\,dr\,d\theta_1\cdots d\theta_{n-2}\,d\phi,
$$

and on $r=R$ the surface element is obtained by omitting $dr$ and replacing $r$ by $R$.

<h3 id="11a/i">i</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/i/solution">Solution</h4>

↑ **Parent:** [I](#11a/i)

The ball volume is

$$
V_n(R)=\frac{\pi^{n/2}R^n}{\Gamma(n/2+1)}.
$$

For $n=2m$ this is $\pi^mR^{2m}/m!$; for $n=2m+1$ it is $2^{2m+1}m!\pi^mR^{2m+1}/(2m+1)!$.

<h3 id="11a/ii">ii</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11a/ii)

Differentiating the ball volume with respect to $R$ gives

$$
\boxed{A_{n-1}(R)=\frac{2\pi^{n/2}R^{n-1}}{\Gamma(n/2)}=\frac nR V_n(R).}
$$

<h3 id="11a/iii">iii</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#11a/iii)

Reflection symmetry makes the [integral](../../../calculus.md#integral) zero for $i\ne j$. Rotational symmetry makes all diagonal [integrals](../../../calculus.md#integral) equal, and their sum is $R^2A_{n-1}(R)$. Therefore

$$
\boxed{\int_{r=R}x_ix_j\,dS=\delta_{ij}\frac{R^2A_{n-1}(R)}n
=\delta_{ij}\frac{\pi^{n/2}R^{n+1}}{\Gamma(n/2+1)}.}
$$

## 12A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12a/solution">Solution</h3>

↑ **Parent:** [12A](#12a)

The product rule gives

$$
\partial_j(T_{ij}v_i)=(\partial_jT_{ij})v_i+T_{ij}\partial_jv_i.
$$

Integrating and applying the divergence theorem proves the identity.

Here $\operatorname{div}T=4(x,y,z)$ and $v=x(x,y,z)$, so

$$
\int_V\operatorname{div}T\cdot v\,dV
=4\int_Vx(x^2+y^2+z^2)\,dV=\frac73.
$$

On the boundary, $(Tn)\cdot v=x(x\cdot n)(x^2+y^2+z^2-1)$. The nonzero contributions from the faces $x=1,y=1,z=1$ are respectively $2/3,5/12,5/12$, totaling $3/2$.

Finally, direct contraction gives

$$
T_{ij}\partial_jv_i=2x(x^2+y^2+z^2)-4x,
$$

whose [integral](../../../calculus.md#integral) is $-5/6$. Thus the right side is $3/2-(-5/6)=7/3$, equal to the left side.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
