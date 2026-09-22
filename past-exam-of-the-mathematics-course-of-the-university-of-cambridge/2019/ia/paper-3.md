# Paper 3

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2019/paperia_3_2019.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2019/paperia_3_2019.pdf)

**Table of contents**

- [1D](#1d)
  - [Solution](#1d/solution)
- [2D](#2d)
  - [Solution](#2d/solution)
- [3B](#3b)
  - [Solution](#3b/solution)
- [4B](#4b)
  - [Solution](#4b/solution)
- [5D](#5d)
  - [i](#5d/i)
    - [Solution](#5d/i/solution)
  - [ii](#5d/ii)
    - [Solution](#5d/ii/solution)
- [6D](#6d)
  - [a](#6d/a)
    - [Solution](#6d/a/solution)
  - [b](#6d/b)
    - [Solution](#6d/b/solution)
  - [c](#6d/c)
    - [Solution](#6d/c/solution)
  - [d](#6d/d)
    - [Solution](#6d/d/solution)
- [7D](#7d)
  - [Solution](#7d/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
- [9B](#9b)
  - [Solution](#9b/solution)
- [10B](#10b)
  - [a](#10b/a)
    - [Solution](#10b/a/solution)
  - [b](#10b/b)
    - [Solution](#10b/b/solution)
- [11B](#11b)
  - [Solution](#11b/solution)
- [12B](#12b)
  - [a](#12b/a)
    - [Solution](#12b/a/solution)
  - [b](#12b/b)
    - [Solution](#12b/b/solution)

## 1D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1d/solution">Solution</h3>

↑ **Parent:** [1D](#1d)

Conjugating a [cycle](../../../finite-group-theory.md#permutation-cycle) merely relabels its entries:

$$
g(a_1\ a_2\ \cdots\ a_k)g^{-1}
=(g(a_1)\ g(a_2)\ \cdots\ g(a_k)).
$$

Thus conjugate [permutations](../../../combinatorics.md#permutation) have the same [cycle type](../../../finite-group-theory.md#cycle-type). Conversely, if $\sigma$ and $\tau$ have the same cycle type, match the entries of each cycle of $\sigma$ bijectively and in cyclic order with those of a cycle of $\tau$ of the same length. Extending these matches to a permutation $g$ gives $g\sigma g^{-1}=\tau$.

Let $C_{S_n}(\sigma)$ be the [centralizer](../../../group-theory.md#centralizer) of $\sigma$. Its $S_n$-conjugacy class remains one $A_n$-conjugacy class exactly when $C_{S_n}(\sigma)$ contains an [odd permutation](../../../finite-group-theory.md#odd-permutation). Indeed, in that case $C_{A_n}(\sigma)$ has index two in $C_{S_n}(\sigma)$, so the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) gives

$$
|\operatorname{Cl}_{A_n}(\sigma)|
=\frac{|A_n|}{|C_{A_n}(\sigma)|}
=\frac{|S_n|}{|C_{S_n}(\sigma)|}
=|\operatorname{Cl}_{S_n}(\sigma)|.
$$

If the centralizer contains only even permutations, the $A_n$ class has half the size and the $S_n$ class splits into two $A_n$ classes.

The even cycle types in $S_5$ are

$$
1^5,\qquad 3\,1^2,\qquad 2^2 1,\qquad 5.
$$

The classes of the identity, a three-cycle, and a double transposition do not split: their centralizers contain an odd permutation. The centralizer of a five-cycle is its cyclic subgroup of order five, which lies in $A_5$, so that class splits in two. Therefore

$$
\boxed{A_5\text{ has }1+1+1+2=5\text{ conjugacy classes}}.
$$

## 2D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2d/solution">Solution</h3>

↑ **Parent:** [2D](#2d)

The [orthogonal group](../../../linear-algebra.md#orthogonal-group) is

$$
O(n)=\{Q\in M_n(\mathbb R):Q^TQ=I\}.
$$

The [special orthogonal group](../../../linear-algebra.md#special-orthogonal-group) is its determinant-one subgroup

$$
SO(n)=\{Q\in O(n):\det Q=1\}.
$$

Every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) has [modulus](../../../complex-analysis.md#modulus) one. A real three-by-three matrix has at least one real eigenvalue, and nonreal eigenvalues occur in a [complex conjugate](../../../complex-analysis.md#complex-conjugate) pair. If $Q\in SO(3)$ has such a pair $e^{\pm i\theta}$, their product is one, so the remaining eigenvalue is $\det Q=1$. If all three eigenvalues are real, each is $\pm1$ and their product is one; an odd number of three signs with product one must include $+1$. Hence every element of $SO(3)$ has an eigenvector of eigenvalue one and represents a [rotation in three dimensions](../../../linear-algebra.md#rotation-in-three-dimensions) about its span.

**It is false** that every element of $O(3)$ is either a rotation or a plane reflection. For example,

$$
Q=\begin{pmatrix}
\cos\theta&-\sin\theta&0\\
\sin\theta&\cos\theta&0\\
0&0&-1
\end{pmatrix},
\qquad 0<\theta<\pi,
$$

is an [improper orthogonal transformation](../../../linear-algebra.md#improper-orthogonal-transformation) combining a rotation with a reflection. Its eigenvalues are $e^{\pm i\theta}$ and $-1$, whereas a plane reflection has eigenvalues $1,1,-1$ and a rotation has determinant one.

## 3B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3b/solution">Solution</h3>

↑ **Parent:** [3B](#3b)

For an arbitrary constant vector $\mathbf c$, the [product rule for divergence](../../../calculus.md#product-rule-for-divergence) gives

$$
\nabla\mathbin{\cdot}(\phi\mathbf c)=\mathbf c\mathbin{\cdot}\nabla\phi.
$$

The [divergence theorem](../../../calculus.md#divergence-theorem) therefore implies

$$
\mathbf c\mathbin{\cdot}\int_V\nabla\phi\,dV
=\int_V\nabla\mathbin{\cdot}(\phi\mathbf c)\,dV
=\int_S\phi\,\mathbf c\mathbin{\cdot}d\mathbf S
=\mathbf c\mathbin{\cdot}\int_S\phi\,d\mathbf S.
$$

Since this holds for every $\mathbf c$,

$$
\boxed{\int_V\nabla\phi\,dV=\int_S\phi\,d\mathbf S}.
$$

For $\phi=x+y$, $\nabla\phi=(1,1,0)$. The ball of radius $a$ has volume $4\pi a^3/3$, so

$$
\int_V\nabla\phi\,dV=\frac{4\pi a^3}{3}(1,1,0).
$$

On the sphere, use $x=a\sin\theta\cos\varphi$, $y=a\sin\theta\sin\varphi$ and the stated outward [oriented surface element](../../../calculus.md#oriented-surface-element). The first component of the surface integral is

$$
a^3\int_0^\pi\sin^3\theta\,d\theta
\int_0^{2\pi}(\cos^2\varphi+\sin\varphi\cos\varphi)\,d\varphi
=a^3\frac43\pi,
$$

and symmetry gives the same second component and a zero third component. The two sides agree.

## 4B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4b/solution">Solution</h3>

↑ **Parent:** [4B](#4b)

On the simply connected domain $\mathbb R^3$, a continuously differentiable [differential one-form](../../../differential-form.md#one-form) is [exact](../../../differential-form.md#exact-differential) if its mixed partial derivatives agree, equivalently if its associated vector field has zero [curl](../../../calculus.md#curl). Here one can verify exactness directly by observing that

$$
F(x,y,z)=(x^2+z^2)e^{(x+y)z}
$$

satisfies

$$
\frac{\partial F}{\partial x}=u,
\qquad
\frac{\partial F}{\partial y}=v,
\qquad
\frac{\partial F}{\partial z}=w.
$$

Thus $u\,dx+v\,dy+w\,dz=dF$. By the [fundamental theorem for line integrals](../../../calculus.md#fundamental-theorem-for-line-integrals), its integral is [path independent](../../../calculus.md#path-independence) and equals

$$
F(1,0,1)-F(-1,0,1)=2e-2e^{-1}.
$$

Consequently, for every path with the stated endpoints,

$$
\boxed{\int_{(-1,0,1)}^{(1,0,1)}(u\,dx+v\,dy+w\,dz)=4\sinh1}.
$$

## 5D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5d/i">i</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/i/solution">Solution</h4>

↑ **Parent:** [I](#5d/i)

Suppose first that $H$ and $K$ are [normal subgroups](../../../group-theory.md#normal-subgroup). For $h\in H$ and $k\in K$, the [commutator](../../../lie-algebra.md#commutator)

$$
[h,k]=hkh^{-1}k^{-1}
$$

lies in $H$, because $kh^{-1}k^{-1}\in H$, and in $K$, because $hkh^{-1}\in K$. Since $H\cap K=\{e\}$, $[h,k]=e$, so $h$ and $k$ commute.

Conversely, suppose every element of $H$ commutes with every element of $K$. Write an arbitrary $g\in G$ as $g=h_0k_0$. For $h\in H$,

$$
ghg^{-1}=h_0k_0hk_0^{-1}h_0^{-1}=h_0hh_0^{-1}\in H,
$$

so $H\trianglelefteq G$. The symmetric calculation proves $K\trianglelefteq G$.

<h3 id="5d/ii">ii</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5d/ii)

[Cauchy's theorem for finite groups](../../../finite-group-theory.md#cauchy-theorem-for-groups) states that if a [prime number](../../../number-theory.md#prime-number) $p$ divides the order of a finite group $G$, then $G$ contains an element of order $p$.

Consider

$$
X=\{(x_1,\ldots,x_p)\in G^p:x_1x_2\cdots x_p=e\}.
$$

The first $p-1$ entries determine the last, so $|X|=|G|^{p-1}$ is divisible by $p$. The [cyclic group](../../../group.md#cyclic-group) $C_p$ acts on $X$ by cyclically shifting the coordinates; the shifted tuple remains in $X$ because $x_2\cdots x_px_1=x_1^{-1}(x_1\cdots x_p)x_1=e$. Every [orbit](../../../dynamical-systems.md#orbit-dynamical-system) has size one or $p$. The fixed points are exactly $(x,\ldots,x)$ with $x^p=e$. Their number is therefore divisible by $p$. Since the identity is one fixed point, another exists; its order is $p$.

Now let the [abelian group](../../../group.md#abelian-group) $G$ have order $pq$ for distinct primes $p,q$. Cauchy's theorem supplies $x,y$ of orders $p,q$. Their cyclic subgroups intersect trivially, and commutativity shows that $xy$ has order $pq$. Thus $G$ is cyclic and

$$
\boxed{G\cong C_{pq}\cong C_p\times C_q}.
$$

The corresponding assertion for order $p^2$ is false: $C_{p^2}$ is not isomorphic to $C_p\times C_p$, since the former has an element of order $p^2$ while every nonidentity element of the latter has order $p$.

## 6D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6d/a">a</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/a/solution">Solution</h4>

↑ **Parent:** [A](#6d/a)

[Lagrange's theorem for finite groups](../../../group-theory.md#lagrange-s-theorem) states that if $H\leq G$ and $G$ is finite, then

$$
|G|=[G:H]|H|,
$$

so $|H|$ divides $|G|$. Indeed, the left [cosets](../../../group-theory.md#coset) of $H$ partition $G$, and multiplication by a coset representative is a bijection from $H$ to each coset.

Applying the theorem to the [cyclic subgroup](../../../group.md#cyclic-subgroup) $\langle g\rangle$ gives

$$
\operatorname{ord}(g)=|\langle g\rangle|\mid |G|.
$$

In $C_3\times C_9$, an element has order dividing three exactly when its first coordinate is arbitrary and its second belongs to the unique subgroup of order three. There are $3\cdot3=9$ such elements, and after removing the identity the answer is $\boxed8$.

<h3 id="6d/b">b</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/b/solution">Solution</h4>

↑ **Parent:** [B](#6d/b)

Write the [dihedral group](../../../finite-group-theory.md#dihedral-group) as $D_{2n}=\langle r,s:r^n=s^2=e,\ srs=r^{-1}\rangle$. Every reflection has order two, so an element of order three must be a rotation. Such rotations exist exactly when $3\mid n$, and then they are $r^{n/3}$ and $r^{2n/3}$. The answer is therefore

$$
\boxed{2\text{ if }3\mid n,\quad 0\text{ otherwise}}.
$$

<h3 id="6d/c">c</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/c/solution">Solution</h4>

↑ **Parent:** [C](#6d/c)

An element of order three in $S_7$ has [cycle type](../../../finite-group-theory.md#cycle-type) $3\,1^4$ or $3^2 1$. There are

$$
\binom73(3-1)!=35\cdot2=70
$$

single three-cycles. For two disjoint three-cycles, choose the two unordered three-element supports and an orientation on each:

$$
\frac12\binom73\binom43(2)(2)=280.
$$

Hence $S_7$ contains $\boxed{350}$ elements of order three.

<h3 id="6d/d">d</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/d/solution">Solution</h4>

↑ **Parent:** [D](#6d/d)

A three-cycle is an [even permutation](../../../finite-group-theory.md#even-permutation), as is a product of two disjoint three-cycles. Thus every element counted in part (c) lies in $A_7$, and every order-three element of $A_7$ was already counted there. The answer remains $\boxed{350}$.

## 7D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7d/solution">Solution</h3>

↑ **Parent:** [7D](#7d)

The [first isomorphism theorem for groups](../../../group-theory.md#first-isomorphism-theorem) states that for a [group homomorphism](../../../group-theory.md#group-homomorphism) $f:G\to Q$,

$$
G/\ker f\cong\operatorname{im}f.
$$

The map $g\ker f\mapsto f(g)$ is well defined because two representatives differ by an element of the kernel; it is a surjective homomorphism onto the image and is injective because $f(g)=e$ exactly when $g\in\ker f$.

For $n_i\in N$ and $h_i\in H$, normality of $N$ gives

$$
(n_1h_1)(n_2h_2)=n_1(h_1n_2h_1^{-1})h_1h_2\in NH,
$$

and $(nh)^{-1}=h^{-1}n^{-1}h\,h^{-1}\in NH$. Hence $NH$ is a subgroup. Also $N\cap H\trianglelefteq H$, since conjugation by $H$ preserves both $N$ and $H$, and $N\trianglelefteq NH$ because $NH\leq G$.

Apply the first isomorphism theorem to $f:H\to NH/N$, $f(h)=hN$. Its kernel is $N\cap H$, and it is surjective because $nhN=hN$. Therefore

$$
\boxed{H/(N\cap H)\cong NH/N}.
$$

If $K,H\trianglelefteq G$, then $KH$ is a normal subgroup: it is a subgroup by the calculation above, and $g(KH)g^{-1}=(gKg^{-1})(gHg^{-1})=KH$. Without normality a product need not be a subgroup. In $S_3$, take $H=\langle(12)\rangle$ and $K=\langle(23)\rangle$. The set $KH$ has four elements, so it cannot be a subgroup of the six-element group by [Lagrange's theorem for finite groups](../../../group-theory.md#lagrange-s-theorem).

## 8D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

Represent a [Möbius transformation](../../../group-theory.md#mobius-transformation) by a matrix, with nonzero scalar multiples representing the same map. Matrix multiplication reproduces composition, so $\theta$ is a [group homomorphism](../../../group-theory.md#group-homomorphism). Every Möbius map has a representing matrix $A\in GL_2(\mathbb C)$; multiplying $A$ by either square root of $(\det A)^{-1}$ gives a matrix in $SL_2(\mathbb C)$ representing the same map. Thus $\theta$ is surjective. A matrix in its kernel represents the identity and is therefore scalar; determinant one leaves

$$
\boxed{\ker\theta=\{I,-I\}}.
$$

If a nonidentity Möbius map $T$ has two distinct fixed points, conjugate those points to $0$ and $\infty$. The conjugated map fixes both and hence has the form $S(z)=\mu z$ with $\mu\ne0,1$. If $T$ has one fixed point, conjugate it to $\infty$. The resulting affine map has the form $az+b$; having no finite fixed point forces $a=1$ and $b\ne0$, and conjugating by a scaling makes it $S(z)=z+1$.

Directly, the finite fixed points satisfy

$$
cz^2+(d-a)z-b=0.
$$

Including $\infty$ when appropriate, a nonidentity Möbius map consequently has one or two distinct fixed points.

Finally suppose $T$ has the unique fixed point $z_0$. With the conjugacy $R$ above,

$$
RTR^{-1}(z)=z+1,
\qquad
(RTR^{-1})^n(z)=z+n.
$$

Every finite point tends to $\infty$ on the [Riemann sphere](../../../complex-analysis.md#riemann-sphere), while $\infty$ itself is fixed. Applying the continuous map $R^{-1}$ shows that

$$
\boxed{T^n(z)\longrightarrow z_0}
$$

for every $z\in\mathbb C\cup\{\infty\}$.

## 9B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9b/solution">Solution</h3>

↑ **Parent:** [9B](#9b)

For the one-to-one transformation $(u,v,w)\mapsto(x,y,z)$, the [Jacobian determinant](../../../calculus.md#jacobian-determinant) used in the stated formula is

$$
J=\det\frac{\partial(x,y,z)}{\partial(u,v,w)}.
$$

Locally, the derivative maps a small rectangular box of volume $du\,dv\,dw$ to a parallelepiped of volume $|J|\,du\,dv\,dw$. Partitioning the region into such boxes and passing to the [Riemann integral](../../../real-analysis.md#riemann-integral) gives the [change of variables formula](../../../calculus.md#change-of-variables-formula)

$$
\int_Df(x,y,z)\,dx\,dy\,dz
=\int_\Delta |J|f(x(u,v,w),y(u,v,w),z(u,v,w))\,du\,dv\,dw.
$$

In the plane $y=0$, the region is inside the unit circle and on the right-hand side of the hyperbola

$$
x^2+z^2\leq1,
\qquad
\frac{x^2}{\alpha^2}-\frac{z^2}{\alpha^2\gamma^2}\geq1.
$$

It is nonempty exactly when $\alpha\leq1$; it has positive area when $\alpha<1$. In $x>0$, its boundaries are $x=\sqrt{1-z^2}$ and $x=\alpha\sqrt{1+z^2/\gamma^2}$. The minimum and maximum $x$ values are $\alpha$ and $1$, both at $z=0$. The largest absolute $z$ occurs where the boundaries meet:

$$
z_0=\gamma\sqrt{\frac{1-\alpha^2}{1+\gamma^2}},
\qquad
x_0=\sqrt{\frac{1+\alpha^2\gamma^2}{1+\gamma^2}}.
$$

<a id="9b/image-cross-section-of-the-integration-region"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-3-region-cross-section.png)

**[Figure 1](#9b/image-cross-section-of-the-integration-region). Cross-section of the integration region**.

Now set $u=x$, $v=y/k$, and $w=z$. The inverse [Jacobian determinant](../../../calculus.md#jacobian-determinant) is $k$, and in cylindrical coordinates $r^2=u^2+v^2$ the transformed region is

$$
r^2+w^2\leq1,
\qquad
r^2\geq\alpha^2+\frac{w^2}{\gamma^2}.
$$

Thus $|w|\leq z_0$, and each horizontal cross-section is an annulus. Its volume is

$$
\begin{aligned}
\operatorname{Vol}(D)
&=k\pi\int_{-z_0}^{z_0}
\left[1-w^2-\alpha^2-\frac{w^2}{\gamma^2}\right]dw\\
&=\frac{4\pi k}{3}(1-\alpha^2)z_0.
\end{aligned}
$$

Therefore, for $\alpha<1$,

$$
\boxed{\operatorname{Vol}(D)=
\frac{4\pi k\gamma}{3\sqrt{1+\gamma^2}}(1-\alpha^2)^{3/2}}.
$$

For $\alpha=1$ the region has zero volume.

## 10B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10b/a">a</h3>

↑ **Parent:** [10B](#10b)

<h4 id="10b/a/solution">Solution</h4>

↑ **Parent:** [A](#10b/a)

Under an orthogonal change of coordinates represented by $Q$, the component matrix changes by

$$
T'=QTQ^T=QTQ^{-1}.
$$

Thus $T'$ is [similar](../../../linear-algebra.md#matrix-similarity) to $T$, so its [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial), [eigenvalues](../../../linear-operator-theory.md#eigenvalue), and their [algebraic multiplicities](../../../linear-operator-theory.md#algebraic-multiplicity) are unchanged.

If $T$ is [symmetric](../../../linear-algebra.md#symmetric-matrix), the [spectral theorem for real symmetric matrices](../../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) makes it [diagonalizable](../../../linear-operator-theory.md#diagonalizable-matrix), so algebraic and geometric multiplicities agree. Consequently the dimensions of its eigenspaces are also independent of the coordinate frame.

For the stated tensor, choose a unit eigenvector $n$ belonging to the simple eigenvalue $\mu$. Its perpendicular plane is the eigenspace of $\lambda$, so

$$
T=\lambda(I-nn^T)+\mu nn^T
=\lambda I+(\mu-\lambda)nn^T.
$$

Hence

$$
\boxed{T_{ij}=\alpha\delta_{ij}+\beta n_in_j},
\qquad
\alpha=\lambda,\quad\beta=\mu-\lambda.
$$

<h3 id="10b/b">b</h3>

↑ **Parent:** [10B](#10b)

<h4 id="10b/b/solution">Solution</h4>

↑ **Parent:** [B](#10b/b)

The unit sphere and the kernel $e^{-c|y-x|^2}$ are invariant under every [rotation in three dimensions](../../../linear-algebra.md#rotation-in-three-dimensions) fixing $y$. Therefore $T(y)$ has the same [axisymmetry](../../../calculus.md#axisymmetric-vector-field), so part (a) gives

$$
T_{ij}=\alpha\delta_{ij}+\beta y_iy_j.
$$

Choose [spherical polar coordinates](../../../calculus.md#spherical-coordinate-system) with polar axis $y$ and put $u=\cos\theta=x\mathbin\cdot y$. Since $|x|=|y|=1$,

$$
|y-x|^2=2(1-u),
\qquad dA=2\pi\,du.
$$

The [tensor contraction](../../../linear-algebra.md#tensor-contraction) giving the trace is

$$
T_{kk}=\int_S|x|^2e^{-c|y-x|^2}\,dA
=2\pi\int_{-1}^1e^{-2c(1-u)}du
=\boxed{\frac{\pi}{c}(1-e^{-4c})}.
$$

Similarly,

$$
T_{ij}y_iy_j
=2\pi\int_{-1}^1u^2e^{-2c(1-u)}du
=\boxed{\frac{\pi e^{-2c}}{c^3}
\left[(2c^2+1)\sinh(2c)-2c\cosh(2c)\right]}.
$$

At $c=0$ these expressions have the continuous limiting values $4\pi$ and $4\pi/3$. Writing them as $A=T_{kk}=3\alpha+\beta$ and $B=T_{ij}y_iy_j=\alpha+\beta$ gives

$$
\boxed{\alpha=\frac{A-B}{2},\qquad \beta=\frac{3B-A}{2}}.
$$

## 11B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11b/solution">Solution</h3>

↑ **Parent:** [11B](#11b)

Using the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) and the [epsilon-delta identity](../../../calculus.md#contraction-of-two-levi-civita-symbols),

$$
[\nabla\times(\nabla\times A)]_i
=\epsilon_{ijk}\epsilon_{klm}\partial_j\partial_lA_m
=\partial_i(\partial_jA_j)-\partial_j\partial_jA_i.
$$

Therefore

$$
\boxed{\nabla\times(\nabla\times A)=\nabla(\nabla\mathbin\cdot A)-\nabla^2A}.
$$

One particularly simple [vector potential](../../../calculus.md#vector-potential) for $u$ is

$$
\boxed{A=\frac13(z^3,x^3,y^3)}.
$$

Direct differentiation gives $\nabla\mathbin\cdot A=0$ and $\nabla\times A=(y^2,z^2,x^2)=u$.

Parametrize the curved cone by

$$
R(z,\varphi)=(z\tan\alpha\cos\varphi,
z\tan\alpha\sin\varphi,z).
$$

The outward [oriented surface element](../../../calculus.md#oriented-surface-element) is

$$
d\mathbf S=(R_\varphi\times R_z)\,d\varphi\,dz
=z(\tan\alpha\cos\varphi,\tan\alpha\sin\varphi,-\tan^2\alpha)\,d\varphi\,dz.
$$

Substitution and integration over $0\leq z\leq h$, $0\leq\varphi<2\pi$ give

$$
\boxed{\int_{S_1}u\mathbin\cdot d\mathbf S
=-\frac{\pi h^4\tan^4\alpha}{4}}.
$$

Because $\nabla\mathbin\cdot u=0$, the [divergence theorem](../../../calculus.md#divergence-theorem) predicts that the two outward fluxes sum to zero. On the top disk $S_2$, $d\mathbf S=(0,0,1)\,dx\,dy$ and $u_z=x^2$, so, with $R=h\tan\alpha$,

$$
\int_{S_2}u\mathbin\cdot d\mathbf S
=\int_{x^2+y^2\leq R^2}x^2\,dx\,dy
=\boxed{\frac{\pi R^4}{4}}
=\frac{\pi h^4\tan^4\alpha}{4},
$$

as predicted.

The outward orientation on $S_2$ induces the stated anticlockwise orientation on $C$, whereas the outward orientation on $S_1$ induces the reverse orientation. Since $u=\nabla\times A$, [Stokes theorem](../../../calculus.md#stokes-theorem) predicts

$$
\int_{S_2}u\mathbin\cdot d\mathbf S=\oint_CA\mathbin\cdot d\mathbf l,
\qquad
\int_{S_1}u\mathbin\cdot d\mathbf S=-\oint_CA\mathbin\cdot d\mathbf l.
$$

On $C$, put $(x,y,z)=(R\cos\varphi,R\sin\varphi,h)$. Then

$$
\oint_CA\mathbin\cdot d\mathbf l
=\frac13\int_0^{2\pi}
\left[-h^3R\sin\varphi+R^4\cos^4\varphi\right]d\varphi
=\boxed{\frac{\pi R^4}{4}},
$$

verifying both identities.

## 12B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12b/a">a</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/a/solution">Solution</h4>

↑ **Parent:** [A](#12b/a)

[Green's first identity](../../../partial-differential-equation.md#green-s-first-identity) and the boundary condition give

$$
\int_V|\nabla u|^2dV
=\int_Su\frac{\partial u}{\partial n}dS-\int_Vu\nabla^2u\,dV=0.
$$

Thus $\nabla u=0$, so $u$ is constant on each connected component of $V$; its zero boundary value forces $\boxed{u=0}$.

Since $w-v=0$ on $S$ and $\nabla^2v=0$, another application of [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity) gives

$$
\int_V\nabla v\mathbin\cdot\nabla(w-v)dV=0.
$$

Consequently

$$
\boxed{\int_V\nabla v\mathbin\cdot\nabla w\,dV
=\int_V|\nabla v|^2dV}.
$$

Expanding $\nabla w=\nabla v+\nabla(w-v)$ and using the vanishing cross term yields the [Dirichlet principle](../../../calculus-of-variations.md#dirichlet-principle)

$$
\boxed{\int_V|\nabla w|^2dV
=\int_V\left(|\nabla v|^2+|\nabla(w-v)|^2\right)dV
\geq\int_V|\nabla v|^2dV}.
$$

<h3 id="12b/b">b</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/b/solution">Solution</h4>

↑ **Parent:** [B](#12b/b)

For a [spherically symmetric function](../../../calculus.md#spherically-symmetric-function) $\Phi(r)$, the [Laplacian in spherical coordinates](../../../partial-differential-equation.md#laplacian-in-spherical-coordinates) is

$$
\nabla^2\Phi=\frac1{r^2}\frac{d}{dr}(r^2\Phi').
$$

Integrating from zero to $r$ and using regularity at the origin gives

$$
\boxed{4\pi r^2\Phi'(r)=4\pi\int_0^rs^2\rho(s)\,ds}.
$$

For the stated density, integration and the boundary condition $\Phi(a)=0$ give

$$
\boxed{
\Phi(r)=
\begin{cases}
\displaystyle \rho_0\left(\frac{r^2}{6}-\frac{b^2}{2}+\frac{b^3}{3a}\right),&0\leq r\leq b,\\[6pt]
\displaystyle \frac{\rho_0b^3}{3}\left(\frac1a-\frac1r\right),&b<r\leq a.
\end{cases}}
$$

The two pieces and their first derivatives agree at $r=b$. If another solution existed, its difference from $\Phi$ would be [harmonic](../../../partial-differential-equation.md#harmonic-function) with zero boundary data, so part (a) proves [Uniqueness of the Dirichlet problem](../../../analysis.md#uniqueness-of-the-dirichlet-problem).

On the shell $U(b,a)$, normalize the outer radial part to obtain the harmonic function

$$
v(r)=\frac{b(a-r)}{(a-b)r},
\qquad v(b)=1,\quad v(a)=0.
$$

By the [Dirichlet principle](../../../calculus-of-variations.md#dirichlet-principle), this function minimizes the energy among all $w$ with the same boundary values. Since

$$
v'(r)=-\frac{ab}{(a-b)r^2},
$$

its energy is

$$
4\pi\int_b^a r^2|v'(r)|^2dr
=\frac{4\pi a^2b^2}{(a-b)^2}\left(\frac1b-\frac1a\right)
=\frac{4\pi ab}{a-b}.
$$

Therefore

$$
\boxed{\int_{U(b,a)}|\nabla w|^2dV\geq\frac{4\pi ab}{a-b}}.
$$

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
