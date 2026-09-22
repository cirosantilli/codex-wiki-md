# Paper 126

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20126.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20126.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [i](#2/i)
    - [a](#2/i/a)
      - [Solution](#2/i/a/solution)
    - [b](#2/i/b)
      - [Solution](#2/i/b/solution)
  - [ii](#2/ii)
    - [a](#2/ii/a)
      - [Solution](#2/ii/a/solution)
    - [b](#2/ii/b)
      - [Solution](#2/ii/b/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)

## 1

↑ **Parent:** [Paper 126](paper-126.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For $A\to B\to C=B/I$, define

$$
\alpha:I/I^2\to\Omega_{B/A}\otimes_BC,
\qquad [i]\mapsto di\otimes1,
$$

and

$$
\beta:\Omega_{B/A}\otimes_BC\to\Omega_{C/A},
\qquad db\otimes c\mapsto c\,d\bar b.
$$

The first map is well-defined because $d(ij)=i\,dj+j\,di$ becomes zero after tensoring with $C$ when $i,j\in I$. The second is induced by the universal derivation $B\to C\xrightarrow d\Omega_{C/A}$ and is surjective because the elements $d\bar b$ generate $\Omega_{C/A}$.

The composite is zero since $\bar i=0$. Conversely, quotienting $\Omega_{B/A}\otimes_BC$ by the $di$ for $i\in I$ imposes exactly the relations needed for the derivation of $B$ to descend to $C$. The universal property of the [module of Kähler differentials](../../../ringed-space.md#kahler-differential) therefore identifies that quotient with $\Omega_{C/A}$, proving the [Conormal exact sequence for Kähler differentials](../../../ringed-space.md#conormal-exact-sequence-for-kahler-differentials)

$$
\boxed{I/I^2\xrightarrow\alpha\Omega_{B/A}\otimes_BC\xrightarrow\beta\Omega_{C/A}\to0.}
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Every $k$-derivation $D:K[t]\to M$ is uniquely determined by its restriction to $K$ and by $D(t)$. Conversely, a $k$-derivation $K\to M$ and an arbitrary element $m\in M$ extend uniquely by

$$
D\left(\sum_i a_it^i\right)=\sum_iD(a_i)t^i+\sum_iia_it^{i-1}m.
$$

Representing this natural decomposition of derivations gives

$$
\boxed{\Omega_{K[t]/k}\cong(\Omega_{K/k}\otimes_KK[t])\oplus K[t],dt.}
$$

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Present $L=K[t]/(f)$ by sending $t$ to $b$. Applying the [Conormal exact sequence for Kähler differentials](../../../ringed-space.md#conormal-exact-sequence-for-kahler-differentials) and part ii gives

$$
L\cong(f)/(f^2)\longrightarrow
(\Omega_{K/k}\otimes_KL)\oplus L,dt
\longrightarrow\Omega_{L/k}\longrightarrow0.
$$

Writing $f(t)=\sum_i a_it^i$, the image of $1$, represented by $f$, is

$$
df=\left(\sum_i b^i,da_i, f'(b),dt\right).
$$

This has the required form $( *,f'(b)dt)$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

If $L/K$ is finite separable, the [primitive element theorem](../../../galois-theory.md#primitive-element-theorem) writes it as $K(b)$ with $f'(b)\ne0$. The relation in part a has a nonzero $dt$ component, so projection along that relation gives an isomorphism

$$
\Omega_{K/k}\otimes_KL\xrightarrow{\sim}\Omega_{L/k}.
$$

For an arbitrary simple finite extension, part a presents $\Omega_{L/k}$ as a quotient of a vector space of dimension $\dim_K\Omega_{K/k}+1$ by the image of a space of dimension at most one. Its dimension is therefore at least $\dim_K\Omega_{K/k}$. Applying this one generator at a time through a finite tower proves the same inequality for every finite extension.

Strict inequality occurs in characteristic $p$. Take $k=K=\mathbb F_p(u)$ and $L=K(u^{1/p})$. Then $\Omega_{K/k}=0$, while the relation $b^p-u=0$ has zero differential relative to $k$, so

$$
\Omega_{L/k}=L,db
$$

has dimension one.

## 2

↑ **Parent:** [Paper 126](paper-126.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/a">a</h4>

↑ **Parent:** [I](#2/i)

<h5 id="2/i/a/solution">Solution</h5>

↑ **Parent:** [A](#2/i/a)

The relevant theorem supplies, locally on $S=\operatorname{Spec}A$, a bounded complex $K^\bullet$ of finite free $A$-modules such that

$$
H^p(X,\mathcal F\otimes_AM)\cong H^p(K^\bullet\otimes_AM)
$$

naturally for every $A$-module $M$. In particular the fiber cohomology at $s$ is computed by $K^\bullet\otimes_A\kappa(s)$.

The Euler characteristic of a finite-dimensional complex equals the alternating sum of the dimensions of its terms. Hence

$$
\chi(X_s,\mathcal F_s)=\sum_i(-1)^i\operatorname{rank}K^i,
$$

which is constant wherever one complex works. It is therefore locally constant on $S$, and is constant when $S$ is connected.

<h4 id="2/i/b">b</h4>

↑ **Parent:** [I](#2/i)

<h5 id="2/i/b/solution">Solution</h5>

↑ **Parent:** [B](#2/i/b)

Use the same [finite complex computing cohomology in a proper flat family](../../../ringed-space.md#finite-complex-computing-cohomology-in-a-proper-flat-family). In fixed bases its differentials are matrices over $A$. The condition that such a matrix have rank at most $r$ is closed, being defined by its $(r+1)\times(r+1)$ minors. Since

$$
\dim H^p(K^\bullet\otimes\kappa(s))
=\dim K^p-\operatorname{rank}d^{p-1}_s-\operatorname{rank}d^p_s,
$$

the condition that this dimension be at least $n$ is a finite union of intersections of closed rank loci. It is therefore closed. This is the [semicontinuity theorem for coherent cohomology](../../../ringed-space.md#semicontinuity-theorem-for-coherent-cohomology).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/a">a</h4>

↑ **Parent:** [Ii](#2/ii)

<h5 id="2/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#2/ii/a)

For every integer $t$,

$$
P(\mathbb P_k^2,\mathcal O,t)=\chi(\mathbb P_k^2,\mathcal O(t))
=\binom{t+2}{2}
=\frac{t^2+3t+2}{2}.
$$

For $t\geq0$ this is the dimension of the homogeneous polynomials of degree $t$, since the higher cohomology vanishes; polynomiality then identifies the [Hilbert polynomial](../../../algebraic-geometry.md#hilbert-polynomial).

<h4 id="2/ii/b">b</h4>

↑ **Parent:** [Ii](#2/ii)

<h5 id="2/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#2/ii/b)

A smooth plane curve of degree $m$ has genus

$$
g=\frac{(m-1)(m-2)}2.
$$

The line bundle $\mathcal O_X(D)(t)$ has degree $d+mt$. The [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) therefore gives

$$
\boxed{P(X,\mathcal O_X(D),t)
=\chi(\mathcal O_X(D)(t))
=mt+d+1-g
=mt+d+1-\frac{(m-1)(m-2)}2.}
$$

## 3

↑ **Parent:** [Paper 126](paper-126.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

A useful form of the [Mumford rigidity lemma](../../../abelian-variety.md#mumford-rigidity-lemma) says that if $X$ is complete and connected and $h:X\times Y\to Z$ is constant on one fiber $X\times\{y_0\}$, then under the pointed separated hypotheses it factors through $Y$.

For $f:X\to G$ with $f(e_X)=e_G$, define

$$
h(x,y)=f(x+y)f(y)^{-1}.
$$

At $x=e_X$ this is constantly $e_G$. Applying rigidity with the complete factor $X$ in the $y$ variable shows that $h(x,y)$ is independent of $y$. At $y=e_X$ its value is $f(x)$, so

$$
f(x+y)=f(x)f(y).
$$

Thus $f$ is a homomorphism of [group varieties](../../../algebraic-geometry.md#algebraic-group).

Completeness is essential. On the additive group variety $\mathbb G_a$ over a field of characteristic different from two, the morphism $f(t)=t^2$ fixes zero but is not additive.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For $x:S\to G$, define

$$
T_x:G\times_kS\to G,
\qquad(g,s)\mapsto x(s)g.
$$

Then $T_{x/S}=(T_x,\operatorname{pr}_2)$ is an $S$-morphism, and translation by $x^{-1}$ is its inverse.

Because an isomorphism preserves relative differentials and $T_{x/S}$ lies over $S$,

$$
T_{x/S}^*\Omega_{G\times S/S}\cong\Omega_{G\times S/S}.
$$

Using base change, $\Omega_{G\times S/S}\cong\operatorname{pr}_1^*\Omega_{G/k}$, while the left side is $T_x^*\Omega_{G/k}$. Pulling this isomorphism back along the identity section $e\times1_S$ gives

$$
x^*\Omega_{G/k}\cong\mathcal O_S\otimes_k\Omega_{G/k}(e).
$$

Finally take $S=G$ and $x=1_G$. This yields the [invariant differential on a group scheme](../../../abelian-variety.md#invariant-differential-on-a-group-scheme) trivialization

$$
\Omega_{G/k}\cong\mathcal O_G\otimes_k\Omega_{G/k}(e),
$$

so $\Omega_{G/k}$ is a free $\mathcal O_G$-module.

## 4

↑ **Parent:** [Paper 126](paper-126.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The [Theorem of the square](../../../abelian-variety.md#theorem-of-the-square) states that for a line bundle $L$ on an [abelian variety](../../../abelian-variety.md) $X$ and $x,y\in X(k)$,

$$
\boxed{T_{x+y}^*L\otimes L\cong T_x^*L\otimes T_y^*L.}
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Define the [homomorphism associated to a line bundle on an abelian variety](../../../abelian-variety.md#homomorphism-associated-to-a-line-bundle-on-an-abelian-variety)

$$
\phi_L:X(k)\to\operatorname{Pic}X,
\qquad \phi_L(x)=T_x^*L\otimes L^{-1}.
$$

The [Theorem of the square](../../../abelian-variety.md#theorem-of-the-square) gives $\phi_L(x+y)=\phi_L(x)\otimes\phi_L(y)$, so this is a homomorphism.

Tensor products satisfy $\phi_{L\otimes M}=\phi_L\otimes\phi_M$ and $\phi_{L^{-1}}=\phi_L^{-1}$. Therefore

$$
\operatorname{Pic}^0X=\{L:\phi_L=0\}
$$

is a subgroup of the [Picard group](../../../ringed-space.md#picard-group). If $M=\phi_L(x)$, translations commute and the theorem of the square gives

$$
T_y^*M\otimes M^{-1}\cong\mathcal O_X
$$

for every $y$. Hence $M\in\operatorname{Pic}^0X$, proving $\operatorname{im}\phi_L\subseteq\operatorname{Pic}^0X$.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

The map

$$
\tau(L_1,L_2)=\operatorname{pr}_1^*L_1\otimes\operatorname{pr}_2^*L_2
$$

is a homomorphism. Pullback along $i_1(x)=(x,e_2)$ recovers $L_1$, up to tensoring with a fixed one-dimensional vector space, which is a trivial line bundle; similarly $i_2^*$ recovers $L_2$. Thus $\tau$ is injective.

It need not be surjective. For an elliptic curve $E$, the line bundle $\mathcal O_{E\times E}(\Delta)$ of the diagonal restricts to $E\times\{y\}$ as $\mathcal O_E(y)$, whose class varies with $y$. A line bundle pulled back separately from the two factors has constant class on these fibers. Hence $\mathcal O(\Delta)$ is not in the image of $\tau$.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

Part iii already proves injectivity. Pullback along $i_j$ sends translation-invariant line bundles to translation-invariant line bundles, so it defines

$$
\rho:\operatorname{Pic}^0(X_1\times X_2)\to
\operatorname{Pic}^0X_1\times\operatorname{Pic}^0X_2.
$$

Clearly $\rho\tau=1$.

For $L\in\operatorname{Pic}^0(X_1\times X_2)$, put $L_j=i_j^*L$ and

$$
M=L\otimes\operatorname{pr}_1^*L_1^{-1}\otimes\operatorname{pr}_2^*L_2^{-1}.
$$

Then $M$ is trivial on both coordinate axes. Since $L$ and the two correcting factors lie in [$\operatorname{Pic}^0$](../../../abelian-variety.md#identity-component-of-the-picard-group), translation by $(x_1,e_2)$ leaves $M$ invariant. Hence every restriction $M|_{\{x_1\}\times X_2}$ is trivial. The [Seesaw theorem](../../../abelian-variety.md#seesaw-theorem) and triviality on $X_1\times\{e_2\}$ imply $M\cong\mathcal O_X$. Thus $L=\tau(L_1,L_2)$, so

$$
\boxed{\operatorname{Pic}^0X_1\times\operatorname{Pic}^0X_2
\xrightarrow{\sim}\operatorname{Pic}^0(X_1\times X_2).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
