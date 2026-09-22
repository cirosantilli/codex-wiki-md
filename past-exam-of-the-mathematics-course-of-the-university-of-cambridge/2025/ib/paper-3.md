# Paper 3

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2025/paperib_3_2025.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2025/paperib_3_2025.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2E](#2e)
  - [Solution](#2e/solution)
- [3A](#3a)
  - [a](#3a/a)
    - [Solution](#3a/a/solution)
  - [b](#3a/b)
    - [Solution](#3a/b/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5D](#5d)
  - [Solution](#5d/solution)
- [6C](#6c)
  - [Solution](#6c/solution)
- [7D](#7d)
  - [Solution](#7d/solution)
- [8H](#8h)
  - [a](#8h/a)
    - [Solution](#8h/a/solution)
  - [b](#8h/b)
    - [Solution](#8h/b/solution)
- [9F](#9f)
  - [a](#9f/a)
    - [Solution](#9f/a/solution)
  - [b](#9f/b)
    - [Solution](#9f/b/solution)
  - [c](#9f/c)
    - [Solution](#9f/c/solution)
- [10E](#10e)
  - [a](#10e/a)
    - [Solution](#10e/a/solution)
    - [i](#10e/a/i)
      - [Solution](#10e/a/i/solution)
    - [ii](#10e/a/ii)
      - [Solution](#10e/a/ii/solution)
  - [b](#10e/b)
    - [Solution](#10e/b/solution)
- [11G](#11g)
  - [Solution](#11g/solution)
- [12F](#12f)
  - [Solution](#12f/solution)
- [13E](#13e)
  - [Solution](#13e/solution)
- [14D](#14d)
  - [Solution](#14d/solution)
- [15B](#15b)
  - [Solution](#15b/solution)
- [16D](#16d)
  - [Solution](#16d/solution)
- [17B](#17b)
  - [a](#17b/a)
    - [Solution](#17b/a/solution)
  - [b](#17b/b)
    - [Solution](#17b/b/solution)
  - [c](#17b/c)
    - [Solution](#17b/c/solution)
- [18H](#18h)
  - [a](#18h/a)
    - [Solution](#18h/a/solution)
  - [b](#18h/b)
    - [Solution](#18h/b/solution)
  - [c](#18h/c)
    - [Solution](#18h/c/solution)
- [19H](#19h)
  - [a](#19h/a)
    - [Solution](#19h/a/solution)
  - [b](#19h/b)
    - [Solution](#19h/b/solution)
  - [c](#19h/c)
    - [Solution](#19h/c/solution)
  - [d](#19h/d)
    - [Solution](#19h/d/solution)

## 1E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

If a finite [group](../../../group.md) is not simple, choose a maximal proper normal [subgroup](../../../group.md#subgroup) and repeat inside it. Orders strictly decrease, so the process terminates; maximality makes every quotient simple.

For $S_4$ one [composition series](../../../finite-group-theory.md#composition-series) is

$$
S_4\triangleright A_4\triangleright V_4
\triangleright\langle(12)(34)\rangle\triangleright1.
$$

The successive quotients have orders $2,3,2,2$, hence are simple. As [subgroups](../../../group.md#subgroup) of $S_4$, the [groups](../../../group.md) $S_4,A_4,V_4$, and $1$ are normal. The selected order-two [subgroup](../../../group.md#subgroup) is not normal, since conjugation permutes the three double transpositions.

## 2E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2e/solution">Solution</h3>

↑ **Parent:** [2E](#2e)

For the Möbius action on the upper half-plane, a noncentral element is elliptic if it has one fixed point in the interior and none on the boundary, parabolic if it has one boundary fixed point, and hyperbolic if it has two boundary fixed points. Examples are

$$
\begin{pmatrix}\cos\theta&\sin\theta\\-\sin\theta&\cos\theta\end{pmatrix},\quad
\begin{pmatrix}1&1\\0&1\end{pmatrix},\quad
\begin{pmatrix}a&0\\0&a^{-1}\end{pmatrix}\ (a>1).
$$

Fixed points satisfy a real quadratic. Its discriminant is $(\operatorname{tr}g)^2-4$, so the three mutually exclusive cases $|\operatorname{tr}g|<2$, $=2$, and $>2$ give precisely the three types.

If $g^n=I$ and $g\ne\pm I$, its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are nonreal reciprocal roots of unity. Thus $|\operatorname{tr}g|<2$ and $g$ is elliptic; no such element is parabolic or hyperbolic.

## 3A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3a/a">a</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/a/solution">Solution</h4>

↑ **Parent:** [A](#3a/a)

Uniqueness of Laurent coefficients applied to $f(z)=f(-z)$ gives

$$
\sum_na_nz^n=\sum_n(-1)^na_nz^n.
$$

**Hence $a_n=(-1)^na_n$, so every coefficient with odd $n$ vanishes.**

<h3 id="3a/b">b</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/b/solution">Solution</h4>

↑ **Parent:** [B](#3a/b)

The poles inside $C_n$ are zero and $\pm k\pi$ for $1\le k\le n$. At a nonzero pole,

$$
\operatorname{Res}_{k\pi}\frac1{z^3\sin z}=\frac{(-1)^k}{k^3\pi^3},
$$

and the residue at $-k\pi$ is its negative. At zero, the [Laurent series](../../../analysis.md#laurent-series) contains only even powers because the [function](../../../function.md) is even, so its residue is zero. All residues cancel and therefore

$$
\boxed{I_n=0\qquad(n=0,1,2,\ldots).}
$$

## 4C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

The Euler–Lagrange equations are

$$
\ddot x+\omega\cos(\omega t)=0,\qquad \ddot y+y=0.
$$

For $\omega\ne0$ their general solution is

$$
x=c_1t+c_2+\frac{\cos(\omega t)}\omega,\qquad
y=c_3\cos t+c_4\sin t,
$$

while for $\omega=0$, $x=c_1t+c_2$.

The action has continuous translation symmetry in $x$; it is also invariant up to endpoint terms under adding homogeneous Jacobi solutions $at+b$ to $x$ and $a\cos t+b\sin t$ to $y$. For $\omega=0$ it additionally has continuous time-translation symmetry; for nonzero $\omega$ only the corresponding discrete period remains.

A complete set of four independent first [integrals](../../../calculus.md#integral) is

$$
C_1=\dot x+\sin(\omega t),
$$



$$
C_2=x-tC_1-\frac{\cos(\omega t)}\omega\quad(\omega\ne0),
\qquad C_2=x-t\dot x\quad(\omega=0),
$$



$$
C_3=y\cos t-\dot y\sin t,\qquad C_4=y\sin t+\dot y\cos t.
$$

In particular $(\dot y^2+y^2)/2=(C_3^2+C_4^2)/2$ is conserved; when $\omega=0$, the usual total energy is conserved as well.

## 5D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5d/solution">Solution</h3>

↑ **Parent:** [5D](#5d)

Insert the transform definitions and use Fubini:

$$
\frac1{2\pi}\int\tilde f(k)\tilde g(k)e^{ikx}dk
=\int f(u)\left[\frac1{2\pi}\int\tilde g(k)e^{ik(x-u)}dk\right]du
=\int f(u)g(x-u)du.
$$

For the indicator of $(-1,1)$,

$$
\tilde f(k)=\int_{-1}^1e^{-ikx}dx=\frac{2\sin k}{k}.
$$

Putting $g=f$ and $x=0$ in the [convolution theorem](../../../fourier-analysis.md#convolution-theorem) gives

$$
2=\frac1{2\pi}\int_{-\infty}^{\infty}\frac{4\sin^2k}{k^2}dk,
$$

and hence

$$
\boxed{\int_{-\infty}^{\infty}\frac{\sin^2k}{k^2}dk=\pi.}
$$

## 6C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6c/solution">Solution</h3>

↑ **Parent:** [6C](#6c)

Position and [momentum](../../../classical-mechanics.md#momentum) are

$$
Q\psi=x\psi,\qquad P\psi=-i\hbar\,\partial_x\psi.
$$

Differentiating the expectation, substituting Schrödinger's equation, and integrating by parts gives Ehrenfest's relation

$$
\frac d{dt}\langle P\rangle=\frac{i}{\hbar}\langle[H,P]\rangle
=-k\langle Q\rangle.
$$

**Thus the mean [momentum](../../../classical-mechanics.md#momentum) changes according to the classical mean force $-kx$.**

## 7D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7d/solution">Solution</h3>

↑ **Parent:** [7D](#7d)

Take $x$ vertically downward and $y$ outward from the wall, with the film occupying $0<y<h$. The ambient [pressure](../../../thermodynamics.md#pressure) is

$$
p_a(x)=p_0+\rho_agx.
$$

At $y=h$, normal stress continuity gives $p=p_a$ and zero ambient shear gives $\mu U'(h)=0$; at the wall, no slip gives $U(0)=0$.

For steady parallel flow $u=(U(y),0)$, incompressibility is automatic and Navier–Stokes reduces to

$$
p_y=0,\qquad0=-p_x+\mu U''+\rho g.
$$

Since $p_x=\rho_ag$, integration yields

$$
\boxed{p=p_0+\rho_agx,\qquad
U(y)=\frac{(\rho-\rho_a)g}{\mu}\left(hy-\frac{y^2}{2}\right).}
$$

## 8H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8h/a">a</h3>

↑ **Parent:** [8H](#8h)

<h4 id="8h/a/solution">Solution</h4>

↑ **Parent:** [A](#8h/a)

A state is recurrent when, starting there, the chain returns to it with probability one. An irreducible chain is recurrent when every state is recurrent.

<h3 id="8h/b">b</h3>

↑ **Parent:** [8H](#8h)

<h4 id="8h/b/solution">Solution</h4>

↑ **Parent:** [B](#8h/b)

A return to zero is possible only at even times, and

$$
P_0(X_{2k}=0)=\binom{2k}{k}[p(1-p)]^k.
$$

Stirling's estimate makes this asymptotic to a positive constant times

$$
\frac{[4p(1-p)]^k}{\sqrt k}.
$$

A state is recurrent exactly when the sum of its return probabilities diverges. If $p=1/2$, the resulting $k^{-1/2}$ [series](../../../real-analysis.md#series-mathematics) diverges. If $p\ne1/2$, then $4p(1-p)<1$ and the [series](../../../real-analysis.md#series-mathematics) converges geometrically. Thus the walk is recurrent exactly when $p=1/2$.

## 9F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9f/a">a</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/a/solution">Solution</h4>

↑ **Parent:** [A](#9f/a)

The [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) $m_\phi$ is the unique monic [polynomial](../../../polynomial.md) of least positive degree with $m_\phi(\phi)=0$. Uniqueness follows because division of one monic annihilator by another would produce a lower-degree annihilator. Cayley–Hamilton says that the characteristic [polynomial](../../../polynomial.md) annihilates $\phi$; division then shows

$$
\boxed{m_\phi\mid\chi_\phi.}
$$

<h3 id="9f/b">b</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/b/solution">Solution</h4>

↑ **Parent:** [B](#9f/b)

The map $\theta:\mathbb C[x]\to V$, $p\mapsto p(\phi)a_1$, is surjective because $1,x,\ldots,x^{n-1}$ map to the given [basis](../../../vector-space.md#basis). Its kernel is generated by the [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) and the quotient has dimension $n$, so $\deg m_\phi=n$. The relation for $\phi(a_n)$ gives

$$
\boxed{m_\phi(x)=x^n-\sum_{k=0}^{n-1}c_{k+1}x^k.}
$$

<h3 id="9f/c">c</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/c/solution">Solution</h4>

↑ **Parent:** [C](#9f/c)

If $V=V_1\oplus V_2$ were a nontrivial invariant decomposition, each restricted minimal [polynomial](../../../polynomial.md) would be a power of $x-\alpha$ of degree at most $\dim V_i<n$. Their least common multiple is the minimal [polynomial](../../../polynomial.md) of $\phi$, contradicting its degree $n$.

Since $m_\phi$ has degree $n$, $\phi$ has a [cyclic vector](../../../linear-operator-theory.md#cyclic-vector) $b_1$. Put $b_k=\phi^{k-1}b_1$. Then $\phi(b_k)=b_{k+1}$ for $k<n$. In this [basis](../../../vector-space.md#basis) the [matrix](../../../vector-space.md#matrix) is the [companion matrix](../../../linear-operator-theory.md#companion-matrix) with ones immediately below the diagonal and last column

$$
c_{k+1}=(-1)^{n-k+1}\binom nk\alpha^{n-k},\qquad0\le k<n,
$$

obtained by expanding $(x-\alpha)^n$.

## 10E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10e/a">a</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/a/solution">Solution</h4>

↑ **Parent:** [A](#10e/a)

The content $c(f)$ is a greatest common divisor of the coefficients, defined up to a unit. A [polynomial](../../../polynomial.md) is primitive when its content is a unit.

<h4 id="10e/a/i">i</h4>

↑ **Parent:** [A](#10e/a)

<h5 id="10e/a/i/solution">Solution</h5>

↑ **Parent:** [I](#10e/a/i)

If a prime divided every coefficient of $fg$, reducing modulo that prime would make the product of the two nonzero reduced primitive [polynomials](../../../polynomial.md) zero in a domain, impossible. Thus a product of primitive [polynomials](../../../polynomial.md) is primitive. Factoring the contents from arbitrary $f,g$ then gives

$$
c(fg)=u,c(f)c(g)
$$

for a unit $u$.

<h4 id="10e/a/ii">ii</h4>

↑ **Parent:** [A](#10e/a)

<h5 id="10e/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10e/a/ii)

Write the rational root in lowest terms as $a/b$. The factor $bx-a$ is primitive and divides $f$ over $\mathbb Q[x]$; Gauss's lemma makes it divide in $\mathbb Z[x]$. Comparison of leading coefficients makes $b$ divide the leading coefficient one, so $b=\pm1$ and the root is [integral](../../../calculus.md#integral).

<h3 id="10e/b">b</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/b/solution">Solution</h4>

↑ **Parent:** [B](#10e/b)

Regard the [polynomial](../../../polynomial.md) as an element of $\mathbb C[x][y]$:

$$
x^3y^3+(x^2-1)y^2+(x^3-1)y+(1-x).
$$

The prime $x-1$ divides every nonleading coefficient, its square does not divide the constant coefficient, and it does not divide the leading coefficient $x^3$. Eisenstein's criterion proves irreducibility over $\mathbb C(x)[y]$; the [polynomial](../../../polynomial.md) is primitive in $\mathbb C[x][y]$, so Gauss's lemma proves irreducibility there.

## 11G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11g/solution">Solution</h3>

↑ **Parent:** [11G](#11g)

A space is connected when it is not a union of two disjoint nonempty open subsets. If $f(X)$ had such a separation, its inverse images would separate connected $X$, so continuous images of [connected spaces](../../../geometry-and-topology.md#connected-space) are connected. Equivalently, a nonconstant continuous map to discrete $\{0,1\}$ records a separation, and every separation defines such a map.

If $\mathbb R$ were separated, points in opposite pieces and the intermediate value theorem applied to the associated $\{0,1\}$-valued map would give a contradiction. Thus $\mathbb R$ is connected. Its quotient by $x\sim y$ is connected because the quotient map is continuous and surjective.

Finally let $A\subset B\subset\operatorname{Cl}(A)$ and suppose $B=U\cup V$ were a separation. Connectedness puts $A$ wholly in one side, say $U$. Every point of $V$ nevertheless lies in the closure of $A$, while $V$ is relatively open and disjoint from $A$, a contradiction. Hence $B$ is connected.

## 12F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12f/solution">Solution</h3>

↑ **Parent:** [12F](#12f)

For a closed surface, $\chi=V-E+F$ for any finite cell decomposition. Gauss–Bonnet for a geodesic polygon says

$$
\int_DK\,dA+\sum\text{ exterior angles}=2\pi\chi(D),
$$

and for a closed smooth surface it says $\int_SK\,dA=2\pi\chi(S)$.

For a large radius, the graph surface bounded over that circle is flat near its boundary. The boundary geodesic-curvature [integral](../../../calculus.md#integral) is $2\pi$, so Gauss–Bonnet on the disc gives $\int K=0$. Since $K\ge0$, continuity forces $K\equiv0$.

For the torus,

$$
K=\frac{\cos u}{2+\cos u}.
$$

Thus $T_+$ has $\cos u>0$ and $T_-$ has $\cos u<0$. Cap the two boundary circles of the outer half $T_+$ by flat discs. The result is a sphere, and the caps contribute no Gaussian curvature, so Gauss–Bonnet gives $\int_{T_+}K=4\pi$. The full torus has [Euler characteristic](../../../homology.md#euler-characteristic) zero, hence total curvature zero and

$$
\boxed{\int_{T_-}K=-4\pi.}
$$

## 13E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="13e/solution">Solution</h3>

↑ **Parent:** [13E](#13e)

Cauchy's formula gives $|f'(z_0)|\le M_R/R$ for an [entire function](../../../complex-analysis.md#entire-function) bounded by $M$ on every radius-$R$ circle. If $f$ is globally bounded, letting $R\to\infty$ gives $f'=0$, proving Liouville's theorem.

Set $h(w)=f(1/w)$. Its [limit](../../../calculus.md#limit-of-a-function) at zero makes the singularity removable, so

$$
h(w)=a+c_1w+c_2w^2+\cdots.
$$

Consequently $f(z)=a+c_1/z+O(z^{-2})$ and $z^2f'(z)\to-c_1=:b$.

The [argument principle](../../../complex-analysis.md#argument-principle) on a large circle gives number of zeros minus poles equal to the winding number of $g$, which is zero because $g\to1$. Thus $m=n$. The [function](../../../function.md)

$$
G(z)=g(z)\frac{\prod_i(z-p_i)}{\prod_j(z-q_j)}
$$

has removable singularities everywhere and tends to one at infinity. Liouville gives $G=1$, hence

$$
\boxed{g(z)=\frac{\prod_j(z-q_j)}{\prod_i(z-p_i)}.}
$$

## 14D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="14d/solution">Solution</h3>

↑ **Parent:** [14D](#14d)

Since

$$
\nabla\cdot(\phi\nabla\psi-\psi\nabla\phi)=\phi\nabla^2\psi-\psi\nabla^2\phi,
$$

the divergence theorem proves Green's second identity.

If $x_0=(x_0,y_0,z_0)$ and $x_0^*=(x_0,y_0,-z_0)$, the image solution is

$$
\psi(x)=-\frac1{4\pi}\left(\frac1{|x-x_0|}-\frac1{|x-x_0^*|}\right).
$$

It vanishes on the plane and has the required unit delta source.

Green's identity yields the Poisson-kernel [integral](../../../calculus.md#integral)

$$
\phi(x_0,y_0,z_0)=\frac1{2\pi}\iint_{x^2+y^2<1}
\frac{z_0\,dx\,dy}{[(x-x_0)^2+(y-y_0)^2+z_0^2]^{3/2}}.
$$

On the axis this becomes

$$
\boxed{\phi(0,0,z)=\int_0^1\frac{zr\,dr}{(r^2+z^2)^{3/2}}
=1-\frac z{\sqrt{1+z^2}}.}
$$

## 15B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="15b/solution">Solution</h3>

↑ **Parent:** [15B](#15b)

With signature $(+---)$ one convenient convention is

$$
F^{\mu\nu}=\begin{pmatrix}
0&-E_x/c&-E_y/c&-E_z/c\\E_x/c&0&-B_z&B_y\\E_y/c&B_z&0&-B_x\\E_z/c&-B_y&B_x&0
\end{pmatrix},
$$

which gives the stated dual after index lowering. The invariants are

$$
F^{\mu\nu}F_{\mu\nu}=2(B^2-E^2/c^2),
$$



$$
F^{\mu\nu}\widetilde F_{\mu\nu}=-4E\cdot B/c,\qquad
\widetilde F^{\mu\nu}\widetilde F_{\mu\nu}=2(E^2/c^2-B^2).
$$

For the boost,

$$
E'_y=\gamma(E_y-vB_z),\quad E'_z=\gamma(E_z+vB_y),
$$



$$
B'_y=\gamma(B_y+vE_z/c^2),\quad B'_z=\gamma(B_z-vE_y/c^2),
$$

with zero $x$ components.

In the final configuration, parallelism gives

$$
\sin\theta\,\beta^2-2\beta+\sin\theta=0,\qquad\beta=v/c.
$$

The physical root is

$$
\beta=\frac{1-\cos\theta}{\sin\theta}=\tan(\theta/2).
$$

**Thus $v\sim c\theta/2$ for small angle. As $\theta\to\pi/2$, $v\to c$, so exactly crossed equal-magnitude null fields cannot be aligned by any finite inertial boost.**

## 16D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="16d/solution">Solution</h3>

↑ **Parent:** [16D](#16d)

The initially irrotational inviscid flow remains irrotational, so $u=\nabla\phi$; incompressibility gives $\nabla^2\phi=0$. At the plates, normal [velocity](../../../classical-mechanics.md#velocity) matches their motion:

$$
\frac1r\phi_\theta(r,\alpha)=-\Omega r,\qquad
\frac1r\phi_\theta(r,-\alpha)=\Omega r.
$$

With $\phi=r^2f(\theta)$, Laplace's equation gives $f''+4f=0$. The symmetric solution is

$$
\phi=\frac{\Omega r^2\cos2\theta}{2\sin2\alpha}.
$$

Hence

$$
u_r=\frac{\Omega r\cos2\theta}{\sin2\alpha},\qquad
u_\theta=-\frac{\Omega r\sin2\theta}{\sin2\alpha}.
$$

A streamfunction is

$$
\psi=\frac{\Omega r^2\sin2\theta}{2\sin2\alpha},
$$

so [streamlines](../../../fluid-mechanics.md#streamline) are $r^2\sin2\theta=\text{constant}$ and fluid is expelled radially as the plates close. The outward flux through $r=R$ is

$$
\boxed{\int_{-\alpha}^{\alpha}u_rR\,d\theta=\Omega R^2.}
$$

## 17B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="17b/a">a</h3>

↑ **Parent:** [17B](#17b)

<h4 id="17b/a/solution">Solution</h4>

↑ **Parent:** [A](#17b/a)

If the monic [orthogonal polynomial](../../../numerical-analysis.md#orthogonal-polynomial) $p_n$ had fewer than $n$ distinct sign-changing zeros in $(-1,1)$, multiply the factors corresponding to those zeros to form a [polynomial](../../../polynomial.md) $q$ of degree below $n$. Then $p_nq$ has one sign and is not identically zero, so its positive-weight [integral](../../../calculus.md#integral) cannot vanish, contradicting orthogonality. Thus all $n$ zeros are distinct and lie in the open interval.

<h3 id="17b/b">b</h3>

↑ **Parent:** [17B](#17b)

<h4 id="17b/b/solution">Solution</h4>

↑ **Parent:** [B](#17b/b)

Expansion of $\det(xI-A_n)$ along the last row gives

$$
D_n=(x-\alpha_n)D_{n-1}-\beta_nD_{n-2},
$$

with $D_0=1$, $D_1=x-\alpha_1$. This is exactly the recurrence defining $P_n$, so induction gives $P_n=\det(xI-A_n)$.

<h3 id="17b/c">c</h3>

↑ **Parent:** [17B](#17b)

<h4 id="17b/c/solution">Solution</h4>

↑ **Parent:** [C](#17b/c)

The three-term recurrence theorem with the displayed coefficients identifies $P_n$ with the monic orthogonal [polynomial](../../../polynomial.md) $p_n$. Part (b) says its zeros are precisely the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of the real symmetric [Jacobi matrix](../../../numerical-analysis.md#jacobi-matrix) $A_n$, and part (a) says those zeros are distinct and all belong to $(-1,1)$.

## 18H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="18h/a">a</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/a/solution">Solution</h4>

↑ **Parent:** [A](#18h/a)

A statistic $T$ is sufficient when the conditional law of the sample given $T$ is independent of the parameter. The factorisation criterion says this holds exactly when

$$
f(x;\theta)=g(T(x);\theta)h(x).
$$

If factorisation holds, cancellation in the conditional mass proves parameter independence. Conversely, multiply the parameter-free conditional mass given $T=t$ by the mass of $T=t$ to obtain the factorisation.

<h3 id="18h/b">b</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/b/solution">Solution</h4>

↑ **Parent:** [B](#18h/b)

Rao–Blackwell says that if $U$ estimates a parameter and $T$ is sufficient, then $U^*=E(U\mid T)$ has the same mean and no larger variance, with strict improvement unless $U$ is already a [function](../../../function.md) of $T$ almost surely. The mean statement is the tower property, while

$$
\operatorname{Var}U=\operatorname{Var}E(U\mid T)+E\operatorname{Var}(U\mid T)
$$

proves the variance claim.

<h3 id="18h/c">c</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/c/solution">Solution</h4>

↑ **Parent:** [C](#18h/c)

The joint mass factorizes through $T=\sum_iX_i$, so $T$ is sufficient for $q$. If $\lambda=\sqrt q$, then

$$
E[X_1^2-X_1]=E[X_1(X_1-1)]=\lambda^2=q.
$$

Conditionally on $T$, $X_1\sim\operatorname{Bin}(T,1/n)$. Rao–Blackwell therefore gives the unbiased estimator

$$
E[X_1(X_1-1)\mid T]=\frac{T(T-1)}{n^2}.
$$

For $n\ge2$ the original estimator is not a [function](../../../function.md) of $T$, so the variance reduction is strict.

## 19H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="19h/a">a</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/a/solution">Solution</h4>

↑ **Parent:** [A](#19h/a)

For probability [vectors](../../../vector-space.md#vector) $p,q$, they are optimal with value $v$ exactly when

$$
p^TAe_j\ge v\quad\text{for every column }j,\qquad
e_i^TAq\le v\quad\text{for every row }i,
$$

and $p^TAq=v$. These are the mutual best-response and security-level conditions.

<h3 id="19h/b">b</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/b/solution">Solution</h4>

↑ **Parent:** [B](#19h/b)

For every probability [vector](../../../vector-space.md#vector) $x$, antisymmetry gives $x^TAx=0$. Applying the minimax inequalities with the same strategy on both sides shows the lower value is at most zero and the upper value at least zero; transposition also changes the value to its negative. Hence the value is zero.

<h3 id="19h/c">c</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/c/solution">Solution</h4>

↑ **Parent:** [C](#19h/c)

Starting from any optimal strategy, transfer all probability on row $i_0$ to row $i_1$. Every payoff against a pure column weakly increases, so the security level remains optimal. The resulting strategy has $p_{i_0}=0$.

<h3 id="19h/d">d</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/d/solution">Solution</h4>

↑ **Parent:** [D](#19h/d)

The [matrix](../../../vector-space.md#matrix) is antisymmetric, so the value is zero. For a common candidate $p=(a,b,c,d)^T$, the column-player inequalities are $Ap\le0$:

$$
b-c\le0,\qquad-a+c+2d\le0,\qquad a-b+d\le0,\qquad-2b-c\le0.
$$

The first three imply $a+d\le b\le c\le a-2d$, hence $d=0$ and $a=b=c$. Normalization gives

$$
p=q=(1/3,1/3,1/3,0)^T.
$$

Indeed $Ap=(0,0,0,-1)^T/3\le0$, and antisymmetry gives the corresponding row inequalities.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
