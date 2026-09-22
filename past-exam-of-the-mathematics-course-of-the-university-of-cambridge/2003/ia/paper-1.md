# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2003/PaperIA_1.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2003/PaperIA_1.pdf)

**Table of contents**

- [1B](#1b)
  - [a](#1b/a)
    - [Solution](#1b/a/solution)
  - [b](#1b/b)
    - [Solution](#1b/b/solution)
- [2D](#2d)
  - [Solution](#2d/solution)
- [3B](#3b)
  - [Solution](#3b/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
  - [i](#4c/i)
    - [Solution](#4c/i/solution)
  - [ii](#4c/ii)
    - [Solution](#4c/ii/solution)
- [5B](#5b)
  - [a](#5b/a)
    - [Solution](#5b/a/solution)
  - [b](#5b/b)
    - [i](#5b/b/i)
      - [Solution](#5b/b/i/solution)
    - [ii](#5b/b/ii)
      - [Solution](#5b/b/ii/solution)
- [6A](#6a)
  - [Solution](#6a/solution)
- [7B](#7b)
  - [i](#7b/i)
    - [Solution](#7b/i/solution)
  - [ii](#7b/ii)
    - [Solution](#7b/ii/solution)
  - [Solution](#7b/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
  - [i](#8d/i)
    - [Solution](#8d/i/solution)
  - [ii](#8d/ii)
    - [Solution](#8d/ii/solution)
  - [iii](#8d/iii)
    - [Solution](#8d/iii/solution)
- [9F](#9f)
  - [Solution](#9f/solution)
- [10F](#10f)
  - [Solution](#10f/solution)
  - [i](#10f/i)
    - [Solution](#10f/i/solution)
  - [ii](#10f/ii)
    - [Solution](#10f/ii/solution)
  - [iii](#10f/iii)
    - [Solution](#10f/iii/solution)
- [11B](#11b)
  - [Solution](#11b/solution)
- [12C](#12c)
  - [Solution](#12c/solution)

## 1B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1b/a">a</h3>

↑ **Parent:** [1B](#1b)

<h4 id="1b/a/solution">Solution</h4>

↑ **Parent:** [A](#1b/a)

Compose [permutations](../../../combinatorics.md#permutation) from right to left. Tracking the four symbols through the two [permutation cycles](../../../finite-group-theory.md#permutation-cycle) gives $1\mapsto2\mapsto1$ and $3\mapsto4\mapsto3$. Thus the [cycle decomposition of a permutation](../../../mathematics.md#cycle-decomposition-of-a-permutation) is

$$
\boxed{(123)(234)=(12)(34).}
$$

The disjoint transpositions commute, and squaring their product gives the [identity element](../../../group.md#identity-element), while the product itself is nonidentity. Its [order of a group element](../../../group-theory.md#order-of-a-group-element) is therefore **two**. Each transposition has negative [sign of a permutation](../../../finite-group-theory.md#sign-of-a-permutation), so the product has sign $(-1)^2=\boxed{+1}$: it is an [even permutation](../../../finite-group-theory.md#even-permutation).

<h3 id="1b/b">b</h3>

↑ **Parent:** [1B](#1b)

<h4 id="1b/b/solution">Solution</h4>

↑ **Parent:** [B](#1b/b)

If $y=gxg^{-1}$, cancellation of successive $g^{-1}g$ factors gives $y^k=gx^kg^{-1}$ for every positive integer $k$. Hence $y^k$ is the [identity element](../../../group.md#identity-element) exactly when $x^k$ is, proving that [conjugate group elements](../../../group-theory.md#conjugate-group-elements) have the same [order of a group element](../../../group-theory.md#order-of-a-group-element). For [permutations](../../../combinatorics.md#permutation), the sign [group homomorphism](../../../group-theory.md#group-homomorphism) similarly gives

$$
\operatorname{sgn}(gxg^{-1})=\operatorname{sgn}(g)\operatorname{sgn}(x)\operatorname{sgn}(g)^{-1}=\operatorname{sgn}(x).
$$

Thus [conjugate permutations](../../../group-theory.md#conjugate-permutation) have the same [sign of a permutation](../../../finite-group-theory.md#sign-of-a-permutation).

The converse is false: [permutation order and sign do not determine conjugacy](../../../finite-group-theory.md#permutation-order-and-sign-do-not-determine-conjugacy). In the [symmetric group](../../../finite-group-theory.md#symmetric-group) $S_6$, take $x=(123)$ and $y=(123)(456)$. Both have order three and positive sign. However, $x$ fixes three symbols whereas $y$ fixes none. If $x$ fixes a symbol $j$, then $gxg^{-1}$ fixes $g(j)$, and applying the inverse conjugation gives a bijection between the fixed-symbol sets. Their different fixed-point counts therefore prove that $x,y$ are not conjugate. Equivalently their [cycle types](../../../finite-group-theory.md#cycle-type) $3\,1^3$ and $3^2$ differ. **Equal order and sign are necessary, but not sufficient, for conjugacy.**

## 2D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2d/solution">Solution</h3>

↑ **Parent:** [2D](#2d)

The two diagonal $2\times2$ blocks allow the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) to factor immediately:

$$
\det(\lambda I-A)=\bigl[(\lambda-i)^2-1\bigr]\bigl[(\lambda-i)^2+1\bigr].
$$

Thus the [characteristic equation](../../../differential-equation.md#characteristic-equation-of-a-constant-coefficient-differential-equation) is

$$
\boxed{(\lambda-i-1)(\lambda-i+1)\lambda(\lambda-2i)=0.}
$$

Solving the two block [eigenvalue](../../../linear-operator-theory.md#eigenvalue) equations gives the following nonzero [eigenvectors](../../../linear-operator-theory.md#eigenvector) and corresponding [eigenvalues](../../../linear-operator-theory.md#eigenvalue):

$$
\begin{array}{c|c}
\text{eigenvector}&\text{eigenvalue}\\\hline
a=(1,1,0,0)^T&1+i\\
b=(1,-1,0,0)^T&-1+i\\
c=(0,0,1,i)^T&2i\\
d=(0,0,1,-i)^T&0
\end{array}
$$

For example, the lower block maps $(1,i)^T$ to $(2i,-2)^T=2i(1,i)^T$, and maps $(1,-i)^T$ to zero. The four [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are distinct. Alternatively, the [determinant](../../../linear-algebra.md#determinant) of the matrix with columns $a,b,c,d$ is $(-2)(-2i)=4i\ne0$. Hence they form a [basis](../../../vector-space.md#basis) and **span the complex vector space $\mathbb C^4$**. Their nonzero scalar multiples are all the corresponding eigenvectors.

For any [eigenvector](../../../linear-operator-theory.md#eigenvector) $v$ with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda_v$, its one-dimensional [vector subspace](../../../vector-space.md#vector-subspace) satisfies $A(sv)=\lambda_vsv$. If $\lambda_v\ne0$, every $tv$ has preimage $(t/\lambda_v)v$, so the restricted [linear map](../../../vector-space.md#linear-map) is onto that same subspace. Consequently

$$
\boxed{A(\mathbb Ca)=\mathbb Ca,\quad A(\mathbb Cb)=\mathbb Cb,\quad A(\mathbb Cc)=\mathbb Cc,\quad A(\mathbb Cd)=\{0\}.}
$$

The last line is the [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) direction: multiplication by $A$ collapses that line to the zero-dimensional subspace.

## 3B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3b/solution">Solution</h3>

↑ **Parent:** [3B](#3b)

A real [function](../../../function.md) is [differentiable](../../../analysis.md#differentiable-function) at an interior point $x$ when the finite [limit](../../../calculus.md#limit-of-a-function)

$$
f'(x)=\lim_{h\to0,\ h\ne0}\frac{f(x+h)-f(x)}h
$$

exists, with $h$ restricted so $x+h$ lies in its domain. In quantified form, for every $\varepsilon>0$ there is $\delta>0$ such that $0<|h|<\delta$ implies that the [difference quotient](../../../calculus.md#difference-quotient) differs from $f'(x)$ by less than $\varepsilon$.

To prove [differentiability implies continuity](../../../analysis.md#differentiability-implies-continuity), the convergent [difference quotient](../../../calculus.md#difference-quotient) is bounded by $|f'(x)|+1$ for sufficiently small nonzero $h$. Thus $|f(x+h)-f(x)|\le(|f'(x)|+1)|h|\to0$. This is exactly [continuity](../../../calculus.md#continuous-function) at $x$.

At zero, the particular function has [difference quotient](../../../calculus.md#difference-quotient) $h\sin(1/h)$. The bound $|h\sin(1/h)|\le|h|$ and the [squeeze theorem](../../../calculus.md#squeeze-theorem) give

$$
\boxed{f'(0)=0.}
$$

For $x\ne0$, the [product rule](../../../calculus.md#product-rule) and [chain rule](../../../calculus.md#chain-rule) give

$$
f'(x)=2x\sin(1/x)-\cos(1/x).
$$

At $x_k=1/(2\pi k)$ this equals $-1$, although $x_k\to0$ and $f'(0)=0$. At $y_k=1/((2k+1)\pi)$ it equals $+1$. Hence the derivative has no limit at zero and is **not continuous there**. This demonstrates that [differentiability does not imply continuity of the derivative](../../../analysis.md#differentiability-does-not-imply-continuity-of-the-derivative), even though the function itself is continuous.

## 4C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

The [radius of convergence](../../../real-analysis.md#radius-of-convergence) of a [power series](../../../real-analysis.md#power-series) $\sum_{n\ge0}a_nz^n$ is the unique $R\in[0,\infty]$ for which the series converges absolutely when $|z|<R$ and diverges when $|z|>R$. When $R=\infty$ it converges for every complex $z$; when $R=0$ it converges only at the centre. The definition makes no assertion about convergence on $|z|=R$, so boundary points must be checked separately.

<h3 id="4c/i">i</h3>

↑ **Parent:** [4C](#4c)

<h4 id="4c/i/solution">Solution</h4>

↑ **Parent:** [I](#4c/i)

The absolute ratio of successive terms is $|z|\,n^2/(n+1)^2\to|z|$. The [ratio test](../../../real-analysis.md#ratio-test) gives convergence for $|z|<1$ and divergence for $|z|>1$, so the [radius of convergence](../../../real-analysis.md#radius-of-convergence) is $\boxed{R=1}$. On the boundary, $|n^{-2}z^n|=n^{-2}$ and

$$
\sum_{n=2}^N\frac1{n^2}\le\sum_{n=2}^N\frac1{n(n-1)}=1-\frac1N.
$$

The positive partial sums are bounded, and thus converge. By the [comparison test for series](../../../real-analysis.md#comparison-test-for-series), the original [power series](../../../real-analysis.md#power-series) **converges absolutely at every point of $|z|=1$**.

<h3 id="4c/ii">ii</h3>

↑ **Parent:** [4C](#4c)

<h4 id="4c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4c/ii)

The coefficient ratio is

$$
\frac{n+1+2^{-(n+1)}}{n+2^{-n}}\longrightarrow1.
$$

Thus the [ratio test](../../../real-analysis.md#ratio-test) again gives [radius of convergence](../../../real-analysis.md#radius-of-convergence) $\boxed{R=1}$. On $|z|=1$, however, the terms have absolute value $n+2^{-n}$, which does not tend to zero. The necessary term condition for a [convergent series](../../../real-analysis.md#convergent-series) fails at every boundary point. Therefore this [power series](../../../real-analysis.md#power-series) **diverges everywhere on $|z|=1$**.

## 5B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5b/a">a</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/a/solution">Solution</h4>

↑ **Parent:** [A](#5b/a)

A positive, counterclockwise [rotation](../../../riemannian-geometry.md#rotation-mathematics) takes the standard [basis](../../../vector-space.md#basis) vectors $(1,0)^T$ and $(0,1)^T$ to $(\cos\theta,\sin\theta)^T$ and $(-\sin\theta,\cos\theta)^T$. These images are the columns of its [rotation matrix](../../../linear-algebra.md#rotation-matrix), so

$$
\boxed{R(\theta)=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}.}
$$

It fixes the origin, preserves the [dot product](../../../linear-algebra.md#dot-product) and has [determinant](../../../linear-algebra.md#determinant) one.

<h3 id="5b/b">b</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/b/i">i</h4>

↑ **Parent:** [B](#5b/b)

<h5 id="5b/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5b/b/i)

Since $AA^T=I$ and $\det A=1$, $A$ is an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) in the [special orthogonal group](../../../linear-algebra.md#special-orthogonal-group). It also satisfies $A^TA=I$ and thus preserves the [dot product](../../../linear-algebra.md#dot-product). Normalize the fixed [eigenvector](../../../linear-operator-theory.md#eigenvector) to $e_3=v/\|v\|$. For $u\cdot e_3=0$,

$$
(Au)\cdot e_3=(Au)\cdot(Ae_3)=u\cdot e_3=0,
$$

so the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) of the fixed axis is invariant. Choose an oriented [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $e_1,e_2,e_3$. In this basis the [matrix](../../../vector-space.md#matrix) has form $\operatorname{diag}(B,1)$, where $B$ is a real $2\times2$ orthogonal matrix of determinant one.

Write the first column of $B$ as $(\cos\theta,\sin\theta)^T$. Its unit second column must be perpendicular to the first; positivity of the determinant selects $(-\sin\theta,\cos\theta)^T$. Thus $B=R(\theta)$, and $A$ fixes the axis through $v$ while rotating its perpendicular plane by $\theta$. Since [trace](../../../linear-algebra.md#matrix-trace) is invariant under change of basis,

$$
\operatorname{tr}A=1+2\cos\theta,\qquad \boxed{\cos\theta=\frac{\operatorname{tr}A-1}{2}.}
$$

This proves that $A$ is the required axial [rotation](../../../riemannian-geometry.md#rotation-mathematics). The trace determines the unsigned angle; the action in the oriented perpendicular plane determines its sign. The identity case has angle zero and any axis.

<h4 id="5b/b/ii">ii</h4>

↑ **Parent:** [B](#5b/b)

<h5 id="5b/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5b/b/ii)

Use the [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) identity $A(I-A^T)=A-I$. The product rule for [determinants](../../../linear-algebra.md#determinant), $\det A=1$, and invariance of determinant under [matrix transpose](../../../vector-space.md#transpose) give

$$
\det(A-I)=\det A\det(I-A^T)=\det(I-A)=-\det(A-I),
$$

where the last sign comes from dimension three. Hence $\det(A-I)=0$. The real [linear map](../../../vector-space.md#linear-map) $A-I$ has a nonzero real vector in its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map), so **$A$ has an eigenvector with eigenvalue one**. This is the [odd-dimensional special orthogonal transformation has a fixed vector](../../../linear-algebra.md#odd-dimensional-special-orthogonal-transformation-has-a-fixed-vector) property, here proved directly without first classifying the other eigenvalues.

## 6A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6a/solution">Solution</h3>

↑ **Parent:** [6A](#6a)

For a [linear map](../../../vector-space.md#linear-map) $\alpha$, its [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) and [image of a linear map](../../../vector-space.md#image-of-a-linear-map) are

$$
K=\{x\in\mathbb R^3:\alpha x=0\},\qquad I=\{\alpha x:x\in\mathbb R^3\}.
$$

By the definition of the image, $\alpha x=y$ has a solution exactly when $y\in I$. If $x_0$ is one solution, every other solution is $x_0+k$ for some $k\in K$: subtracting the two equations proves necessity, and linearity proves sufficiency. Thus a solvable equation has a unique solution exactly when $K=\{0\}$.

Write the columns of the given matrix as $c_1=(1,0,1)^T$, $c_2=(1,t,t)^T$ and $c_3=(t,-2b,0)^T$. Its [determinant](../../../linear-algebra.md#determinant) is

$$
\det\alpha=-t^2+2bt-2b=-D,\qquad D=t^2-2bt+2b.
$$

The columns $c_1,c_2$ are [linearly independent](../../../vector-space.md#linear-independence) for every real $t$: proportionality would require the proportionality factor to be one from the first coordinate, then simultaneously $t=0$ from the second and $t=1$ from the third. Thus the [rank](../../../linear-algebra.md#rank-one-quadratic-form) is always at least two.

If $D\ne0$, the matrix is invertible and

$$
\boxed{K=\{0\},\qquad I=\mathbb R^3.}
$$

If $D=0$, the rank is exactly two. A direct substitution verifies the nonzero kernel vector $k=(-t^2,t,t-1)^T$: its first and third row products vanish identically and its second is $D$. The [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) then gives

$$
\boxed{K=\operatorname{span}\{(-t^2,t,t-1)^T\}.}
$$

In that case the image is the plane spanned by $c_1,c_2$. Their [cross product](../../../vector-space.md#cross-product) is $(-t,1-t,t)^T$, so an equivalent description is

$$
\boxed{I=\operatorname{span}\{(1,0,1)^T,(1,t,t)^T\}=\{y:-ty_1+(1-t)y_2+ty_3=0\}.}
$$

These formulas include the singular case $t=b=0$, giving kernel $\mathbb R(0,0,1)$ and image $y_2=0$; no exceptional case was lost by dividing by $t$.

Finally, when $0<b<2$,

$$
D=(t-b)^2+b(2-b)>0\quad\text{for every real }t.
$$

Therefore **the equation has a unique solution for every $t$ and every $y\in\mathbb R^3$**, in particular for every $y\in I$. Outside this parameter range, the singular cases are precisely $t=b\pm\sqrt{b(b-2)}$ when that square root is real.

## 7B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7b/i">i</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/i/solution">Solution</h4>

↑ **Parent:** [I](#7b/i)

For a [group action](../../../group-theory.md#group-action) of $G$ on a set $X$ and $x\in X$, the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) states

$$
|Gx|=[G:G_x],\qquad G_x=\{g\in G:gx=x\}.
$$

If $G$ is finite, this becomes $\boxed{|G|=|Gx|\,|G_x|}$. The underlying bijection sends the left [coset](../../../group-theory.md#coset) $gG_x$ to $gx$. Equality of two image points is equivalent to $g_2^{-1}g_1\in G_x$, so this map is both well-defined and injective, and it is surjective by the definition of the [group orbit](../../../group-theory.md#orbit-of-a-group-action).

<h3 id="7b/ii">ii</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7b/ii)

Place the cube's vertices at $(\pm1,\pm1,\pm1)$. Every symmetry fixes its centre, and permutes the three perpendicular pairs of face normals, so it is a [signed permutation matrix](../../../vector-space.md#signed-permutation-matrix). Conversely every such matrix preserves the cube. The [symmetry group of a cube](../../../group-theory.md#symmetry-group-of-a-cube) acts transitively on its eight vertices: independent coordinate sign changes take $(1,1,1)$ to any vertex.

A symmetry fixing $(1,1,1)$ must permute its three incident edges. This gives an injective map from its [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) into $S_3$, since those three edge directions determine the linear transformation. All six permutations are realized by coordinate [permutation matrices](../../../vector-space.md#permutation-matrix), which fix $(1,1,1)$. Thus the vertex stabilizer has order six. The [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) now yields

$$
\boxed{|G|=8\cdot6=48.}
$$

The use of all symmetries includes reflections as well as the twenty-four elements of the [rotational symmetry group of a cube](../../../group-theory.md#rotational-symmetry-group-of-a-cube).

<h3 id="7b/solution">Solution</h3>

↑ **Parent:** [7B](#7b)

There are nontrivial proper [normal subgroups](../../../group-theory.md#normal-subgroup). The [determinant](../../../linear-algebra.md#determinant) defines a surjective [group homomorphism](../../../group-theory.md#group-homomorphism) $G\to\{1,-1\}$. Its kernel is the [rotational symmetry group of a cube](../../../group-theory.md#rotational-symmetry-group-of-a-cube), a normal subgroup of order twenty-four. Also $\{I,-I\}$ is a central subgroup of order two: central inversion preserves the cube and commutes with every matrix. Both provide affirmative examples.

For the body diagonal through $(1,1,1)$, write a general cube symmetry as $D_\varepsilon P$, with $P$ a [permutation matrix](../../../vector-space.md#permutation-matrix) and $D_\varepsilon=\operatorname{diag}(\varepsilon_1,\varepsilon_2,\varepsilon_3)$, each $\varepsilon_j=\pm1$. Since $P(1,1,1)^T=(1,1,1)^T$, preserving the unoriented diagonal requires $(\varepsilon_1,\varepsilon_2,\varepsilon_3)$ to be either $(1,1,1)$ or $(-1,-1,-1)$. Thus

$$
H=\{\varepsilon P:\varepsilon\in\{1,-1\},\ P\text{ a }3\times3\text{ permutation matrix}\}.
$$

The map $(\pi,\varepsilon)\mapsto\varepsilon P_\pi$ from $S_3\times C_2$ to $H$ is a [group homomorphism](../../../group-theory.md#group-homomorphism), because central inversion commutes with every coordinate permutation. It is surjective by the displayed description and injective because a permutation matrix cannot equal the negative of another permutation matrix. Consequently the [body-diagonal stabilizer in the cube symmetry group](../../../group-theory.md#body-diagonal-stabilizer-in-the-cube-symmetry-group) is

$$
\boxed{H\cong S_3\times C_2,\qquad |H|=12.}
$$

This also agrees with the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) for the transitive action on the four body diagonals. The line is preserved as a set, so exchanging its opposite endpoints is allowed.

## 8D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

Two nonzero vectors are [linearly independent](../../../vector-space.md#linear-independence) when $ax+by=0$ implies $a=b=0$. Their [span](../../../vector-space.md#linear-span) then has [dimension](../../../vector-space.md#dimension-vector-space) two. If they are [linearly dependent](../../../vector-space.md#linear-dependence), one is a scalar multiple of the other, so their span is a nonzero line and has dimension one. Thus the requested dimensions are **two and one, respectively**.

The [dot product](../../../linear-algebra.md#dot-product) and corresponding [Euclidean norm](../../../functional-analysis.md#euclidean-norm) are

$$
x\cdot y=\sum_{j=1}^n x_jy_j,\qquad \|x\|=\sqrt{x\cdot x}=\left(\sum_{j=1}^n x_j^2\right)^{1/2}.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) states $\boxed{|x\cdot y|\le\|x\|\,\|y\|}$. If $y=0$ this is immediate. Otherwise the nonnegativity of a squared norm, with $t=(x\cdot y)/\|y\|^2$, gives

$$
0\le\|x-ty\|^2=\|x\|^2-\frac{(x\cdot y)^2}{\|y\|^2}.
$$

Multiplying by $\|y\|^2$ and taking square roots proves the inequality. Equality holds precisely when the vectors are linearly dependent. Expanding another squared norm and using the inequality gives

$$
\|x+y\|^2=\|x\|^2+2x\cdot y+\|y\|^2\le(\|x\|+\|y\|)^2,
$$

and hence the [triangle inequality](../../../topological-analysis.md#triangle-inequality) $\boxed{\|x+y\|\le\|x\|+\|y\|}$.

In $\mathbb R^3$, the two vectors lie in a common plane. If their directions make angle $\alpha$, the [law of cosines](../../../geometry-and-topology.md#law-of-cosines) gives $\|x-y\|^2=\|x\|^2+\|y\|^2-2\|x\|\|y\|\cos\alpha$. Comparing with the dot-product expansion yields

$$
\boxed{x\cdot y=\|x\|\,\|y\|\cos\alpha.}
$$

The sketch shows the same relation as a projection: multiply the length of $x$ by the signed component of $y$ in its direction. That component is negative for obtuse $\alpha$.

<a id="8d/image-dot-product-as-a-signed-projection-in-the-plane-of-two-vectors"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1-dot-product-projection.png)

**[Figure 1](#8d/image-dot-product-as-a-signed-projection-in-the-plane-of-two-vectors). Dot product as a signed projection in the plane of two vectors**.

A [unit vector](../../../vector-space.md#unit-vector) is a vector of [Euclidean norm](../../../functional-analysis.md#euclidean-norm) one, equivalently $u\cdot u=1$. In particular the [dot product](../../../linear-algebra.md#dot-product) of two unit vectors is the cosine of their mutual angle.

<h3 id="8d/i">i</h3>

↑ **Parent:** [8D](#8d)

<h4 id="8d/i/solution">Solution</h4>

↑ **Parent:** [I](#8d/i)

Put $q=u\cdot v$ and $d=u+v$. The [linear independence](../../../vector-space.md#linear-independence) assumption implies $d\ne0$. Since $w$ is a [unit vector](../../../vector-space.md#unit-vector), the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
S=q+w\cdot d\ge q-\|d\|.
$$

Equality holds exactly when $w$ points opposite to $d$. Its required unit length then fixes the scale:

$$
\boxed{w=-\frac{u+v}{\|u+v\|},\qquad\lambda=-\frac1{\|u+v\|}=-\frac1{\sqrt{2+2q}}.}
$$

Here $\|u+v\|^2=2+2q$ because both vectors have unit norm. The minimizing vector is unique, and the [minimum pairwise dot-product sum of three unit vectors](../../../probability-and-statistics.md#minimum-pairwise-dot-product-sum-of-three-unit-vectors) for these fixed $u,v$ is

$$
\boxed{S_{\min}=q-\sqrt{2+2q}.}
$$

<h3 id="8d/ii">ii</h3>

↑ **Parent:** [8D](#8d)

<h4 id="8d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8d/ii)

The [triangle inequality](../../../topological-analysis.md#triangle-inequality) for the two [unit vectors](../../../vector-space.md#unit-vector) gives $0<\|u+v\|\le2$. Taking reciprocals and using the negative sign in $\lambda=-1/\|u+v\|$ yields

$$
\boxed{\lambda\le-\frac12.}
$$

In fact equality would require $u=v$, by the equality condition in the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Since the two vectors here are [linearly independent](../../../vector-space.md#linear-independence), the inequality is strict for every admissible pair.

<h3 id="8d/iii">iii</h3>

↑ **Parent:** [8D](#8d)

<h4 id="8d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#8d/iii)

For the stated angle, $q=\cos(2\pi/3)=-1/2$, so $\|u+v\|=\sqrt{2+2q}=1$. The minimizing [unit vector](../../../vector-space.md#unit-vector) is therefore $w=-(u+v)$, and

$$
\boxed{\lambda=-1,\qquad S_{\min}=-\frac12-1=-\frac32.}
$$

Indeed all three pairwise [dot products](../../../linear-algebra.md#dot-product) equal $-1/2$, so the vectors lie in one plane, separated by $120$ degrees. This is also the global [minimum pairwise dot-product sum of three unit vectors](../../../probability-and-statistics.md#minimum-pairwise-dot-product-sum-of-three-unit-vectors): for any three unit vectors,

$$
0\le\|u+v+w\|^2=3+2S,
$$

so $S\ge-3/2$, with equality exactly when $u+v+w=0$.

## 9F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9f/solution">Solution</h3>

↑ **Parent:** [9F](#9f)

To prove the [Archimedean property](../../../arithmetic.md#archimedean-property), suppose the positive integers were bounded above in $\mathbb R$. By the [least upper bound axiom](../../../real-analysis.md#least-upper-bound-property) they would have a finite [supremum](../../../real-analysis.md#supremum) $s$. Since $s-1$ is not an upper bound, some positive integer $k$ satisfies $k>s-1$. Then the positive integer $k+1>s$, contradicting the definition of $s$. Thus the positive integers are unbounded. Equivalently, for any positive real $a,b$, some positive integer $n$ satisfies $na>b$, by applying unboundedness to $b/a$.

For fixed $m$, put $r_m=\cos^2(m!\pi x)$. The standard properties needed are $0\le\cos^2 t\le1$, and $\cos^2 t=1$ exactly when $t\in\pi\mathbb Z$. If $0\le r<1$, then $r^n\to0$; for $0<r<1$ this also follows from the [Bernoulli inequality](../../../algebra.md#bernoulli-s-inequality), since $r^{-n}\ge1+n(r^{-1}-1)\to\infty$. Therefore the inner [limit](../../../calculus.md#limit-of-a-function) is

$$
\lim_{n\to\infty}\cos^{2n}(m!\pi x)=\begin{cases}1,&m!x\in\mathbb Z,\\0,&m!x\notin\mathbb Z.\end{cases}
$$

If $x=p/q$ is a [rational number](../../../number-theory.md#rational-number), with $q\ge1$, then $q$ divides the [factorial](../../../combinatorics.md#factorial) $m!$ whenever $m\ge q$. Hence $m!x$ is an integer for all sufficiently large $m$, and the outer limit is one. This includes the endpoints $x=0,1$. If $x$ is an [irrational number](../../../algebra.md#irrational-number), $m!x$ cannot be an integer for any $m$, since division by $m!$ would make $x$ rational. Then every inner limit is zero. The [factorial cosine iterated limit detects rationality](../../../real-analysis.md#factorial-cosine-iterated-limit-detects-rationality) result is consequently

$$
\boxed{\lim_{m\to\infty}\left[\lim_{n\to\infty}\cos^{2n}(m!\pi x)\right]=\begin{cases}1,&x\in\mathbb Q,\\0,&x\notin\mathbb Q.\end{cases}}
$$

Each inner limit was taken with $m$ fixed; the argument does not interchange the two limits or assert a joint limit as both indices grow.

## 10F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10f/solution">Solution</h3>

↑ **Parent:** [10F](#10f)

The [integral test for convergence](../../../real-analysis.md#integral-test-for-convergence) applies when $a_n=h(n)$ for all sufficiently large $n$, where $h$ is nonnegative, continuous and nonincreasing on $[N,\infty)$. It states that $\sum_{n=N}^\infty a_n$ converges if and only if the [improper integral](../../../real-analysis.md#improper-integral) $\int_N^\infty h(x)\,dx$ is finite. Its comparison bounds are

$$
\int_N^{M+1}h(x)\,dx\le\sum_{n=N}^M h(n)\le h(N)+\int_N^M h(x)\,dx.
$$

No conclusion about an arbitrary nonnegative sequence follows without such a monotone comparison function; finite initial terms do not affect convergence.

For $h(x)=x^{-\alpha}$ with $\alpha>0$, all the hypotheses hold. If $\alpha\ne1$,

$$
\int_1^R x^{-\alpha}\,dx=\frac{R^{1-\alpha}-1}{1-\alpha},
$$

whereas for $\alpha=1$ the integral is $\log R$. The first expression has a finite limit exactly when $\alpha>1$. Thus the [p-series](../../../real-analysis.md#p-series) satisfies

$$
\boxed{\sum_{n=1}^\infty n^{-\alpha}\text{ converges iff }\alpha>1;\quad\text{it diverges for }0<\alpha\le1.}
$$

<h3 id="10f/i">i</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/i/solution">Solution</h4>

↑ **Parent:** [I](#10f/i)

On $[3,\infty)$, $h(x)=1/(x\log x)$ is positive, continuous and decreasing, since its denominator has positive derivative $\log x+1$. Substituting $u=\log x$ gives

$$
\int_3^R\frac{dx}{x\log x}=\log\log R-\log\log3\longrightarrow\infty.
$$

The [integral test for convergence](../../../real-analysis.md#integral-test-for-convergence) therefore shows that the [series](../../../real-analysis.md#series-mathematics) is **divergent**.

<h3 id="10f/ii">ii</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10f/ii)

Because $3>e$, each of $x$, $\log x$ and $\log\log x$ is positive and increasing for $x\ge3$. Hence $h(x)=1/[x\log x(\log\log x)^2]$ is positive, continuous and decreasing. With $u=\log\log x$, $du=dx/(x\log x)$, so

$$
\int_3^\infty\frac{dx}{x\log x(\log\log x)^2}=\int_{\log\log3}^\infty u^{-2}\,du=\frac1{\log\log3}<\infty.
$$

The [integral test for convergence](../../../real-analysis.md#integral-test-for-convergence) implies that the [series](../../../real-analysis.md#series-mathematics) is **convergent**.

<h3 id="10f/iii">iii</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#10f/iii)

Compare with the divergent [series](../../../real-analysis.md#series-mathematics) from part (i). The ratio of its new summand to $1/(n\log n)$ is

$$
\frac{1/[n^{1+1/n}\log n]}{1/(n\log n)}=n^{-1/n}=e^{-(\log n)/n}\longrightarrow1.
$$

For completeness, $\log n=\int_1^n x^{-1}\,dx\le\int_1^n x^{-1/2}\,dx=2(\sqrt n-1)$, so $(\log n)/n\to0$. The [limit comparison test](../../../real-analysis.md#limit-comparison-test) now gives **divergence**. Although the exponent $1+1/n$ exceeds one for each summand, it approaches one and does not produce a convergent [p-series](../../../real-analysis.md#p-series) with a fixed exponent greater than one.

## 11B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11b/solution">Solution</h3>

↑ **Parent:** [11B](#11b)

For a partition $a=x_0<\cdots<x_k=b$ and tags $\xi_j\in[x_{j-1},x_j]$, form the [Riemann sum](../../../real-analysis.md#riemann-sum) $\sum_{j=1}^k f(\xi_j)(x_j-x_{j-1})$. The [Riemann integral](../../../real-analysis.md#riemann-integral) is the unique real number $I$ such that for every $\varepsilon>0$ there is $\delta>0$ for which every tagged partition with mesh $\max_j(x_j-x_{j-1})<\delta$ has its sum within $\varepsilon$ of $I$. Then $I=\int_a^b f(x)\,dx$. The stated continuity ensures existence, which need not be proved here.

The properties required are linearity, the integral of a constant, and [monotonicity of the Riemann integral](../../../real-analysis.md#monotonicity-of-the-riemann-integral). Monotonicity follows directly because a nonnegative function has nonnegative [Riemann sums](../../../real-analysis.md#riemann-sum), and therefore a nonnegative integral. Integrating $f-m\ge0$ and $M-f\ge0$ gives

$$
\boxed{m(b-a)\le\int_a^b f(x)\,dx\le M(b-a).}
$$

Since $g\ge0$, multiplication preserves the pointwise inequalities: $mg\le fg\le Mg$. The continuous products are integrable, so the same monotonicity and linearity give

$$
\boxed{m\int_a^b g(x)\,dx\le\int_a^b f(x)g(x)\,dx\le M\int_a^b g(x)\,dx.}
$$

Neither $m$ nor $f$ needs to be nonnegative for this argument.

For the first limit, set $r_n=n^{-1/2}$, $g_n(x)=ne^{-nx}$, and $\varepsilon_n=\max_{0\le x\le r_n}|f(x)-f(0)|$. By [continuity](../../../calculus.md#continuous-function) at zero, $\varepsilon_n\to0$. On this shrinking interval $f(0)-\varepsilon_n\le f(x)\le f(0)+\varepsilon_n$, and

$$
\int_0^{r_n}g_n(x)\,dx=1-e^{-\sqrt n}.
$$

Applying the weighted bounds just proved gives

$$
(f(0)-\varepsilon_n)(1-e^{-\sqrt n})\le\int_0^{r_n}nf(x)e^{-nx}\,dx\le(f(0)+\varepsilon_n)(1-e^{-\sqrt n}).
$$

Both bounding expressions tend to $f(0)$, so the [squeeze theorem](../../../calculus.md#squeeze-theorem) proves the first limit.

For the full interval, continuity on $[0,1]$ gives a finite bound $B=\max_{[0,1]}|f|$ by the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem). The remaining tail has absolute value at most

$$
\left|\int_{r_n}^1nf(x)e^{-nx}\,dx\right|\le B\int_{r_n}^1ne^{-nx}\,dx=B(e^{-\sqrt n}-e^{-n})\longrightarrow0.
$$

Adding this to the already evaluated near-end integral proves

$$
\boxed{\lim_{n\to\infty}\int_0^{1/\sqrt n}nf(x)e^{-nx}\,dx=\lim_{n\to\infty}\int_0^1nf(x)e^{-nx}\,dx=f(0).}
$$

These are instances of a [one-sided exponential approximate identity](../../../fourier-analysis.md#one-sided-exponential-approximate-identity): the positive weight has total mass tending to one, concentrated in a shrinking neighborhood of zero. No interchange of limit and integral has been assumed.

## 12C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12c/solution">Solution</h3>

↑ **Parent:** [12C](#12c)

For real functions $u,v$ that are continuously differentiable on a closed interval $[a,b]$, [integration by parts](../../../calculus.md#integration-by-parts) states

$$
\boxed{\int_a^b u(x)v'(x)\,dx=[u(x)v(x)]_a^b-\int_a^b u'(x)v(x)\,dx.}
$$

It follows from the [product rule](../../../calculus.md#product-rule) and the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus). With the convention $\int_a^b=-\int_b^a$, the identity also applies to reversed limits. These regularity assumptions ensure that all the proper integrals exist.

For the smooth $f$ in the problem, define the [integral remainder in Taylor theorem](../../../calculus.md#integral-remainder-in-taylor-theorem) by

$$
R_n(t)=\frac1{(n-1)!}\int_0^t f^{(n)}(x)(t-x)^{n-1}\,dx.
$$

The [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) gives $f(t)=f(0)+R_1(t)$. Applying [integration by parts](../../../calculus.md#integration-by-parts) to $R_n$, with $u=f^{(n)}(x)$ and antiderivative $v=-(t-x)^n/n!$ of $(t-x)^{n-1}/(n-1)!$, gives

$$
R_n(t)=\frac{f^{(n)}(0)t^n}{n!}+\frac1{n!}\int_0^t f^{(n+1)}(x)(t-x)^n\,dx=\frac{f^{(n)}(0)t^n}{n!}+R_{n+1}(t).
$$

Induction starting from $n=1$ therefore proves

$$
\boxed{f(t)=\sum_{k=0}^{n-1}\frac{f^{(k)}(0)t^k}{k!}+\frac1{(n-1)!}\int_0^t f^{(n)}(x)(t-x)^{n-1}\,dx.}
$$

The same calculation holds for negative $t$: all integrals are oriented, and the segment joining $0$ and $t$ lies in $(-1,1)$. Thus the proof covers every stated $t$ and every positive integer $n$.

Now take $f(x)=\log(1-x)$. For $k\ge1$, differentiation gives $f^{(k)}(x)=-(k-1)!/(1-x)^k$, and $f(0)=0$. With $n=N+1$ and $t=1/2$, the [Taylor formula with integral remainder](../../../calculus.md#taylor-formula-with-integral-remainder) becomes

$$
\log2=\sum_{k=1}^N\frac1{k2^k}+J_N,\qquad J_N=\int_0^{1/2}\frac{(1/2-x)^N}{(1-x)^{N+1}}\,dx.
$$

For $0\le x\le1/2$, $0\le(1/2-x)/(1-x)\le1/2$ and $(1-x)^{-1}\le2$. Hence $0\le J_N\le2^{-N}$ after integrating over an interval of length $1/2$. Thus the [logarithmic series from an integral Taylor remainder](../../../calculus.md#logarithmic-series-from-an-integral-taylor-remainder) satisfies

$$
\boxed{\sum_{k=1}^\infty\frac1{k2^k}=\log2,\qquad 0\le\log2-\sum_{k=1}^N\frac1{k2^k}\le2^{-N}.}
$$

The explicit vanishing remainder establishes convergence and identifies the sum, without using a pre-existing logarithmic power series.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
