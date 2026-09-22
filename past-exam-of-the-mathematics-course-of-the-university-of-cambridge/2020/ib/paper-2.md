# Paper 2

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2020/paperib_2_2020.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2020/paperib_2_2020.pdf)

**Table of contents**

- [1G](#1g)
  - [Solution](#1g/solution)
- [2E](#2e)
  - [Solution](#2e/solution)
- [3D](#3d)
  - [Solution](#3d/solution)
- [4B](#4b)
  - [Solution](#4b/solution)
- [5D](#5d)
  - [Solution](#5d/solution)
- [6C](#6c)
  - [Solution](#6c/solution)
- [7H](#7h)
  - [Solution](#7h/solution)
- [8F](#8f)
  - [i](#8f/i)
    - [Solution](#8f/i/solution)
  - [ii](#8f/ii)
    - [Solution](#8f/ii/solution)
  - [iii](#8f/iii)
    - [Solution](#8f/iii/solution)
  - [iv](#8f/iv)
    - [Solution](#8f/iv/solution)
- [9G](#9g)
  - [Solution](#9g/solution)
- [10E](#10e)
  - [i](#10e/i)
    - [Solution](#10e/i/solution)
  - [ii](#10e/ii)
    - [Solution](#10e/ii/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12B](#12b)
  - [i](#12b/i)
    - [Solution](#12b/i/solution)
  - [ii](#12b/ii)
    - [Solution](#12b/ii/solution)
  - [iii](#12b/iii)
    - [Solution](#12b/iii/solution)
- [13A](#13a)
  - [i](#13a/i)
    - [Solution](#13a/i/solution)
  - [ii](#13a/ii)
    - [Solution](#13a/ii/solution)
- [14A](#14a)
  - [a](#14a/a)
    - [Solution](#14a/a/solution)
  - [b](#14a/b)
    - [Solution](#14a/b/solution)
- [15D](#15d)
  - [a](#15d/a)
    - [Solution](#15d/a/solution)
  - [b](#15d/b)
    - [Solution](#15d/b/solution)
- [16C](#16c)
  - [a](#16c/a)
    - [Solution](#16c/a/solution)
  - [b](#16c/b)
    - [Solution](#16c/b/solution)
  - [c](#16c/c)
    - [Solution](#16c/c/solution)
- [17C](#17c)
  - [a](#17c/a)
    - [Solution](#17c/a/solution)
  - [b](#17c/b)
    - [Solution](#17c/b/solution)
  - [c](#17c/c)
    - [Solution](#17c/c/solution)
- [18H](#18h)
  - [a](#18h/a)
    - [Solution](#18h/a/solution)
  - [b](#18h/b)
    - [Solution](#18h/b/solution)
  - [c](#18h/c)
    - [Solution](#18h/c/solution)
  - [d](#18h/d)
    - [Solution](#18h/d/solution)
  - [e](#18h/e)
    - [Solution](#18h/e/solution)
- [19H](#19h)
  - [Solution](#19h/solution)

## 1G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1g/solution">Solution</h3>

↑ **Parent:** [1G](#1g)

Fix $\alpha\in\Omega$. If $\beta=g\alpha$, then normality of $H$ gives

$$
g(H\alpha)=(gHg^{-1})(g\alpha)=H\beta.
$$

Thus the transitive [group action](../../../group-theory.md#group-action) of $G$ permutes the [orbits of a group action](../../../group-theory.md#orbit-of-a-group-action) of $H$, so all $H$-orbits have the same cardinality $d$. They partition the prime-sized set $\Omega$, hence $d$ divides $|\Omega|$. The only possibilities are $d=1$ and $d=|\Omega|$. The first would make every element of $H$ fix every point, contrary to the assumption that $H$ acts nontrivially. Therefore $d=|\Omega|$ and

$$
\boxed{H\text{ acts transitively on }\Omega}.
$$

Now suppose $H\cap G_\alpha=\{1\}$. Define the [orbit map](../../../group-theory.md#orbit-map)

$$
\theta:H\longrightarrow\Omega,
\qquad
\theta(h)=h\alpha.
$$

It is surjective by transitivity of $H$. If $\theta(h_1)=\theta(h_2)$, then $h_2^{-1}h_1\in H\cap G_\alpha$, so $h_1=h_2$; hence $\theta$ is bijective. For $k\in G_\alpha$,

$$
\theta(khk^{-1})
=khk^{-1}\alpha
=kh\alpha
=k\theta(h).
$$

**Thus $\theta$ is an [equivariant map](../../../group-theory.md#equivariant-map): [conjugation](../../../group-theory.md#conjugation) by $G_\alpha$ on $H$ corresponds exactly to the given action of $G_\alpha$ on $\Omega$.**

## 2E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2e/solution">Solution</h3>

↑ **Parent:** [2E](#2e)

Write $D(f)=\mathbb C\setminus f^{-1}(0)$. The zero and constant-one polynomials give $D(0)=\varnothing$ and $D(1)=\mathbb C$. Also,

$$
D(f)\cap D(g)=D(fg),
$$

so $\tau$ is closed under finite intersections. Every nonzero one-variable complex polynomial has only finitely many roots, and every finite subset $\{a_1,\ldots,a_m\}$ is the zero set of $\prod_j(z-a_j)$. Consequently $\tau$ is exactly the [cofinite topology](../../../topology.md#cofinite-topology): its open sets are the empty set and the complements of finite sets. An arbitrary union of such sets is again empty or has finite complement, so $\tau$ is a [topology](../../../topology.md).

The [product topology](../../../geometry-and-topology.md#product-topology) on $X\times Y$ is the topology with basis

$$
\{U\times V:U\subseteq X\text{ open},\ V\subseteq Y\text{ open}\}.
$$

The proposed complement need not be open. Take

$$
g(z,w)=z-w.
$$

Then $g^{-1}(0)$ is the diagonal. If its complement were open, a point such as $(0,1)$ would have a basic neighbourhood $U\times V$ contained in that complement. But $U$ and $V$ are nonempty cofinite subsets of $\mathbb C$, so $U\cap V\ne\varnothing$. For $t\in U\cap V$, the point $(t,t)$ belongs both to $U\times V$ and to the diagonal, a contradiction. Hence

$$
\boxed{\mathbb C^2\setminus g^{-1}(0)\text{ is not always product-open}}.
$$

## 3D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3d/solution">Solution</h3>

↑ **Parent:** [3D](#3d)

Because the constraint determines

$$
x=b^2-a^2y^2-z^2,
$$

the constrained function is

$$
\Phi(y,z)=yz(b^2-a^2y^2-z^2).
$$

Its [stationary points](../../../calculus-of-variations.md#stationary-point) satisfy

$$
\frac{\partial\Phi}{\partial y}
=z(b^2-3a^2y^2-z^2)=0,
\qquad
\frac{\partial\Phi}{\partial z}
=y(b^2-a^2y^2-3z^2)=0.
$$

When $yz=0$, these equations give

$$
(x,y,z)=(b^2,0,0),\quad
(0,\pm b/a,0),\quad
(0,0,\pm b).
$$

When $yz\ne0$, subtracting the two bracketed equations gives $z^2=a^2y^2$, and substitution then gives

$$
x=\frac{b^2}{2},
\qquad
y=\pm\frac b{2a},
\qquad
z=\pm\frac b2,
$$

with the two signs chosen independently. These are exactly the constrained stationary points; equivalently they follow from the [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) equations.

Under the additional restriction $x\ge0$, the constraint gives the compact elliptical disc $a^2y^2+z^2\le b^2$. On its boundary $x=0$, the objective is zero. At the four nonzero interior stationary points,

$$
\phi=xyz=\pm\frac{b^4}{8a},
$$

with the sign determined by $yz$. Therefore

$$
\boxed{\max\phi=\frac{b^4}{8a},
\qquad
\min\phi=-\frac{b^4}{8a}}.
$$

## 4B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4b/solution">Solution</h3>

↑ **Parent:** [4B](#4b)

Use the angular-frequency [Fourier transform](../../../analysis.md#fourier-transform)

$$
\widehat f(k)=\int_{-\infty}^{\infty}f(x)e^{-ikx}\,dx.
$$

Then

$$
\boxed{\widehat f(k)=A\int_{-1}^{1}e^{-ikx}\,dx
=2A\frac{\sin k}{k}},
$$

with the continuous value $\widehat f(0)=2A$.

The [convolution](../../../fourier-analysis.md#convolution) $(f*f)(x)$ is $A^2$ times the length of the overlap of the intervals $[-1,1]$ and $[x-1,x+1]$. Thus

$$
\boxed{(f*f)(x)=
\begin{cases}
A^2(2-|x|),&|x|\le2,\\
0,&|x|>2.
\end{cases}}
$$

The [convolution theorem](../../../fourier-analysis.md#convolution-theorem) states, for this convention, that

$$
\widehat{u*v}(k)=\widehat u(k)\widehat v(k).
$$

Since $g=(B/A^2)(f*f)$, it follows that

$$
\boxed{\widehat g(k)
=4B\left(\frac{\sin k}{k}\right)^2},
$$

again interpreted continuously at $k=0$, where $\widehat g(0)=4B$.

## 5D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5d/solution">Solution</h3>

↑ **Parent:** [5D](#5d)

Let $r$ be distance from the common centre. By [Gauss's law](../../../electromagnetism.md#gauss-s-law), the [electric field](../../../electromagnetism.md#electric-field) is radial and equals

$$
\boxed{
\mathbf E(r)=
\begin{cases}
0,&0\le r<R,\\[2mm]
\dfrac{Q_1}{4\pi\epsilon_0r^2}\,\widehat{\mathbf r},
&R<r<2R,\\[3mm]
\dfrac{Q_1+Q_2}{4\pi\epsilon_0r^2}\,\widehat{\mathbf r},
&r>2R.
\end{cases}}
$$

Taking the [electric potential](../../../electromagnetism.md#electric-potential) to vanish at infinity and requiring continuity across each shell gives

$$
\boxed{
\Phi(r)=\frac1{4\pi\epsilon_0}
\begin{cases}
\dfrac{Q_1}{R}+\dfrac{Q_2}{2R},&0\le r\le R,\\[3mm]
\dfrac{Q_1}{r}+\dfrac{Q_2}{2R},&R\le r\le2R,\\[3mm]
\dfrac{Q_1+Q_2}{r},&r\ge2R.
\end{cases}}
$$

The [electrostatic energy](../../../electromagnetism.md#electrostatic-energy) is the integral of the electric-field energy density:

$$
U=\frac{\epsilon_0}{2}\int_{\mathbb R^3}|\mathbf E|^2\,dV.
$$

Only the two nonzero-field regions contribute, so

$$
U=\frac{Q_1^2}{8\pi\epsilon_0}
\int_R^{2R}\frac{dr}{r^2}
+\frac{(Q_1+Q_2)^2}{8\pi\epsilon_0}
\int_{2R}^{\infty}\frac{dr}{r^2}.
$$

Therefore

$$
\boxed{U
=\frac{Q_1^2+(Q_1+Q_2)^2}{16\pi\epsilon_0R}
=\frac{2Q_1^2+2Q_1Q_2+Q_2^2}{16\pi\epsilon_0R}}.
$$

## 6C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6c/solution">Solution</h3>

↑ **Parent:** [6C](#6c)

Let the upper plate in flow A move at speed $U$, with the lower plate fixed. The [Couette flow](../../../viscous-fluid-flow.md#couette-flow) profile is

$$
u_A(y)=\frac Uh\,y,
$$

so its mid-plane speed is $U/2$ and its total [viscous dissipation](../../../stokes-flow.md#viscous-dissipation) per unit plate area is

$$
\dot Q_A=\int_0^h\mu\left(\frac Uh\right)^2dy
=\frac{\mu U^2}{h}.
$$

Write $G=-dp/dx>0$ for the constant pressure-gradient magnitude in flow B. The [plane Poiseuille flow](../../../viscous-fluid-flow.md#plane-poiseuille-flow) profile is

$$
u_B(y)=\frac{G}{2\mu}y(h-y).
$$

Equality of the mid-plane speeds gives

$$
\frac{Gh^2}{8\mu}=\frac U2,
\qquad
G=\frac{4\mu U}{h^2}.
$$

Since $u_B'(y)=G(h-2y)/(2\mu)$,

$$
\dot Q_B
=\frac{G^2}{4\mu}\int_0^h(h-2y)^2dy
=\frac{G^2h^3}{12\mu}
=\frac{4\mu U^2}{3h}.
$$

Hence

$$
\boxed{\frac{\dot Q_A}{\dot Q_B}=\frac34}.
$$

## 7H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7h/solution">Solution</h3>

↑ **Parent:** [7H](#7h)

Set

$$
p_n=\mathbb P(X_n=1\mid X_0=1).
$$

Conditioning on $X_n$ gives the affine recurrence

$$
p_{n+1}=(1-\alpha)p_n+\beta(1-p_n)
=\beta+(1-\alpha-\beta)p_n.
$$

Its fixed point is the first component of the [stationary distribution](../../../markov-process.md#stationary-distribution),

$$
\pi_1=\frac{\beta}{\alpha+\beta}.
$$

Thus $p_n-\pi_1=(1-\alpha-\beta)^n(p_0-\pi_1)$, and $p_0=1$ gives

$$
\boxed{\mathbb P(X_n=1\mid X_0=1)
=\frac{\beta}{\alpha+\beta}
+\frac{\alpha}{\alpha+\beta}(1-\alpha-\beta)^n}.
$$

Starting instead from state two gives the same recurrence with initial value zero. Therefore

$$
\boxed{\mathbb P(X_n=1\mid X_0=2)
=\frac{\beta}{\alpha+\beta}
\left[1-(1-\alpha-\beta)^n\right]}.
$$

## 8F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8f/i">i</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/i/solution">Solution</h4>

↑ **Parent:** [I](#8f/i)

An endomorphism $\alpha$ is a projection onto its image precisely when it is the identity on $\operatorname{im}\alpha$ and kills a complementary subspace. If $\alpha^2=\alpha$, then

$$
\alpha(\alpha v)=\alpha v,
$$

so $\alpha$ is the identity on its image. Moreover,

$$
v=\alpha v+(v-\alpha v),
\qquad
\alpha(v-\alpha v)=0,
$$

and $\operatorname{im}\alpha\cap\ker\alpha=\{0\}$. Hence

$$
V=\operatorname{im}\alpha\oplus\ker\alpha,
$$

and $\alpha$ is the projection onto its image along its kernel. Conversely, every projection is the identity after one application, so applying it twice has the same effect: $\alpha^2=\alpha$.

Statement (i) is **false**. On a two-dimensional vector space, take the nonzero nilpotent endomorphism

$$
\alpha=
\begin{pmatrix}
0&1\\
0&0
\end{pmatrix}.
$$

Then $\alpha^2=\alpha^3=0$, but $\alpha^2\ne\alpha$, so $\alpha$ is not [idempotent](../../../commutative-algebra.md#idempotent).

<h3 id="8f/ii">ii</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8f/ii)

Statement (ii) is **false**. The condition is necessary for an idempotent, but it is not sufficient. For example,

$$
\alpha=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

satisfies $(I-\alpha)^2=0$, hence $\alpha(I-\alpha)^2=0$, while

$$
\alpha^2=
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix}\ne\alpha
$$

over, for example, $\mathbb Q$.

<h3 id="8f/iii">iii</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#8f/iii)

Statement (iii) is **false over an arbitrary field**. Expanding the assumed idempotence gives

$$
(\alpha+\beta)^2=\alpha+\beta
\quad\Longrightarrow\quad
\alpha\beta+\beta\alpha=0.
$$

Multiplying this relation on the left and right by $\alpha$ shows

$$
\alpha\beta=-\alpha\beta\alpha=\beta\alpha.
$$

**Thus $2\alpha\beta=0$, so the conclusion would be true in characteristic different from two. In characteristic two, however, take $\alpha=\beta=I$. Then $\alpha$, $\beta$, and $\alpha+\beta=0$ are idempotent, but $\alpha\beta=I\ne0$.**

<h3 id="8f/iv">iv</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#8f/iv)

Statement (iv) is **false** because $\alpha\beta=0$ need not imply $\beta\alpha=0$. For example, over any field take

$$
\alpha=
\begin{pmatrix}
1&0\\
0&0
\end{pmatrix},
\qquad
\beta=
\begin{pmatrix}
0&0\\
1&1
\end{pmatrix}.
$$

Both maps are idempotent and $\alpha\beta=0$, but

$$
\beta\alpha=
\begin{pmatrix}
0&0\\
1&0
\end{pmatrix}\ne0.
$$

Consequently

$$
\boxed{(\alpha+\beta)^2=\alpha+\beta+\beta\alpha\ne\alpha+\beta.}
$$

## 9G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9g/solution">Solution</h3>

↑ **Parent:** [9G](#9g)

[Gauss lemma for polynomials](../../../commutative-algebra.md#gauss-lemma-for-polynomials) states that the product of two [primitive polynomials](../../../commutative-algebra.md#primitive-polynomial) over a [unique factorization domain](../../../algebra.md#unique-factorization-domain) is primitive. In particular, a primitive polynomial in $\mathbb Z[X]$ is reducible over $\mathbb Q$ exactly when it is reducible over $\mathbb Z$.

[Eisenstein criterion](../../../commutative-algebra.md#eisenstein-criterion) says that a primitive polynomial

$$
F(X)=a_nX^n+\cdots+a_0\in\mathbb Z[X]
$$

is irreducible over $\mathbb Q$ if there is a prime $p$ such that $p\nmid a_n$, $p\mid a_j$ for every $j<n$, and $p^2\nmid a_0$. To prove it, suppose $F=GH$ with both factors of positive degree. After removing contents, Gauss's lemma lets us take $G,H\in\mathbb Z[X]$ primitive. Reduction modulo $p$ gives

$$
\overline F=a_nX^n=\overline G\,\overline H,
$$

so both reduced factors are monomials of positive degree. Their constant terms are therefore divisible by $p$, making $p^2$ divide $a_0=G(0)H(0)$, a contradiction.

An [algebraic integer](../../../algebraic-number-theory.md#algebraic-integer) is a complex number satisfying a monic polynomial in $\mathbb Z[X]$. Let $\alpha$ be one and let $m_\alpha\in\mathbb Q[X]$ be its monic [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial). The usual proof using polynomial content shows that $m_\alpha\in\mathbb Z[X]$. The set

$$
I_\alpha=\{f\in\mathbb Z[X]:f(\alpha)=0\}
$$

is the kernel of the polynomial-evaluation [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism), hence an ideal. Every $f\in I_\alpha$ is divisible by $m_\alpha$ in $\mathbb Q[X]$. Because $m_\alpha$ is monic, polynomial division of $f$ by $m_\alpha$ takes place in $\mathbb Z[X]$, and the remainder must vanish by minimality. Therefore

$$
\boxed{I_\alpha=(m_\alpha)},
$$

where $m_\alpha$ is monic and irreducible.

For

$$
f(X)=X^4+2X^3-3X^2-4X-11,
$$

translation gives

$$
f(X+1)=X^4+6X^3+9X^2-15.
$$

This is Eisenstein at $p=3$, so $f(X+1)$ and therefore $f(X)$ are irreducible over $\mathbb Q$. Hence

$$
\boxed{\mathbb Q[X]/(f)\text{ is a field}}.
$$

Irreducibility and Gauss's lemma also show that $(f)$ is a [prime ideal](../../../commutative-algebra.md#prime-ideal) of $\mathbb Z[X]$, so

$$
\boxed{\mathbb Z[X]/(f)\text{ is an integral domain}}.
$$

It is not a field. The class of $2$ is nonzero but not a unit: reducing further modulo $2$ gives a nonzero quotient

$$
\mathbb F_2[X]/(\overline f),
$$

in which the image of $2$ is zero, whereas a unit must remain a unit under every unital quotient map. Thus

$$
\boxed{\mathbb Z[X]/(f)\text{ is not a field}}.
$$

## 10E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10e/i">i</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/i/solution">Solution</h4>

↑ **Parent:** [I](#10e/i)

Here

$$
d_1(f,g)=\int_0^1|f(x)-g(x)|\,dx,
\qquad
d_\infty(f,g)=\max_{x\in[0,1]}|f(x)-g(x)|.
$$

The [L1 norm](../../../functional-analysis.md#l1-norm) and [uniform norm](../../../functional-analysis.md#supremum-norm) satisfy

$$
d_1(f,g)\le d_\infty(f,g),
$$

so the identity from the $d_\infty$ metric to the $d_1$ metric is one-Lipschitz and therefore continuous. The two metrics do not induce the same topology on all of $C[0,1]$. For

$$
f_n(x)=\max(1-nx,0),
$$

one has $d_1(f_n,0)=1/(2n)\to0$ but $d_\infty(f_n,0)=1$. Thus $d_1$ convergence need not imply uniform convergence.

A map $F:(X,d_X)\to(Y,d_Y)$ is [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) if there is $L<\infty$ such that

$$
d_Y(F(x),F(x'))\le Ld_X(x,x')
$$

for all $x,x'\in X$. Evaluation at $a\in[0,1]$ is one-Lipschitz because

$$
|f(a)-g(a)|\le d_\infty(f,g).
$$

Choose distinct $a_0,\ldots,a_n\in[0,1]$ and define

$$
T:\mathcal P_n\longrightarrow\mathbb R^{n+1},
\qquad
T(p)=(p(a_0),\ldots,p(a_n)).
$$

The [Vandermonde determinant](../../../galois-theory.md#vandermonde-determinant) is nonzero, so $T$ is a bijection. It is one-Lipschitz for the two uniform metrics. If $\ell_i$ are the associated [Lagrange cardinal polynomials](../../../numerical-analysis.md#lagrange-polynomial), then

$$
p(x)=\sum_{i=0}^np(a_i)\ell_i(x),
$$

and hence

$$
\|p-q\|_\infty
\le\left(\sum_{i=0}^n\|\ell_i\|_\infty\right)
\|T(p)-T(q)\|_\infty.
$$

Thus $T^{-1}$ is also Lipschitz.

Let $\widehat{\mathcal P}_n$ be the polynomials whose values lie in $[-1,1]$. Its image under $T$ lies in the bounded cube $[-1,1]^{n+1}$. It is closed: if $T(p_j)\to v$, then the Lipschitz inverse gives uniform convergence $p_j\to p=T^{-1}(v)$, and passing to the limit pointwise preserves $|p(x)|\le1$. By the [Heine-Borel theorem](../../../topology.md#heine-borel-theorem), $T(\widehat{\mathcal P}_n)$ is compact, and the continuous inverse carries compactness back to $\widehat{\mathcal P}_n$. Therefore

$$
\boxed{(\widehat{\mathcal P}_n,d_\infty)\text{ is compact}}.
$$

<h3 id="10e/ii">ii</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10e/ii)

The identity map

$$
\operatorname{id}:
(\widehat{\mathcal P}_n,d_\infty)
\longrightarrow
(\widehat{\mathcal P}_n,d_1)
$$

is a continuous bijection by $d_1\le d_\infty$. Its domain is compact by part (i), and its codomain is a [Hausdorff space](../../../topology.md#hausdorff-space) because every metric space is Hausdorff. The [compact-to-Hausdorff continuous bijection theorem](../../../topology.md#compact-to-hausdorff-continuous-bijection-theorem) therefore makes the identity a homeomorphism. Consequently

$$
\boxed{d_1\text{ and }d_\infty\text{ induce the same topology on }\widehat{\mathcal P}_n}.
$$

## 11F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

For a continuously differentiable curve $\gamma(t)=x(t)+iy(t)$ in the [Poincaré half-plane model](../../../geometry-and-topology.md#poincare-half-plane-model), its hyperbolic length is

$$
\boxed{L_H(\gamma)=\int_a^b
\frac{\sqrt{\dot x(t)^2+\dot y(t)^2}}{y(t)}\,dt}.
$$

The hyperbolic lines are the [geodesics](../../../geometry-and-topology.md#geodesic-in-the-poincare-half-plane-model): vertical Euclidean lines and Euclidean semicircles whose centres lie on the real axis.

The unique hyperbolic line through distinct $z,w\in H$ can be carried by an upper-half-plane [Möbius transformation](../../../group-theory.md#mobius-transformation) to the imaginary axis. Such transformations are isometries by hypothesis, so it is enough to consider endpoints $iy_0$ and $iy_1$. Every joining curve satisfies

$$
L_H(\gamma)
\ge\int_a^b\frac{|\dot y|}{y}\,dt
\ge\left|\log\frac{y_1}{y_0}\right|.
$$

Equality holds for the monotone vertical parametrization

$$
\gamma(t)=iy_0\exp\!\left(t\log\frac{y_1}{y_0}\right),
\qquad 0\le t\le1.
$$

Thus the appropriately parametrized hyperbolic-line segment $[z,w]$ attains the infimum defining $\rho(z,w)$.

Now let $l,m$ have positive infimum distance. They neither intersect nor share an ideal endpoint: an intersection would give distance zero directly, while lines sharing an ideal endpoint approach one another arbitrarily closely near that endpoint. Hence they are ultraparallel. An upper-half-plane isometry puts them into the form

$$
l=\{re^{i\theta}:0<\theta<\pi\},
\qquad
m=\{Re^{i\theta}:0<\theta<\pi\},
\qquad 0<r<R.
$$

This is the normal form underlying the [common perpendicular of ultraparallel hyperbolic lines](../../../geometry-and-topology.md#common-perpendicular-of-ultraparallel-hyperbolic-lines). Put $z=e^{u+i\theta}$. Since

$$
dx^2+dy^2=e^{2u}(du^2+d\theta^2),
\qquad
y=e^u\sin\theta,
$$

the metric becomes

$$
ds^2=\frac{du^2+d\theta^2}{\sin^2\theta}.
$$

Every path from $l$ to $m$ therefore has

$$
L_H\ge\int|du|\ge\log\frac Rr.
$$

Equality requires $\theta=\pi/2$ and monotone $u$, so it is attained on the imaginary axis, which meets both semicircles orthogonally. Its intersection points $ir$ and $iR$ realize the distance

$$
\boxed{d=\log(R/r)}.
$$

For a nonattained example, take the vertical lines $l=\{iy:y>0\}$ and $m=\{1+iy:y>0\}$. They share the ideal endpoint at infinity. The horizontal segment at height $y$ has hyperbolic length $1/y$, so their infimum distance is zero, but distinct points of $H$ always have positive distance. Hence the infimum is not attained.

## 12B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12b/i">i</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/i/solution">Solution</h4>

↑ **Parent:** [I](#12b/i)

The [partial fraction decomposition](../../../isolated-singularity.md#partial-fraction-decomposition) is

$$
f(z)=-\frac1{2z}+\frac1{2(z-2)}.
$$

For $0<|z|<2$, expand the second term as a [geometric series](../../../real-analysis.md#geometric-series):

$$
\frac1{2(z-2)}
=-\frac14\frac1{1-z/2}
=-\sum_{n=0}^{\infty}\frac{z^n}{2^{n+2}}.
$$

Hence

$$
\boxed{f(z)=-\frac1{2z}
-\sum_{n=0}^{\infty}\frac{z^n}{2^{n+2}}},
\qquad 0<|z|<2.
$$

<h3 id="12b/ii">ii</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#12b/ii)

For $|z|>2$, expand directly in inverse powers:

$$
f(z)=\frac1{z^2}\frac1{1-2/z}.
$$

Therefore the outer [Laurent series](../../../analysis.md#laurent-series) is

$$
\boxed{f(z)=\sum_{n=0}^{\infty}\frac{2^n}{z^{n+2}}},
\qquad |z|>2.
$$

<h3 id="12b/iii">iii</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#12b/iii)

Put $w=z-1$. Then

$$
f(z)=\frac1{(w+1)(w-1)}
=-\frac1{1-w^2}.
$$

Thus

$$
\boxed{f(z)=-\sum_{n=0}^{\infty}(z-1)^{2n}},
\qquad 0<|z-1|<1.
$$

This is actually a [Taylor series](../../../calculus.md#taylor-series), because $z=1$ is a regular point. The point $z=0$ is a [simple pole](../../../isolated-singularity.md#simple-pole). At infinity,

$$
f(1/w)=\frac{w^2}{1-2w}
$$

extends analytically to $w=0$, so infinity is a [removable singularity](../../../isolated-singularity.md#removable-singularity) of $f$, with extended value zero.

For the real integral, first write

$$
\frac{2-\cos\theta}{5-4\cos\theta}
=\frac14+\frac{3}{4(5-4\cos\theta)}.
$$

Let

$$
J=\int_0^{2\pi}\frac{d\theta}{5-4\cos\theta}.
$$

With $z=e^{i\theta}$,

$$
J=\oint_{|z|=1}\frac{dz}{i(-2z^2+5z-2)}.
$$

The denominator has roots $1/2$ and $2$, so only $1/2$ lies inside the contour. Its [residue](../../../analysis.md#residue) is $1/(3i)$, and the [residue theorem](../../../analysis.md#residue-theorem) gives

$$
J=2\pi i\frac1{3i}=\frac{2\pi}{3}.
$$

Consequently

$$
\boxed{\int_0^{2\pi}\frac{2-\cos\theta}{5-4\cos\theta}\,d\theta
=\frac{\pi}{2}+\frac34\frac{2\pi}{3}
=\pi}.
$$

## 13A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="13a/i">i</h3>

↑ **Parent:** [13A](#13a)

<h4 id="13a/i/solution">Solution</h4>

↑ **Parent:** [I](#13a/i)

Let

$$
u(x)=J_0(\alpha x),
\qquad
v(x)=J_0(\beta x).
$$

Their [Bessel equations](../../../analysis.md#bessel-differential-equation) in self-adjoint form are

$$
(xu')'+\alpha^2xu=0,
\qquad
(xv')'+\beta^2xv=0.
$$

Multiply the first by $v$, the second by $u$, subtract, and integrate. The left side becomes a boundary term:

$$
\left[x(vu'-uv')\right]_0^1
+(\alpha^2-\beta^2)\int_0^1uvx\,dx=0.
$$

Regularity at zero makes the lower boundary term vanish, while

$$
u'(1)=\alpha J_0'(\alpha),
\qquad
v'(1)=\beta J_0'(\beta).
$$

Therefore

$$
\boxed{
\int_0^1J_0(\alpha x)J_0(\beta x)x\,dx
=\frac{\beta J_0(\alpha)J_0'(\beta)
-\alpha J_0(\beta)J_0'(\alpha)}
{\alpha^2-\beta^2}}.
$$

If $\alpha=\gamma_k$ and $\beta=\gamma_\ell$ with $k\ne\ell$, both endpoint values of $J_0$ vanish, so the integral is zero. This is the weighted [orthogonality](../../../linear-algebra.md#orthogonal-vectors) of distinct eigenfunctions in a [Sturm-Liouville problem](../../../analysis.md#sturm-liouville-problem). For the norm, hold $\alpha=\gamma_k$ and let $\beta\to\gamma_k$. Since

$$
J_0(\beta)=J_0'(\gamma_k)(\beta-\gamma_k)
+o(\beta-\gamma_k),
$$

the quotient tends to

$$
\boxed{\int_0^1J_0(\gamma_kx)^2x\,dx
=\frac12J_0'(\gamma_k)^2}.
$$

<h3 id="13a/ii">ii</h3>

↑ **Parent:** [13A](#13a)

<h4 id="13a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#13a/ii)

By [separation of variables](../../../partial-differential-equation.md#separation-of-variables), the axisymmetric [normal modes](../../../wave-equation.md#normal-mode) satisfying regularity at $r=0$ and the fixed-edge condition at $r=1$ are

$$
J_0(\gamma_kr)\cos(\gamma_kt),
\qquad
J_0(\gamma_kr)\sin(\gamma_kt),
$$

where $J_0(\gamma_k)=0$. The zero initial displacement removes all cosine terms, so

$$
z(r,t)=\sum_{k=1}^{\infty}
C_kJ_0(\gamma_kr)\sin(\gamma_kt).
$$

Differentiating at $t=0$ gives the weighted Fourier-Bessel expansion

$$
U\mathbf1_{\{r<b\}}
=\sum_{k=1}^{\infty}\gamma_kC_kJ_0(\gamma_kr).
$$

Multiply by $rJ_0(\gamma_\ell r)$ and integrate from zero to one. The orthogonality and norm from part (i) give

$$
\frac12\gamma_\ell C_\ell J_0'(\gamma_\ell)^2
=U\int_0^b rJ_0(\gamma_\ell r)\,dr.
$$

Using

$$
\frac{d}{dr}\bigl[rJ_1(\gamma r)\bigr]
=\gamma rJ_0(\gamma r),
\qquad
J_1(x)=-J_0'(x),
$$

the remaining integral is

$$
\int_0^b rJ_0(\gamma_\ell r)\,dr
=-\frac b{\gamma_\ell}J_0'(\gamma_\ell b).
$$

Hence

$$
\boxed{
C_k=-\frac{2bU\,J_0'(\gamma_kb)}
{\gamma_k^2J_0'(\gamma_k)^2}},
$$

and therefore

$$
\boxed{
z(r,t)=\sum_{k=1}^{\infty}
C_kJ_0(\gamma_kr)\sin(\gamma_kt)}.
$$

## 14A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="14a/a">a</h3>

↑ **Parent:** [14A](#14a)

<h4 id="14a/a/solution">Solution</h4>

↑ **Parent:** [A](#14a/a)

For a one-dimensional wavefunction, the [probability current](../../../quantum-mechanics.md#probability-current) is

$$
j=\frac{\hbar}{2mi}
\left(\psi^*\frac{d\psi}{dx}
-\psi\frac{d\psi^*}{dx}\right).
$$

A plane wave $De^{ikx}$ carries current $(\hbar k/m)|D|^2$ to the right, while $De^{-ikx}$ carries the negative of this current. Thus the asymptotic terms are interpreted as an incident wave of amplitude $A$, a reflected wave of amplitude $B$, and a transmitted wave of amplitude $C$. Their currents are

$$
j_{\rm in}=\frac{\hbar k}{m}|A|^2,
\qquad
j_{\rm ref}=-\frac{\hbar k}{m}|B|^2,
\qquad
j_{\rm tr}=\frac{\hbar k}{m}|C|^2.
$$

Current conservation for a real potential gives $j_{\rm in}+j_{\rm ref}=j_{\rm tr}$, and therefore

$$
\boxed{P_{\rm ref}=\frac{|B|^2}{|A|^2},
\qquad
P_{\rm tr}=\frac{|C|^2}{|A|^2}},
$$

with $P_{\rm ref}+P_{\rm tr}=1$.

A normalizable [bound state](../../../quantum-mechanics.md#bound-state) has $E<0$. Writing

$$
\kappa=\frac{\sqrt{-2mE}}{\hbar}>0,
$$

its decaying asymptotic behaviour is

$$
\boxed{\psi(x)\sim D_-e^{\kappa x}\quad(x\to-\infty),
\qquad
\psi(x)\sim D_+e^{-\kappa x}\quad(x\to+\infty)}.
$$

<h3 id="14a/b">b</h3>

↑ **Parent:** [14A](#14a)

<h4 id="14a/b/solution">Solution</h4>

↑ **Parent:** [B](#14a/b)

Write $T=\tanh(ax)$ and $S=\operatorname{sech}^2(ax)$. Using

$$
T'=aS,
\qquad
S'=-2aST,
$$

two differentiations of

$$
\psi(x)=Ne^{ikx}(aT-ik)
$$

give

$$
-\frac{\hbar^2}{2m}\psi''
-\frac{\hbar^2a^2}{m}S\psi
=\frac{\hbar^2k^2}{2m}\psi.
$$

Thus it solves the time-independent [Schrödinger equation](../../../physics.md#schrodinger-equation) in the stated [Pöschl-Teller potential](../../../quantum-mechanics.md#poschl-teller-potential), with

$$
\boxed{E=\frac{\hbar^2k^2}{2m}}.
$$

As $x\to-\infty$ and $x\to+\infty$, respectively,

$$
\psi(x)\sim N(-a-ik)e^{ikx},
\qquad
\psi(x)\sim N(a-ik)e^{ikx}.
$$

There is no left-moving term, so this is a [reflectionless potential](../../../quantum-mechanics.md#reflectionless-potential):

$$
\boxed{P_{\rm ref}=0}.
$$

The incident and transmitted amplitudes have equal modulus because

$$
|-a-ik|^2=|a-ik|^2=a^2+k^2.
$$

Hence

$$
\boxed{P_{\rm tr}=1}.
$$

Now set $k=i\lambda$ with $\lambda>0$. Then

$$
\psi(x)=Ne^{-\lambda x}\bigl(a\tanh(ax)+\lambda\bigr),
\qquad
E=-\frac{\hbar^2\lambda^2}{2m}.
$$

At $+\infty$ this decays for every positive $\lambda$. At $-\infty$, however, the factor tends to $\lambda-a$ while $e^{-\lambda x}$ grows. Normalizability therefore requires $\lambda=a$. In that case

$$
\psi(x)=Na\,e^{-ax}(1+\tanh ax)
=Na\,\operatorname{sech}(ax),
$$

which decays at both ends. The bound-state energy is

$$
\boxed{E=-\frac{\hbar^2a^2}{2m}}.
$$

## 15D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="15d/a">a</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/a/solution">Solution</h4>

↑ **Parent:** [A](#15d/a)

Translation symmetry in the plane and reflection symmetry across it force the [magnetic field](../../../electromagnetism.md#magnetic-field) to be uniform on each side, parallel to $\mathbf e_y$, and opposite on the two sides. Apply [Ampère's law](../../../electromagnetism.md#ampere-s-circuital-law) to a rectangular loop perpendicular to the sheet whose two long sides have length $L$. The enclosed current is $KL$, so

$$
2BL=\mu_0KL.
$$

The right-hand rule fixes the directions:

$$
\boxed{
\mathbf B(z>0)=-\frac{\mu_0K}{2}\mathbf e_y,
\qquad
\mathbf B(z<0)=\frac{\mu_0K}{2}\mathbf e_y}.
$$

Consequently

$$
\mathbf e_z\times\mathbf B(0^+)
-\mathbf e_z\times\mathbf B(0^-)
=\frac{\mu_0K}{2}\mathbf e_x
-\left(-\frac{\mu_0K}{2}\mathbf e_x\right)
=\boxed{\mu_0\mathbf K},
$$

which is the magnetic jump condition for a [surface current density](../../../electromagnetism.md#surface-current-density).

<h3 id="15d/b">b</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/b/solution">Solution</h4>

↑ **Parent:** [B](#15d/b)

The accumulated [point charge](../../../electromagnetism.md#point-charge) $Q(t)$ produces

$$
\boxed{\mathbf E(r,t)
=\frac{Q(t)}{4\pi\epsilon_0r^2}\mathbf e_r}.
$$

Since $\dot Q=I$, the [displacement current](../../../electromagnetism.md#displacement-current) density is

$$
\boxed{\epsilon_0\frac{\partial\mathbf E}{\partial t}
=\frac{I}{4\pi r^2}\mathbf e_r}.
$$

Apply the integral [Ampère-Maxwell equation](../../../electromagnetism.md#ampere-s-circuital-law) to the boundary of a [spherical cap](../../../geometry-and-topology.md#spherical-cap) of radius $r$ and polar angle $\theta<\pi/2$. By axial symmetry $\mathbf B=B_\phi\mathbf e_\phi$ is constant along the boundary, whose circumference is $2\pi r\sin\theta$. The displacement-current flux through the cap is

$$
\int_{\rm cap}\frac{I}{4\pi r^2}\,dA
=\frac{I}{4\pi r^2}\,2\pi r^2(1-\cos\theta)
=\frac I2(1-\cos\theta).
$$

Thus

$$
2\pi r\sin\theta\,B_\phi
=\frac{\mu_0I}{2}(1-\cos\theta).
$$

Using $(1-\cos\theta)/\sin\theta=\tan(\theta/2)$ gives

$$
\boxed{\mathbf B(r,\theta)
=\frac{\mu_0I}{4\pi r}
\tan\!\left(\frac\theta2\right)\mathbf e_\phi}.
$$

## 16C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="16c/a">a</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/a/solution">Solution</h4>

↑ **Parent:** [A](#16c/a)

Equation (1) is [Laplace equation](../../../partial-differential-equation.md#laplace-equation) for the [velocity potential](../../../fluid-mechanics.md#velocity-potential). It expresses incompressibility, $\nabla\cdot\mathbf u=0$, together with $\mathbf u=\nabla\phi$. Equation (2) is the linearized dynamic free-surface condition: the unsteady [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) and constant atmospheric pressure balance the potential acceleration against the gravitational restoring term $g\zeta$. Equation (3), with the printed $c$ understood as $\zeta$, is the kinematic free-surface condition: the surface moves with the vertical fluid velocity. Equations (4) and (5) are [no-penetration boundary conditions](../../../viscous-fluid-flow.md#no-penetration-boundary-condition) at the rigid bottom and cylindrical sidewall, respectively.

<h3 id="16c/b">b</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/b/solution">Solution</h4>

↑ **Parent:** [B](#16c/b)

For an axisymmetric separated amplitude $\widehat\phi(r,z)=R(r)Z(z)$, [Laplace equation in cylindrical coordinates](../../../partial-differential-equation.md#laplace-equation-in-cylindrical-coordinates) becomes

$$
\frac1R\frac1r(rR')'
=-\frac{Z''}{Z}
=-k^2.
$$

The radial equation is

$$
R''+\frac1rR'+k^2R=0.
$$

Its solution regular at the axis is the [Bessel function](../../../analysis.md#bessel-function) $J_0(kr)$. The vertical equation is $Z''-k^2Z=0$, and the bottom condition $Z'(-h)=0$ selects

$$
\boxed{Z(z)=\cosh(k(z+h))}
$$

up to an irrelevant constant multiplier. Finally, the sidewall condition gives

$$
0=R'(R)=kJ_0'(kR).
$$

Therefore the allowed positive wavenumbers are

$$
\boxed{k_n=\frac{x_n}{R},
\qquad J_0'(x_n)=0},
$$

and

$$
\boxed{\widehat\phi(r,z)
=A J_0(k_nr)\cosh(k_n(z+h))}.
$$

<h3 id="16c/c">c</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/c/solution">Solution</h4>

↑ **Parent:** [C](#16c/c)

At $z=0$, the two free-surface conditions for a [normal mode](../../../wave-equation.md#normal-mode) give

$$
-i\sigma_n\widehat\phi+g\widehat\zeta=0,
\qquad
-i\sigma_n\widehat\zeta-\partial_z\widehat\phi=0.
$$

Eliminating $\widehat\zeta$ yields

$$
\sigma_n^2\widehat\phi
=g\,\partial_z\widehat\phi.
$$

For the vertical factor found in part (b),

$$
\left.\frac{\partial_z\widehat\phi}{\widehat\phi}\right|_{z=0}
=k_n\tanh(k_nh).
$$

Thus the gravity-wave [dispersion relation](../../../wave-equation.md#dispersion-relation) is

$$
\boxed{\sigma_n^2=gk_n\tanh(k_nh)
=\frac gh\,\Psi(k_nh)},
$$

where

$$
\boxed{\Psi(x)=x\tanh x}.
$$

## 17C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="17c/a">a</h3>

↑ **Parent:** [17C](#17c)

<h4 id="17c/a/solution">Solution</h4>

↑ **Parent:** [A](#17c/a)

A one-step or [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) has order $p$ if, when the exact sufficiently smooth solution is substituted for the numerical values, its unscaled [local truncation error](../../../numerical-analysis.md#local-truncation-error) is $O(h^{p+1})$, and this estimate is not generally $O(h^{p+2})$. For a stable method this corresponds to a global error of order $O(h^p)$ on a fixed time interval.

<h3 id="17c/b">b</h3>

↑ **Parent:** [17C](#17c)

<h4 id="17c/b/solution">Solution</h4>

↑ **Parent:** [B](#17c/b)

Expand the exact solution about $t_{n+1}=t$. The left side is

$$
y(t+h)-y(t)
=hy'+\frac{h^2}{2}y''
+\frac{h^3}{6}y'''
+\frac{h^4}{24}y^{(4)}+O(h^5).
$$

Since $f(t,y(t))=y'(t)$, the right side expands as

$$
hy'
+h^2(1+2\alpha+\beta)y''
+\frac{h^3}{2}(1-\beta)y'''
+\frac{h^4}{6}(1+2\alpha+\beta)y^{(4)}
+O(h^5).
$$

The $hy'$ terms agree for every $\alpha,\beta$, so the method is always consistent and is generically of order one.

The method is explicit exactly when $1+\alpha=0$. With $\alpha=-1$, its $h^2$ defect vanishes only for $\beta=3/2$, so a generic explicit member has order one; that exceptional explicit member has order two and cannot satisfy the next order condition.

For the unrestricted method to have order at least three, the $h^2$ and $h^3$ coefficients must agree:

$$
1+2\alpha+\beta=\frac12,
\qquad
\frac{1-\beta}{2}=\frac16.
$$

Solving gives

$$
\boxed{\alpha=-\frac7{12},
\qquad
\beta=\frac23}.
$$

For these values, $1+2\alpha+\beta=1/2$, so the right-side $h^4$ coefficient is $1/12$, different from the left-side coefficient $1/24$. Hence the order is exactly three.

<h3 id="17c/c">c</h3>

↑ **Parent:** [17C](#17c)

<h4 id="17c/c/solution">Solution</h4>

↑ **Parent:** [C](#17c/c)

The first characteristic polynomial of the [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) comes only from its left side:

$$
\rho(\zeta)=\zeta^2-\zeta=\zeta(\zeta-1).
$$

Its roots are zero and one; both lie in the closed unit disc, and the only unit-modulus root is simple. Thus the method satisfies the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) and is [zero-stable](../../../numerical-analysis.md#zero-stability). Part (b) showed consistency for every $\alpha,\beta$. The [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem) states that a consistent linear multistep method is convergent exactly when it is zero-stable. Therefore

$$
\boxed{\text{the method is convergent}}
$$

under the usual Lipschitz hypotheses on $f$.

## 18H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="18h/a">a</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/a/solution">Solution</h4>

↑ **Parent:** [A](#18h/a)

Because $X$ has [full column rank](../../../vector-space.md#full-column-rank), $X^TX$ is invertible. The [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) estimator is

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY}.
$$

It satisfies the [normal equations](../../../statistical-modelling.md#normal-equation)

$$
X^T(Y-X\widehat\beta)=0,
$$

so the residual is orthogonal to the [column space](../../../vector-space.md#column-space) of $X$. For any $\beta$,

$$
Y-X\beta
=(Y-X\widehat\beta)+X(\widehat\beta-\beta).
$$

The two terms are orthogonal, and the [Pythagorean theorem in an inner-product space](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) gives

$$
S(\beta)
=S(\widehat\beta)
+(\beta-\widehat\beta)^TX^TX(\beta-\widehat\beta)
\ge S(\widehat\beta).
$$

**Thus $\widehat\beta$ minimizes the least-squares objective.**

<h3 id="18h/b">b</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/b/solution">Solution</h4>

↑ **Parent:** [B](#18h/b)

Since $\widehat\beta=\beta^0+(X^TX)^{-1}X^T\varepsilon$ and $\operatorname{cov}(\varepsilon)=\sigma^2I_n$,

$$
\boxed{\operatorname{cov}(\widehat\beta)
=\sigma^2(X^TX)^{-1}}.
$$

<h3 id="18h/c">c</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/c/solution">Solution</h4>

↑ **Parent:** [C](#18h/c)

Write $\widetilde\beta=(\widetilde\gamma^T,0)^T$, where

$$
\widetilde\gamma=(Z^TZ)^{-1}Z^TY.
$$

The final coordinate is deterministic, while the first $p-1$ coordinates have the usual least-squares covariance. Hence

$$
\boxed{
\operatorname{cov}(\widetilde\beta)
=\sigma^2
\begin{pmatrix}
(Z^TZ)^{-1}&0\\
0&0
\end{pmatrix}}.
$$

<h3 id="18h/d">d</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/d/solution">Solution</h4>

↑ **Parent:** [D](#18h/d)

Because $\operatorname{col}Z\subseteq\operatorname{col}X$, the two [orthogonal projection matrices](../../../linear-algebra.md#orthogonal-projection-matrix) satisfy

$$
P_0P=PP_0=P_0.
$$

Consequently $P-P_0$ is itself an orthogonal projection, onto the orthogonal complement of $\operatorname{col}Z$ within $\operatorname{col}X$. In particular it is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix), so for every $u\in\mathbb R^n$,

$$
\boxed{u^TPu-u^TP_0u
=u^T(P-P_0)u
=\|(P-P_0)u\|^2\ge0}.
$$

<h3 id="18h/e">e</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/e/solution">Solution</h4>

↑ **Parent:** [E](#18h/e)

Full column rank of $X$ makes $X^T:\mathbb R^n\to\mathbb R^p$ surjective. Given $x\in\mathbb R^p$, choose $u$ with $x=X^Tu$. The fitted values for the unrestricted and restricted regressions are

$$
X\widehat\beta=PY,
\qquad
X\widetilde\beta=P_0Y.
$$

Therefore

$$
x^T\widehat\beta=u^TPY,
\qquad
x^T\widetilde\beta=u^TP_0Y.
$$

Using $\operatorname{cov}(Y)=\sigma^2I_n$ and idempotence of the projections,

$$
\operatorname{var}(x^T\widehat\beta)
=\sigma^2u^TPu,
\qquad
\operatorname{var}(x^T\widetilde\beta)
=\sigma^2u^TP_0u.
$$

Part (d) now gives

$$
\boxed{\operatorname{var}(x^T\widetilde\beta)
\le\operatorname{var}(x^T\widehat\beta)}.
$$

## 19H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="19h/solution">Solution</h3>

↑ **Parent:** [19H](#19h)

The [Lagrangian sufficiency theorem](../../../mathematical-optimization.md#lagrange-sufficiency-theorem) for a maximization problem says the following. Suppose the constraints are $g_i(q)\ge0$ and $h_j(q)=0$, and define

$$
L(q,\lambda,\mu)
=f(q)+\sum_i\lambda_i g_i(q)+\sum_j\mu_jh_j(q),
\qquad \lambda_i\ge0.
$$

If a feasible $q^*$ satisfies [complementary slackness](../../../mathematical-optimization.md#complementary-slackness) $\lambda_i g_i(q^*)=0$ and globally maximizes $L(\,\cdot\,,\lambda,\mu)$, then $q^*$ globally maximizes $f$. Indeed, for every feasible $q$,

$$
f(q)\le L(q,\lambda,\mu)
\le L(q^*,\lambda,\mu)
=f(q^*).
$$

This proves the theorem. In a [concave maximization problem](../../../real-analysis.md#concave-function), stationarity and the boundary optimality conditions ensure the required global maximum of the Lagrangian.

For the problem at hand, retain $x,z\ge0$ as the domain and attach a multiplier $\lambda$ to the equality:

$$
L=x+y+2a\sqrt{1+z}
+\lambda\left(b-x-\frac12y^2-z\right).
$$

For $\lambda\ge1$, this is concave in $(x,y,z)$ on the domain. Its separate maximizers satisfy

$$
y=\frac1\lambda,
\qquad
z=\max\left(\frac{a^2}{\lambda^2}-1,0\right),
$$

while the $x$ term is $(1-\lambda)x$. Thus $x$ may be positive only when $\lambda=1$; when $\lambda>1$, its maximizing value is $x=0$.

If

$$
b\ge a^2-\frac12,
$$

take $\lambda=1$. Then $y=1$, $z=a^2-1$, and feasibility fixes

$$
x=b-a^2+\frac12\ge0.
$$

The Lagrangian sufficiency theorem gives the maximum

$$
\boxed{(x,y,z)=
\left(b-a^2+\frac12,\,1,\,a^2-1\right)},
$$



$$
\boxed{f_{\max}=b+a^2+\frac32}.
$$

If

$$
\frac12\le b<a^2-\frac12,
$$

then $\lambda>1$ and $x=0$. The equality constraint becomes

$$
\frac1{2\lambda^2}
+\frac{a^2}{\lambda^2}-1=b,
$$

so

$$
\lambda^2=\frac{a^2+1/2}{b+1}.
$$

Consequently

$$
\boxed{x=0,\qquad
y=\sqrt{\frac{2(b+1)}{2a^2+1}},
\qquad
z=\frac{2a^2b-1}{2a^2+1}}.
$$

The assumptions $a\ge1$ and $b\ge1/2$ ensure $z\ge0$. At the stationary point $\sqrt{1+z}=ay$, so the maximum value is

$$
\boxed{f_{\max}
=(1+2a^2)y
=\sqrt{2(b+1)(2a^2+1)}}.
$$

The two formulas agree at $b=a^2-1/2$.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2020](../../2020.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
