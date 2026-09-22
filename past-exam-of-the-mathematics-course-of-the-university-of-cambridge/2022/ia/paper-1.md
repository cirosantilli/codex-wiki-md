# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2022/paperia_1_2022.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2022/paperia_1_2022.pdf)

**Table of contents**

- [1B](#1b)
  - [a](#1b/a)
    - [i](#1b/a/i)
      - [Solution](#1b/a/i/solution)
    - [ii](#1b/a/ii)
      - [Solution](#1b/a/ii/solution)
    - [iii](#1b/a/iii)
      - [Solution](#1b/a/iii/solution)
  - [b](#1b/b)
    - [i](#1b/b/i)
      - [Solution](#1b/b/i/solution)
    - [ii](#1b/b/ii)
      - [Solution](#1b/b/ii/solution)
- [2B](#2b)
  - [a](#2b/a)
    - [i](#2b/a/i)
      - [Solution](#2b/a/i/solution)
    - [ii](#2b/a/ii)
      - [Solution](#2b/a/ii/solution)
  - [b](#2b/b)
    - [Solution](#2b/b/solution)
- [3D](#3d)
  - [Solution](#3d/solution)
- [4D](#4d)
  - [Solution](#4d/solution)
- [5B](#5b)
  - [a](#5b/a)
    - [i](#5b/a/i)
      - [Solution](#5b/a/i/solution)
    - [ii](#5b/a/ii)
      - [Solution](#5b/a/ii/solution)
    - [iii](#5b/a/iii)
      - [Solution](#5b/a/iii/solution)
  - [b](#5b/b)
    - [Solution](#5b/b/solution)
- [6B](#6b)
  - [a](#6b/a)
    - [i](#6b/a/i)
      - [Solution](#6b/a/i/solution)
    - [ii](#6b/a/ii)
      - [Solution](#6b/a/ii/solution)
    - [iii](#6b/a/iii)
      - [Solution](#6b/a/iii/solution)
  - [b](#6b/b)
    - [Solution](#6b/b/solution)
- [7B](#7b)
  - [a](#7b/a)
    - [Solution](#7b/a/solution)
  - [b](#7b/b)
    - [Solution](#7b/b/solution)
  - [c](#7b/c)
    - [Solution](#7b/c/solution)
  - [d](#7b/d)
    - [Solution](#7b/d/solution)
  - [e](#7b/e)
    - [Solution](#7b/e/solution)
- [8B](#8b)
  - [Solution](#8b/solution)
- [9D](#9d)
  - [a](#9d/a)
    - [Solution](#9d/a/solution)
  - [b](#9d/b)
    - [Solution](#9d/b/solution)
  - [c](#9d/c)
    - [Solution](#9d/c/solution)
- [10D](#10d)
  - [Solution](#10d/solution)
- [11D](#11d)
  - [a](#11d/a)
    - [Solution](#11d/a/solution)
  - [b](#11d/b)
    - [Solution](#11d/b/solution)
  - [c](#11d/c)
    - [Solution](#11d/c/solution)
  - [d](#11d/d)
    - [Solution](#11d/d/solution)
- [12D](#12d)
  - [Solution](#12d/solution)

## 1B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1b/a">a</h3>

↑ **Parent:** [1B](#1b)

<h4 id="1b/a/i">i</h4>

↑ **Parent:** [A](#1b/a)

<h5 id="1b/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1b/a/i)

The [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
|a-b|=|(a-z)+(z-b)|\leq |z-a|+|z-b|.
$$

**Hence the left-hand side of the proposed equation is always at least $|a-b|$. There are no solutions when $c<|a-b|$.**

<h4 id="1b/a/ii">ii</h4>

↑ **Parent:** [A](#1b/a)

<h5 id="1b/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1b/a/ii)

Equality in the [triangle inequality](../../../topological-analysis.md#triangle-inequality) holds exactly when the two displacement vectors $a-z$ and $z-b$ point in the same direction. Thus $z$ lies on the closed line segment joining $a$ and $b$. Conversely, every point of that segment satisfies

$$
|z-a|+|z-b|=|a-b|.
$$

The solution set is therefore precisely that segment in the [complex plane](../../../complex-analysis.md#complex-plane).

<h4 id="1b/a/iii">iii</h4>

↑ **Parent:** [A](#1b/a)

<h5 id="1b/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1b/a/iii)

By the focal definition of an [ellipse](../../../geometry-and-topology.md#ellipse), the solution set is the ellipse with foci $a$ and $b$. Its centre is $(a+b)/2$, its major axis lies along the line through the foci, and its semiaxes are

$$
\frac c2,\qquad \frac12\sqrt{c^2-|a-b|^2}.
$$

The sketch is consequently a [nondegenerate ellipse](../../../geometry-and-topology.md#nondegenerate-ellipse) symmetric about both the [focal line](../../../geometry-and-topology.md#focal-line) and its [perpendicular bisector](../../../geometry-and-topology.md#perpendicular-bisector).

<h3 id="1b/b">b</h3>

↑ **Parent:** [1B](#1b)

<h4 id="1b/b/i">i</h4>

↑ **Parent:** [B](#1b/b)

<h5 id="1b/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1b/b/i)

The required [root of unity](../../../algebra.md#root-of-unity) is

$$
\omega=e^{2\pi i/3}=-\frac12+\frac{\sqrt3}{2}i,
$$

so

$$
1+\omega=\frac12+\frac{\sqrt3}{2}i=e^{i\pi/3}.
$$

Therefore

$$
(1+\omega)^{10}=e^{10\pi i/3}=e^{4\pi i/3}
=\boxed{-\frac12-\frac{\sqrt3}{2}i}.
$$

<h4 id="1b/b/ii">ii</h4>

↑ **Parent:** [B](#1b/b)

<h5 id="1b/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1b/b/ii)

The logarithms of $1+\omega=e^{i\pi/3}$ are

$$
i\left(\frac\pi3+2\pi k\right),\qquad k\in\mathbb Z.
$$

The definition of [complex exponentiation](../../../analysis.md#complex-exponentiation) therefore gives all values as

$$
\exp\!\left[
i(1+\omega)\left(\frac\pi3+2\pi k\right)
\right].
$$

Since $1+\omega=\tfrac12+i\tfrac{\sqrt3}{2}$, these can be written

$$
\boxed{
(-1)^k e^{-\sqrt3\pi(k+1/6)}e^{i\pi/6}},
\qquad k\in\mathbb Z.
$$

## 2B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2b/a">a</h3>

↑ **Parent:** [2B](#2b)

<h4 id="2b/a/i">i</h4>

↑ **Parent:** [A](#2b/a)

<h5 id="2b/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2b/a/i)

Taking [determinants](../../../linear-algebra.md#determinant) of $M^TJM=J$ gives

$$
\det(M)^2\det J=\det J.
$$

Since $\det J=-1\ne0$, one has $\det(M)^2=1$, and hence

$$
\boxed{\det M=1\quad\text{or}\quad\det M=-1}.
$$

Both values occur, for example for $M=I$ and $M=\operatorname{diag}(1,-1)$.

<h4 id="2b/a/ii">ii</h4>

↑ **Parent:** [A](#2b/a)

<h5 id="2b/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2b/a/ii)

If $M_1^TJM_1=J$ and $M_2^TJM_2=J$, then [matrix multiplication](../../../vector-space.md#matrix-multiplication) and the transpose rule give

$$
(M_1M_2)^TJ(M_1M_2)
=M_2^T(M_1^TJM_1)M_2
=M_2^TJM_2=J.
$$

Thus the product also satisfies the equation.

The equation and part (i) imply that $M_1$ is invertible. Multiplying  
$M_1^TJM_1=J$ on the left by $(M_1^{-1})^T$ and on the right by $M_1^{-1}$ gives

$$
(M_1^{-1})^TJ M_1^{-1}=J.
$$

**Hence the set of solutions is closed under products and [matrix inverses](../../../linear-algebra.md#matrix-inverse).**

<h3 id="2b/b">b</h3>

↑ **Parent:** [2B](#2b)

<h4 id="2b/b/solution">Solution</h4>

↑ **Parent:** [B](#2b/b)

Write

$$
M=\begin{pmatrix}p&q\\r&s\end{pmatrix}.
$$

The first column has unit length for the indefinite quadratic form:

$$
p^2-r^2=1.
$$

Because $p=M_{11}>0$, there is a unique $u\in\mathbb R$ such that

$$
p=\cosh u,\qquad r=\sinh u.
$$

The two columns are orthogonal for the same form and the second has squared length $-1$:

$$
pq-rs=0,\qquad q^2-s^2=-1.
$$

The vectors with these properties are

$$
(q,s)=\pm(\sinh u,\cosh u).
$$

Using the [hyperbolic cosine](../../../calculus.md#hyperbolic-cosine) and [hyperbolic sine](../../../calculus.md#hyperbolic-sine), the two possible families are therefore

$$
\boxed{
\begin{pmatrix}\cosh u&\sinh u\\\sinh u&\cosh u\end{pmatrix},
\qquad
\begin{pmatrix}\cosh u&-\sinh u\\\sinh u&-\cosh u\end{pmatrix}},
\qquad u\in\mathbb R.
$$

## 3D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3d/solution">Solution</h3>

↑ **Parent:** [3D](#3d)

The [alternating series test](../../../real-analysis.md#alternating-series-test) says that if $a_n\geq0$ decreases to $0$, then

$$
\sum_{n=1}^{\infty}(-1)^na_n
$$

converges. Taking $a_n=n^{-1/2}$ proves convergence of the given series.

It is not [absolute convergence](../../../real-analysis.md#absolute-convergence), because the series of absolute values is the [p-series](../../../real-analysis.md#p-series)

$$
\sum_{n=1}^{\infty}\frac1{\sqrt n},
$$

which diverges since $p=1/2\leq1$. Thus the original series has [conditional convergence](../../../real-analysis.md#conditional-convergence).

For an explicit divergent [rearrangement of a series](../../../real-analysis.md#rearrangement-of-a-series), take unused positive terms, which are the even-indexed terms, until the partial sum exceeds $1$, then take the first unused negative term. Next take positive terms until the sum exceeds $2$, then the next unused negative term, and continue. Both the positive and negative subseries have infinite total magnitude, so this procedure uses every term. The negative term inserted at stage $m$ tends to zero, while the preceding partial sum exceeds $m$; consequently these rearranged partial sums tend to $+\infty$. This is a divergent series with exactly the prescribed terms.

## 4D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4d/solution">Solution</h3>

↑ **Parent:** [4D](#4d)

For the sum $F=f+g$:

- In case (a), **yes**. If $F$ were [differentiable](../../../analysis.md#differentiable-function) at $a$, then $g=F-f$ would be differentiable there, contrary to the hypothesis.
- In case (b), **no**. Take$$
  f(x)=|x-a|,\qquad g(x)=-|x-a|.
  $$

  Both are continuous and nondifferentiable at $a$, but $F=0$ is differentiable.

For the product $G=fg$, the answer is **no** in both cases:

- For case (a), take $f(x)=x-a$ and $g(x)=|x-a|$. Then $f$ is differentiable at $a$, $g$ is not, but$$
  G(x)=(x-a)|x-a|
  $$

  has derivative $0$ at $a$.
- For case (b), take $f(x)=g(x)=|x-a|$. Neither factor is differentiable at $a$, whereas$$
  G(x)=(x-a)^2
  $$

  is differentiable.

Every displayed $f$ and $g$ is a [continuous function](../../../calculus.md#continuous-function) and is nonzero at points arbitrarily close to $a$, so the extra condition in the question is satisfied.

## 5B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5b/a">a</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/a/i">i</h4>

↑ **Parent:** [A](#5b/a)

<h5 id="5b/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5b/a/i)

For $A=(A_1,A_2,A_3)$ and $B=(B_1,B_2,B_3)$, the scalar product is the [inner product](../../../linear-algebra.md#inner-product)

$$
A\mathbin{\cdot}B=A_1B_1+A_2B_2+A_3B_3.
$$

The [cross product](../../../vector-space.md#cross-product) is

$$
A\mathbin{\times}B
=(A_2B_3-A_3B_2,,
A_3B_1-A_1B_3,,
A_1B_2-A_2B_1).
$$

It is perpendicular to both vectors and has magnitude $|A||B|\sin\theta$.

<h4 id="5b/a/ii">ii</h4>

↑ **Parent:** [A](#5b/a)

<h5 id="5b/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5b/a/ii)

The [vector triple product](../../../calculus.md#vector-triple-product) identity gives

$$
\boxed{A\times(B\times C)
=B(A\cdot C)-C(A\cdot B)}.
$$

Applying the same identity after reversing the outer cross product gives

$$
\boxed{(A\times B)\times C
=B(A\cdot C)-A(B\cdot C)}.
$$

The formulas differ because the cross product is not associative.

<h4 id="5b/a/iii">iii</h4>

↑ **Parent:** [A](#5b/a)

<h5 id="5b/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5b/a/iii)

Let

$$
\Delta=A\cdot(B\times C).
$$

Linear independence implies that the [scalar triple product](../../../linear-algebra.md#scalar-triple-product) $Delta$ is nonzero. Applying the vector triple-product formulas to $(A\times B)\times(C\times D)$ recovers the coefficients of $D$ in the basis $A,B,C$. Equivalently, the [reciprocal basis](../../../linear-algebra.md#reciprocal-basis) to $A,B,C$ is

$$
\frac{B\times C}{\Delta},\qquad
\frac{C\times A}{\Delta},\qquad
\frac{A\times B}{\Delta}.
$$

Taking scalar products with $D$ therefore yields

$$
\boxed{
D=
\frac{D\cdot(B\times C)}{\Delta}A
+\frac{D\cdot(C\times A)}{\Delta}B
+\frac{D\cdot(A\times B)}{\Delta}C}.
$$

<h3 id="5b/b">b</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/b/solution">Solution</h4>

↑ **Parent:** [B](#5b/b)

Because the sphere passes through the origin and has centre $P$, its radius is $|P|$. A point $X$ lies on it exactly when

$$
|X-P|^2=|P|^2,
$$

or equivalently

$$
2P\cdot X=|X|^2.
$$

With $P=\alpha A+\beta B+\gamma C$, the three required equations are the [Gram matrix](../../../linear-algebra.md#gram-matrix) system

$$
\begin{pmatrix}
A\cdot A&A\cdot B&A\cdot C\\
B\cdot A&B\cdot B&B\cdot C\\
C\cdot A&C\cdot B&C\cdot C
\end{pmatrix}
\begin{pmatrix}\alpha\\\beta\\\gamma\end{pmatrix}
=\frac12
\begin{pmatrix}|A|^2\\|B|^2\\|C|^2\end{pmatrix}.
$$

For the specified vectors this becomes

$$
\alpha+\beta=\frac12,\qquad
\alpha+2\beta+\gamma=1,\qquad
\beta+5\gamma=\frac52.
$$

Thus

$$
\alpha=\frac12,\qquad\beta=0,\qquad\gamma=\frac12,
$$

and the centre is

$$
\boxed{P=\frac12A+\frac12C
=\left(\frac12,\frac12,1\right)}.
$$

## 6B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6b/a">a</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/a/i">i</h4>

↑ **Parent:** [A](#6b/a)

<h5 id="6b/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6b/a/i)

An anticlockwise [rotation matrix](../../../linear-algebra.md#rotation-matrix) and reflection in the $x$-axis are

$$
\boxed{
R=\begin{pmatrix}\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta\end{pmatrix}},
\qquad
\boxed{
M=\begin{pmatrix}1&0\\0&-1\end{pmatrix}}.
$$

The columns of $R$ are the images of the standard coordinate vectors, while $M(x,y)^T=(x,-y)^T$.

<h4 id="6b/a/ii">ii</h4>

↑ **Parent:** [A](#6b/a)

<h5 id="6b/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6b/a/ii)

Direct multiplication gives

$$
MRM=
\begin{pmatrix}\cos\theta&\sin\theta\\
-\sin\theta&\cos\theta\end{pmatrix}
=R^{-1}.
$$

Hence

$$
\boxed{MRM=R^a\quad\text{with }a=-1}.
$$

This is the defining conjugation relation between a rotation and reflection in a [dihedral group](../../../finite-group-theory.md#dihedral-group).

<h4 id="6b/a/iii">iii</h4>

↑ **Parent:** [A](#6b/a)

<h5 id="6b/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6b/a/iii)

**No.** Every power $R^a$ has [determinant](../../../linear-algebra.md#determinant) $1$, whereas

$$
\det(MR^b)=\det M\det(R^b)=-1.
$$

Matrices with different determinants cannot be equal.

<h3 id="6b/b">b</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/b/solution">Solution</h4>

↑ **Parent:** [B](#6b/b)

The relations

$$
M^2=I,\qquad R^n=I,\qquad MRM=R^{-1}
$$

imply $RM=MR^{-1}$. Moving every occurrence of $M$ to the left and reducing exponents therefore puts every word into one of the normal forms

$$
R^j\quad\text{or}\quad MR^j,
\qquad 0\leq j<n.
$$

Explicitly, with $\theta=2\pi/n$,

$$
R^j=
\begin{pmatrix}
\cos(j\theta)&-\sin(j\theta)\\
\sin(j\theta)&\cos(j\theta)
\end{pmatrix},
$$

and

$$
MR^j=
\begin{pmatrix}
\cos(j\theta)&-\sin(j\theta)\\
-\sin(j\theta)&-\cos(j\theta)
\end{pmatrix}.
$$

The $n$ rotations are distinct. The $n$ reflected matrices are also distinct, and no reflected matrix equals a rotation because their determinants are $-1$ and $1$, respectively. Hence there are exactly

$$
\boxed{2n}
$$

matrices, forming the [dihedral group](../../../finite-group-theory.md#dihedral-group).

## 7B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7b/a">a</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/a/solution">Solution</h4>

↑ **Parent:** [A](#7b/a)

Let $Av=\lambda v$ for a nonzero eigenvector $v$ of the [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) $A$. Hermitian symmetry of the [inner product](../../../linear-algebra.md#inner-product) gives

$$
\lambda\lVert v\rVert^2
=(v,Av)=(Av,v)
=\overline\lambda\lVert v\rVert^2.
$$

Since $lVert v\rVert^2>0$, $lambda=\overline\lambda$, so every eigenvalue is real.

<h3 id="7b/b">b</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/b/solution">Solution</h4>

↑ **Parent:** [B](#7b/b)

For an [orthogonal projection matrix](../../../linear-algebra.md#orthogonal-projection-matrix) $P=P^\dagger=P^2$,

$$
(x,Px)
=x^\dagger P^\dagger Px
=(Px)^\dagger(Px)
=\lVert Px\rVert^2\geq0.
$$

**Thus $P$ is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix).**

<h3 id="7b/c">c</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/c/solution">Solution</h4>

↑ **Parent:** [C](#7b/c)

Set

$$
v_1=Pv,\qquad v_0=(I-P)v.
$$

Then $v=v_0+v_1$, and [idempotence](../../../commutative-algebra.md#idempotent) gives

$$
Pv_0=P(I-P)v=(P-P^2)v=0,\qquad
Pv_1=P^2v=Pv=v_1.
$$

Moreover,

$$
(v_0,v_1)
=((I-P)v,Pv)
=(v,(I-P)P v)=0,
$$

because both $P$ and $I-P$ are Hermitian. This is the orthogonal decomposition into the kernel and image of the projection.

<h3 id="7b/d">d</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/d/solution">Solution</h4>

↑ **Parent:** [D](#7b/d)

Put $H=A-B$. This is a nonzero [Hermitian matrix](../../../hilbert-space.md#hermitian-operator). By the [finite-dimensional spectral theorem](../../../linear-operator-theory.md#finite-dimensional-spectral-theorem), it has a unit eigenvector $v$ with a nonzero real eigenvalue $lambda$. Define the rank-one [orthogonal projection matrix](../../../linear-algebra.md#orthogonal-projection-matrix)

$$
P=vv^\dagger.
$$

The cyclic property of the [matrix trace](../../../linear-algebra.md#matrix-trace) gives

$$
\operatorname{Tr}(PA)-\operatorname{Tr}(PB)
=\operatorname{Tr}(PH)
=\operatorname{Tr}(vv^\dagger H)
=v^\dagger Hv
=\lambda\ne0.
$$

**Hence this $P$ distinguishes $A$ and $B$ through the required traces.**

<h3 id="7b/e">e</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/e/solution">Solution</h4>

↑ **Parent:** [E](#7b/e)

**No.** Consider the two orthogonal projections

$$
P=\begin{pmatrix}1&0\\0&0\end{pmatrix},
\qquad
Q=\frac12\begin{pmatrix}1&1\\1&1\end{pmatrix}.
$$

Their product is

$$
PQ=\frac12\begin{pmatrix}1&1\\0&0\end{pmatrix}.
$$

For $x=(-1,2)^T$,

$$
x^\dagger PQx=-\frac12<0.
$$

**Thus $PQ$ is not a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix). It is also not Hermitian; products of orthogonal projections need not remain orthogonal projections unless the factors commute.**

## 8B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8b/solution">Solution</h3>

↑ **Parent:** [8B](#8b)

For the standard basis vector $e_j$, matrix multiplication selects the $j$th column, so

$$
Me_j=c_j.
$$

Consequently

$$
(PM)e_j=P(Me_j)=Pc_j,
$$

and the columns of $PM$ are $Pc_1,\ldots,Pc_n$.

Suppose first that $v,Av,\ldots,A^{n-1}v$ are linearly independent, and define

$$
S=\begin{pmatrix}v&Av&\cdots&A^{n-1}v\end{pmatrix}.
$$

Then $S$ is invertible. The first $n-1$ columns of $AS$ are the last $n-1$ columns of $S$. By the [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem),

$$
A^nv=-a_0v-a_1Av-\cdots-a_{n-1}A^{n-1}v.
$$

This is exactly the last-column rule for the [companion matrix](../../../linear-operator-theory.md#companion-matrix) $C$, so

$$
AS=SC,\qquad S^{-1}AS=C.
$$

Conversely, suppose $S^{-1}AS=C$, or $AS=SC$, and write the columns of $S$ as $s_1,\ldots,s_n$. Comparing the first $n-1$ columns gives

$$
As_j=s_{j+1}\qquad(1\leq j<n).
$$

Hence

$$
s_j=A^{j-1}s_1.
$$

Since $S$ is invertible, its columns are linearly independent. Taking $v=s_1$ therefore makes

$$
v,Av,\ldots,A^{n-1}v
$$

linearly independent. Thus $A$ is similar to $C$ exactly when it has the stated [cyclic vector](../../../linear-operator-theory.md#cyclic-vector).

## 9D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9d/a">a</h3>

↑ **Parent:** [9D](#9d)

<h4 id="9d/a/solution">Solution</h4>

↑ **Parent:** [A](#9d/a)

Suppose $a_n\to L$. Given $\varepsilon>0$, choose $N$ such that $|a_k-L|<\varepsilon/2$ for $k>N$. Then

$$
\left|\frac1n\sum_{k=1}^na_k-L\right|
\leq
\frac1n\sum_{k=1}^N|a_k-L|
+\frac1n\sum_{k=N+1}^n|a_k-L|.
$$

The first term tends to zero because its numerator is fixed, and the second is at most $\varepsilon/2$. Thus the [Cesaro mean](../../../real-analysis.md#cesaro-mean) tends to $L$.

The converse is false. For $a_n=(-1)^n$, the Cesaro means tend to $0$, while the original [sequence](../../../real-analysis.md#sequence) alternates between $-1$ and $1$ and does not converge.

<h3 id="9d/b">b</h3>

↑ **Parent:** [9D](#9d)

<h4 id="9d/b/solution">Solution</h4>

↑ **Parent:** [B](#9d/b)

First suppose $x_n\to L>0$. Continuity of the [natural logarithm](../../../calculus.md#natural-logarithm) gives $\log x_n\to\log L$. Part (a), applied to this sequence, yields

$$
\frac1n\sum_{k=1}^n\log x_k\longrightarrow\log L.
$$

Applying the continuous [exponential function](../../../calculus.md#exponential-function),

$$
\sqrt[n]{x_1x_2\cdots x_n}
=\exp\!\left(\frac1n\sum_{k=1}^n\log x_k\right)
\longrightarrow L.
$$

If $L=0$, then for every $\varepsilon>0$ all sufficiently late $x_k$ are below $\varepsilon$. Splitting off the fixed initial product shows that the limsup of the geometric means is at most $\varepsilon$; hence it is zero. This proves the [geometric mean of a sequence](../../../real-analysis.md#geometric-mean-of-a-sequence) result in all cases.

Now suppose

$$
r_n=\frac{x_n}{x_{n-1}}\longrightarrow r.
$$

The telescoping product is

$$
x_n=x_0\prod_{k=1}^nr_k.
$$

Therefore

$$
\sqrt[n]{x_n}
=x_0^{1/n}\sqrt[n]{r_1r_2\cdots r_n}
\longrightarrow 1\cdot r,
$$

and so

$$
\boxed{\lim_{n\to\infty}\sqrt[n]{x_n}
=\lim_{n\to\infty}\frac{x_n}{x_{n-1}}}.
$$

<h3 id="9d/c">c</h3>

↑ **Parent:** [9D](#9d)

<h4 id="9d/c/solution">Solution</h4>

↑ **Parent:** [C](#9d/c)

A [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) is a sequence $(x_n)$ such that for every $\varepsilon>0$ there is $N$ for which

$$
m,n\geq N\quad\Longrightarrow\quad |x_m-x_n|<\varepsilon.
$$

The general principle of convergence, or [completeness of the real numbers](../../../real-analysis.md#completeness-of-the-real-numbers), states that a real sequence converges if and only if it is Cauchy.

For the final claim, let $m=\lfloor n/2\rfloor$. Since $(a_n)$ is decreasing and positive,

$$
0\leq (n-m)a_n
\leq\sum_{k=m+1}^na_k.
$$

Because the [series](../../../real-analysis.md#series-mathematics) $\sum a_k$ converges, its tails tend to zero. Also $n-m\geq n/2$, so

$$
0\leq na_n
\leq2\sum_{k=m+1}^na_k
\longrightarrow0.
$$

The squeeze theorem gives

$$
\boxed{na_n\to0}.
$$

## 10D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10d/solution">Solution</h3>

↑ **Parent:** [10D](#10d)

Let $f:[a,b]\to\mathbb R$ be continuous. If it were unbounded, one could choose $x_n\in[a,b]$ with $|f(x_n)|>n$. The [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) gives a subsequence $x_{n_j}\to x\in[a,b]$, but continuity would then give $f(x_{n_j})\to f(x)$, contradicting unboundedness.

Now let $M=\sup f([a,b])$. Choose $x_n$ with $f(x_n)>M-1/n$. A convergent subsequence and continuity give $f(x)=M$ at its limit. Applying the same argument to $-f$ shows that the infimum is attained. This proves the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem) on a closed bounded interval.

The function

$$
\phi(x)=x\qquad(0<x<1)
$$

is continuous and bounded, but attains neither its infimum $0$ nor its supremum $1$. For the second example, enumerate the rationals in $[0,1]$ as $(q_n)$ and set

$$
\psi(x)=
\begin{cases}
n,&x=q_n,\\
0,&x\notin\mathbb Q.
\end{cases}
$$

Every [nondegenerate interval](../../../topology.md#nondegenerate-interval) contains infinitely many [rational numbers](../../../number-theory.md#rational-number), hence some $q_n$ with arbitrarily large $n$; therefore $\psi$ is [unbounded](../../../function.md#unbounded-function) on every such interval.

For the running extrema, compactness lets us write

$$
m(x)=\min_{a\leq\xi\leq x}f(\xi),\qquad
M(x)=\max_{a\leq\xi\leq x}f(\xi).
$$

The function $f$ is [uniformly continuous](../../../topological-analysis.md#uniform-continuity) on $[a,b]$. Given $\varepsilon>0$, choose $\delta>0$ such that $|f(u)-f(v)|<\varepsilon$ whenever $|u-v|<\delta$. If $x<y$ and $y-x<\delta$, every new value $f(\xi)$ with $x\leq\xi\leq y$ is at most $f(x)+\varepsilon\leq M(x)+\varepsilon$. Since $M(y)\geq M(x)$,

$$
0\leq M(y)-M(x)\leq\varepsilon.
$$

Interchanging $x,y$ handles the other order. Applying this argument to $-f$ proves continuity of $m$ as well.

Finally fix $T>0$ and put $h(x)=g(x+T)-g(x)$. For each positive integer $n$, there must be some $x_n>n$ with $|h(x_n)|<1/n$. Otherwise, for some $n$ the continuous function $h$ would satisfy $|h(x)|\geq1/n$ on the interval $(n,\infty)$. By the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem), $h$ would have a constant sign there. The values

$$
g(x),g(x+T),g(x+2T),\ldots
$$

would then increase or decrease by at least $1/n$ at every step, contradicting boundedness of $g$. Thus $x_n\to\infty$ and

$$
\boxed{g(x_n+T)-g(x_n)\to0}.
$$

## 11D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11d/a">a</h3>

↑ **Parent:** [11D](#11d)

<h4 id="11d/a/solution">Solution</h4>

↑ **Parent:** [A](#11d/a)

[Rolle theorem](../../../calculus.md#rolle-theorem): if $f$ is continuous on $[a,b]$, differentiable on $(a,b)$, and $f(a)=f(b)$, then $f'(c)=0$ for some $c\in(a,b)$. Indeed, the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem) gives a maximum and minimum. If both occur only at the endpoints then $f$ is constant; otherwise an interior extremum $c$ satisfies $f'(c)=0$ by comparing the two-sided difference quotients.

[Mean value theorem](../../../calculus.md#mean-value-theorem): if $f$ is continuous on $[a,b]$ and differentiable on $(a,b)$, then some $c\in(a,b)$ satisfies

$$
f'(c)=\frac{f(b)-f(a)}{b-a}.
$$

Apply Rolle's theorem to

$$
h(x)=f(x)-f(a)-\frac{f(b)-f(a)}{b-a}(x-a),
$$

which has $h(a)=h(b)=0$.

<h3 id="11d/b">b</h3>

↑ **Parent:** [11D](#11d)

<h4 id="11d/b/solution">Solution</h4>

↑ **Parent:** [B](#11d/b)

Let

$$
m=\frac{f(b)-f(a)}{b-a},\qquad
h(x)=f(x)-f(a)-m(x-a).
$$

Then $h(a)=h(b)=0$. Since $f$ is not linear, $h(c)\ne0$ for some $c\in(a,b)$. If $h(c)>0$, the [mean value theorem](../../../calculus.md#mean-value-theorem) on $[a,c]$ gives a point $\xi$ with

$$
h'(\xi)=\frac{h(c)-h(a)}{c-a}>0.
$$

If $h(c)<0$, apply it on $[c,b]$ to obtain

$$
h'(\xi)=\frac{h(b)-h(c)}{b-c}>0.
$$

In either case $h'=f'-m$, and therefore

$$
\boxed{f'(\xi)>\frac{f(b)-f(a)}{b-a}}.
$$

<h3 id="11d/c">c</h3>

↑ **Parent:** [11D](#11d)

<h4 id="11d/c/solution">Solution</h4>

↑ **Parent:** [C](#11d/c)

**No.** On $[-1,1]$, take

$$
f(x)=x^3,\qquad \xi=0.
$$

Then $f'(0)=0$. For every $x_1<0<x_2$,

$$
\frac{f(x_2)-f(x_1)}{x_2-x_1}
=x_2^2+x_1x_2+x_1^2.
$$

This quadratic expression is strictly positive: it equals

$$
\left(x_2+\frac{x_1}{2}\right)^2+\frac34x_1^2.
$$

**Thus no chord with endpoints on opposite sides of $\xi$ has slope $f'(\xi)=0$.**

<h3 id="11d/d">d</h3>

↑ **Parent:** [11D](#11d)

<h4 id="11d/d/solution">Solution</h4>

↑ **Parent:** [D](#11d/d)

Set

$$
H(x)=(g(b)-g(a))f(x)-(f(b)-f(a))g(x).
$$

Its endpoint values are equal. [Rolle theorem](../../../calculus.md#rolle-theorem) therefore supplies $\xi\in(a,b)$ with

$$
(g(b)-g(a))f'(\xi)
=(f(b)-f(a))g'(\xi). \qquad (1)
$$

If $g'(\xi)=0$, then (1) and $g(b)\ne g(a)$ force $f'(\xi)=0$, contrary to the hypothesis. Hence $g'(\xi)\ne0$, and division in (1) gives

$$
\boxed{
\frac{f(b)-f(a)}{g(b)-g(a)}
=\frac{f'(\xi)}{g'(\xi)}}.
$$

The condition is necessary. On $[0,2\pi]$, let

$$
f(x)=\sin x,\qquad
g(x)=\sin x+\frac{x}{4}+\frac{\sin2x}{8}.
$$

Here $g(2\pi)-g(0)=\pi/2$ while $f(2\pi)-f(0)=0$, so the endpoint ratio is zero. But

$$
f'(x)=\cos x,\qquad
g'(x)=\cos x\left(1+\frac12\cos x\right).
$$

Where $g'(x)\ne0$, their ratio is $1/(1+\tfrac12\cos x)$ and is never zero. At the remaining points both derivatives vanish, so the derivative ratio is undefined. Thus the conclusion fails when simultaneous zeros are allowed.

## 12D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12d/solution">Solution</h3>

↑ **Parent:** [12D](#12d)

It is enough to treat an increasing function; replacing $f$ by $-f$ handles a decreasing one. Let $\mathcal R$ be the common refinement of dissections $\mathcal D$ and $\mathcal D'$. Refinement raises lower [Darboux sums](../../../real-analysis.md#darboux-sum) and lowers upper ones, so

$$
L_{\mathcal D}(f)\leq L_{\mathcal R}(f)
\leq U_{\mathcal R}(f)\leq U_{\mathcal D'}(f).
$$

For the uniform dissection $\mathcal D_n=\{k/n:0\leq k\leq n\}$, monotonicity gives the telescoping difference

$$
U_{\mathcal D_n}(f)-L_{\mathcal D_n}(f)
=\frac1n\sum_{k=1}^n
\left(f\left(\frac kn\right)-f\left(\frac{k-1}{n}\right)\right)
=\frac{f(1)-f(0)}n.
$$

This can be made smaller than any $\varepsilon>0$, so the [Riemann integrability criterion](../../../real-analysis.md#riemann-integrability-criterion) proves that $f$ is integrable.

The integral lies between the lower and upper sums, and the displayed sum in the question is the right-endpoint upper sum. Hence the generally valid sharp estimate is

$$
\boxed{
\left|\int_0^1f(x)\,dx
-\frac1n\sum_{k=1}^nf\left(\frac kn\right)\right|
\leq\frac{|f(1)-f(0)|}{n}}. \qquad (1)
$$

The strict inequality printed in the question is false for arbitrary monotone functions: if $f(x)=0$ for $x<1$ and $f(1)=1$, the two sides of (1) are both $1/n$.

For the final claim, write

$$
\Delta_n
=\sum_{k=1}^n\int_{(k-1)/n}^{k/n}
\left(F(x)-F\left(\frac kn\right)\right)dx.
$$

Since $F'$ is continuous on a compact interval, it is uniformly continuous. Uniformly for $0\leq t\leq1$,

$$
F\left(\frac{k-1+t}{n}\right)-F\left(\frac kn\right)
=-\frac{1-t}{n}F'\left(\frac kn\right)+o\left(\frac1n\right).
$$

After the substitution $x=(k-1+t)/n$, summing the uniform errors gives

$$
\Delta_n
=-\frac1{2n^2}\sum_{k=1}^nF'\left(\frac kn\right)
+o\left(\frac1n\right).
$$

The right-hand sum is a [Riemann integral](../../../real-analysis.md#riemann-integral), so the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) yields

$$
\lim_{n\to\infty}n\Delta_n
=-\frac12\int_0^1F'(x)\,dx
=\boxed{\frac{F(0)-F(1)}2}.
$$

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
