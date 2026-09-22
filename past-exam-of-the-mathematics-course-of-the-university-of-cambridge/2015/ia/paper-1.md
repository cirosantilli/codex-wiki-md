# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2015/PaperIA_1.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2015/PaperIA_1.pdf)

**Table of contents**

- [1B](#1b)
  - [a](#1b/a)
    - [Solution](#1b/a/solution)
  - [b](#1b/b)
    - [Solution](#1b/b/solution)
- [2C](#2c)
  - [Solution](#2c/solution)
- [3F](#3f)
  - [a](#3f/a)
    - [Solution](#3f/a/solution)
  - [b](#3f/b)
    - [Solution](#3f/b/solution)
  - [c](#3f/c)
    - [Solution](#3f/c/solution)
- [4E](#4e)
  - [Solution](#4e/solution)
- [5B](#5b)
  - [i](#5b/i)
    - [Solution](#5b/i/solution)
  - [ii](#5b/ii)
    - [Solution](#5b/ii/solution)
  - [iii](#5b/iii)
    - [Solution](#5b/iii/solution)
- [6C](#6c)
  - [i](#6c/i)
    - [Solution](#6c/i/solution)
  - [ii](#6c/ii)
    - [Solution](#6c/ii/solution)
- [7A](#7a)
  - [i](#7a/i)
    - [Solution](#7a/i/solution)
  - [ii](#7a/ii)
    - [Solution](#7a/ii/solution)
  - [iii](#7a/iii)
    - [Solution](#7a/iii/solution)
  - [iv](#7a/iv)
    - [Solution](#7a/iv/solution)
- [8A](#8a)
  - [a](#8a/a)
    - [i](#8a/a/i)
      - [Solution](#8a/a/i/solution)
    - [ii](#8a/a/ii)
      - [Solution](#8a/a/ii/solution)
    - [iii](#8a/a/iii)
      - [Solution](#8a/a/iii/solution)
    - [iv](#8a/a/iv)
      - [Solution](#8a/a/iv/solution)
    - [v](#8a/a/v)
      - [Solution](#8a/a/v/solution)
  - [b](#8a/b)
    - [Solution](#8a/b/solution)
  - [c](#8a/c)
    - [Solution](#8a/c/solution)
  - [d](#8a/d)
    - [Solution](#8a/d/solution)
- [9F](#9f)
  - [Solution](#9f/solution)
- [10D](#10d)
  - [a](#10d/a)
    - [Solution](#10d/a/solution)
  - [b](#10d/b)
    - [Solution](#10d/b/solution)
- [11D](#11d)
  - [i](#11d/i)
    - [Solution](#11d/i/solution)
  - [ii](#11d/ii)
    - [Solution](#11d/ii/solution)
- [12E](#12e)
  - [Solution](#12e/solution)

## 1B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1b/a">a</h3>

↑ **Parent:** [1B](#1b)

<h4 id="1b/a/solution">Solution</h4>

↑ **Parent:** [A](#1b/a)

Write $z=x+iy$. Using the [complex conjugate](../../../complex-analysis.md#complex-conjugate), the squared [complex modulus](../../../complex-analysis.md#complex-modulus) on the left is $(\alpha+\beta)^2x^2+(\alpha-\beta)^2y^2$. Squaring the equality and dividing by $(\alpha-\beta)^2$, which is nonzero, gives

$$
x^2+y^2-4\sqrt{\alpha\beta}\,x-(\alpha-\beta)^2=0.
$$

Completing the square identifies the candidate [circle](../../../topology.md#circle):

$$
\boxed{(x-2\sqrt{\alpha\beta})^2+y^2=(\alpha+\beta)^2.}
$$

Its **centre is $2\sqrt{\alpha\beta}$ on the real axis and its radius is $\alpha+\beta$** in the [complex plane](../../../complex-analysis.md#complex-plane).

It remains to exclude extraneous points introduced by squaring. On this [circle](../../../topology.md#circle), $x\geq 2\sqrt{\alpha\beta}-(\alpha+\beta)$, so the original right-hand side satisfies

$$
2\sqrt{\alpha\beta}\,x+(\alpha-\beta)^2\geq(\alpha+\beta)(\alpha+\beta-2\sqrt{\alpha\beta})>0.
$$

Thus taking the nonnegative square root recovers the original equality at every point of the [circle](../../../topology.md#circle). This is a [circle from an affine complex-modulus equation](../../../topology.md#circle-from-an-affine-complex-modulus-equation), with the sign check essential to the geometric conclusion.

<h3 id="1b/b">b</h3>

↑ **Parent:** [1B](#1b)

<h4 id="1b/b/solution">Solution</h4>

↑ **Parent:** [B](#1b/b)

Put $q=e^{i\theta}$. Since $q\ne1$, the [finite geometric series](../../../real-analysis.md#finite-geometric-series) gives

$$
\sum_{m=1}^N q^m=\frac{q(1-q^N)}{1-q}=\frac{q-1-q^{N+1}+q^N}{2(1-\cos\theta)},
$$

where the second equality multiplies numerator and denominator by $1-\overline q$. Taking imaginary parts gives the [finite trigonometric sum](../../../real-analysis.md#finite-trigonometric-sum)

$$
\boxed{\sum_{m=1}^N\sin(m\theta)=\frac{\sin\theta+\sin(N\theta)-\sin((N+1)\theta)}{2(1-\cos\theta)}.}
$$

Taking real parts of the same [finite geometric series](../../../real-analysis.md#finite-geometric-series) gives

$$
\boxed{\sum_{m=1}^N\cos(m\theta)=\frac{\cos\theta-1+\cos(N\theta)-\cos((N+1)\theta)}{2(1-\cos\theta)}.}
$$

The denominator is nonzero by the restriction on $\theta$. Equivalently, these [finite trigonometric sums](../../../real-analysis.md#finite-trigonometric-sum) are $\sin(N\theta/2)\sin((N+1)\theta/2)/\sin(\theta/2)$ and $\sin(N\theta/2)\cos((N+1)\theta/2)/\sin(\theta/2)$, respectively.

## 2C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2c/solution">Solution</h3>

↑ **Parent:** [2C](#2c)

Denote the four displayed matrices, from left to right, by $T_1,T_2,T_3,T_4$. An [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) has an orthonormal set of columns, equivalently $T^TT=I$. Direct column [dot products](../../../linear-algebra.md#dot-product) give $T_j^TT_j=I$ for $j=1,2,4$. The first column of $T_3$ has squared [Euclidean norm](../../../functional-analysis.md#euclidean-norm) $(1+6+1)/6=4/3$, so **the third matrix is the unique nonorthogonal matrix**.

For $T_1$, the [determinant](../../../linear-algebra.md#determinant) is $1$. A nonidentity [orthogonal transformation](../../../linear-algebra.md#orthogonal-transformation) of $\mathbb R^3$ with [determinant](../../../linear-algebra.md#determinant) $1$ is a rotation: it has a fixed axis and restricts to a plane rotation on its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement). Consequently **$T_1$ is the rotation**.

For $T_2$, calculation gives

$$
\det T_2=-1,\qquad \det(T_2-I)=-\frac43.
$$

A plane [reflection](../../../linear-algebra.md#reflection-mathematics) fixes its entire plane, and therefore has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $1$. Since $T_2-I$ is invertible, $T_2$ is not a plane [reflection](../../../linear-algebra.md#reflection-mathematics). Thus **$T_2$ is the combination of a rotation and a reflection**. More explicitly, $(1,-2,0)^T$ is an [eigenvector](../../../linear-operator-theory.md#eigenvector) with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $-1$. On the perpendicular plane, $T_2$ is a rotation with $\cos\phi=2/3$, because $\operatorname{tr}T_2=-1+2\cos\phi=1/3$. This gives a [three-dimensional improper orthogonal transformation](../../../linear-algebra.md#three-dimensional-improper-orthogonal-transformation).

For $T_4$, set $n=(1,2,2)^T/3$. Then

$$
T_4=I-2nn^T.
$$

This [reflection matrix](../../../linear-algebra.md#reflection-matrix) reverses the normal $n$ and fixes every vector perpendicular to $n$. Therefore **$T_4$ is reflection in the plane $x+2y+2z=0$**. In particular, $\det T_4=-1$ and $\det(T_4-I)=0$. Finally **$T_3$ represents none of the three listed orthogonal transformations**, since each preserves the [Euclidean norm](../../../functional-analysis.md#euclidean-norm).

## 3F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3f/a">a</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/a/solution">Solution</h4>

↑ **Parent:** [A](#3f/a)

For $0<x<\pi/2$, the usual unit-circle area comparison, with angles measured in radians, gives $\sin x\leq x\leq\tan x$. Hence

$$
\cos x\leq\frac{\sin x}{x}\leq1.
$$

The [cosine](../../../geometry-and-topology.md#cosine) is a [continuous function](../../../calculus.md#continuous-function) at zero, so the [squeeze theorem](../../../calculus.md#squeeze-theorem) yields the right-hand [limit of a function](../../../calculus.md#limit-of-a-function) $1$. The quotient $\sin x/x$ is even, so the left-hand [limit of a function](../../../calculus.md#limit-of-a-function) is the same. Thus **the limit is $1$**.

<h3 id="3f/b">b</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/b/solution">Solution</h4>

↑ **Parent:** [B](#3f/b)

For $x$ sufficiently close to zero, $1+x>0$. Apply the [mean value theorem](../../../calculus.md#mean-value-theorem) to the [logarithm](../../../calculus.md#logarithm) between $1$ and $1+x$: there is a point $\xi_x$ between these endpoints with

$$
\frac{\log(1+x)}{x}=\frac1{\xi_x}.
$$

As $x\to0$ from either side, $\xi_x\to1$, so this quotient tends to $1$. The [exponential function](../../../calculus.md#exponential-function) is continuous, and therefore

$$
\boxed{\lim_{x\to0}(1+x)^{1/x}=\lim_{x\to0}\exp\!\left(\frac{\log(1+x)}x\right)=e.}
$$

The hypotheses of the [mean value theorem](../../../calculus.md#mean-value-theorem) hold because $\log t$ is continuous and differentiable for $t>0$, with derivative $1/t$.

<h3 id="3f/c">c</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/c/solution">Solution</h4>

↑ **Parent:** [C](#3f/c)

For $x>0$, the exponent $x/(1+x)$ lies in $(0,1)$, and $0\leq\cos^4x\leq1$. Consequently

$$
0\leq\frac{(1+x)^{x/(1+x)}\cos^4x}{e^x}\leq\frac{1+x}{e^x}\leq\frac{2(1+x)}{x^2}.
$$

The last inequality uses the positive-term [power series](../../../real-analysis.md#power-series) $e^x=\sum_{k\geq0}x^k/k!\geq x^2/2$ for $x>0$. The final bound tends to zero, so the [squeeze theorem](../../../calculus.md#squeeze-theorem) gives **limit $0$**.

## 4E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4e/solution">Solution</h3>

↑ **Parent:** [4E](#4e)

A complex [power series](../../../real-analysis.md#power-series) with [radius of convergence](../../../real-analysis.md#radius-of-convergence) $R$ converges absolutely at every $z$ with $|z|<R$ and diverges at every $z$ with $|z|>R$. This makes no general assertion at $|z|=R$: boundary points must be examined separately. The series always converges at $z=0$. If $R=0$, no nonzero point lies in the convergence disk; if $R=\infty$, the series converges absolutely throughout the [complex plane](../../../complex-analysis.md#complex-plane).

If $p$ is the zero polynomial, every coefficient vanishes, so **$R=\infty$**. Otherwise let $d$ be its degree and $c\ne0$ its leading coefficient. Since $p(n)=cn^d(1+o(1))$,

$$
\left|\frac{p(n+1)}{p(n)}\right|\longrightarrow1.
$$

The [ratio test](../../../real-analysis.md#ratio-test) therefore proves absolute convergence when $|z|<1$. For $|z|>1$, the terms $p(n)z^n$ do not tend to zero, so the series diverges. Thus the [polynomial-coefficient power series](../../../real-analysis.md#polynomial-coefficient-power-series) has **$R=1$ for every nonzero polynomial**. In fact, it also diverges at every $|z|=1$, because $|p(n)z^n|=|p(n)|$ does not tend to zero, whether $d=0$ or $d>0$.

## 5B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5b/i">i</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/i/solution">Solution</h4>

↑ **Parent:** [I](#5b/i)

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) in $\mathbb R^n$ is

$$
\boxed{|a\cdot b|\leq\|a\|\,\|b\|.}
$$

Here the [Euclidean norm](../../../functional-analysis.md#euclidean-norm) is induced by the [dot product](../../../linear-algebra.md#dot-product). If $b=0$, the result is immediate. If $b\ne0$, the squared [Euclidean norm](../../../functional-analysis.md#euclidean-norm) of the component of $a$ perpendicular to $b$ is nonnegative:

$$
0\leq\left\|a-\frac{a\cdot b}{\|b\|^2}b\right\|^2=\|a\|^2-\frac{(a\cdot b)^2}{\|b\|^2}.
$$

Rearrangement proves the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Equality holds precisely when $a$ and $b$ are linearly dependent, including the cases of a zero vector.

Expanding the squared [Euclidean norm](../../../functional-analysis.md#euclidean-norm) and using the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\|a+b\|^2=\|a\|^2+2a\cdot b+\|b\|^2\leq(\|a\|+\|b\|)^2.
$$

Taking nonnegative square roots gives the [triangle inequality](../../../topological-analysis.md#triangle-inequality). Applying the [triangle inequality](../../../topological-analysis.md#triangle-inequality) once more gives

$$
\boxed{\|a+b\|\leq\|a\|+\|b\|,\qquad\|a+b+c\|\leq\|a\|+\|b\|+\|c\|.}
$$

<h3 id="5b/ii">ii</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5b/ii)

Subtract the two constraints to obtain $x\cdot(a-b)=A-B$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $|A-B|\leq\|x\|\,\|a-b\|$. Since $a\ne b$, division and squaring give the [distance bound from two hyperplane constraints](../../../probability-and-statistics.md#distance-bound-from-two-hyperplane-constraints)

$$
\boxed{\|x\|^2\geq\frac{(A-B)^2}{\|a-b\|^2}.}
$$

If $a=b$ and $A\ne B$, **the intersection is empty**. If $a=b\ne0$ and $A=B$, the constraints describe the same hyperplane. Its points satisfy $\|x\|^2\geq A^2/\|a\|^2$, with equality at $x=Aa/\|a\|^2$. The fraction involving $a-b$ is undefined in this case and cannot be used.

If $a=b=0$, both equations are satisfied by every $x$ when $A=B=0$, and otherwise there is no solution. These degenerate cases distinguish an inconsistent constraint from a repeated one.

<h3 id="5b/iii">iii</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5b/iii)

Apply the [triangle inequality](../../../topological-analysis.md#triangle-inequality) to the path from $x_1$ through $y_2$ to $y_1$:

$$
\|x_1-y_1\|-\|x_1-y_2\|\leq\|y_1-y_2\|.
$$

This is one direction of the [reverse triangle inequality](../../../topological-analysis.md#reverse-triangle-inequality). A second application of the [triangle inequality](../../../topological-analysis.md#triangle-inequality), this time through $x_2$, gives

$$
\boxed{\|x_1-y_1\|-\|x_1-y_2\|\leq\|y_1-y_2\|\leq\|x_2-y_1\|+\|x_2-y_2\|.}
$$

The resulting [four-point triangle inequality](../../../topological-analysis.md#four-point-triangle-inequality) follows without any assumptions on coincidences among the four points.

## 6C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6c/i">i</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/i/solution">Solution</h4>

↑ **Parent:** [I](#6c/i)

Write a vector in the domain as $(u,v,w,t)^T$. The first and third equations defining the [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) imply $v=2\alpha u-2t$. Substitution into the second equation then gives

$$
2(\alpha-1)\bigl(t-(\alpha+1)u\bigr)=0.
$$

For $\alpha\ne1$, this forces $t=(\alpha+1)u$, $v=-2u$ and $w=3u$. Hence

$$
\boxed{\ker M_\alpha=\operatorname{span}\{(1,-2,3,\alpha+1)^T\},\qquad\operatorname{im}M_\alpha=\mathbb R^3\quad(\alpha\ne1).}
$$

The [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) has dimension one, so the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) gives rank three and proves the assertion about the [image of a linear map](../../../vector-space.md#image-of-a-linear-map). Alternatively, the minor formed from columns $2,3,4$ has [determinant](../../../linear-algebra.md#determinant) $2(\alpha-1)$, including a nonzero value at $\alpha=-1$.

For $\alpha=1$, the parameters $u,t$ are free and $v=2u-2t$, $w=-3u+3t$. Thus

$$
\boxed{\ker M_1=\operatorname{span}\{(1,2,-3,0)^T,(0,-2,3,1)^T\}.}
$$

The third row is the first row minus the second. The [image of a linear map](../../../vector-space.md#image-of-a-linear-map) is therefore contained in $y_1-y_2-y_3=0$. The first and third columns, $(1,2,-1)^T$ and $(1,0,1)^T$, are linearly independent, so the [matrix rank](../../../vector-space.md#matrix-rank) is two and this containment is equality:

$$
\boxed{\operatorname{im}M_1=\{y\in\mathbb R^3:y_1-y_2-y_3=0\}=\operatorname{span}\{(1,2,-1)^T,(1,0,1)^T\}.}
$$

This is the sole [kernel jump in a parameter-dependent linear map](../../../linear-algebra.md#kernel-jump-in-a-parameter-dependent-linear-map); there is no further exceptional case at $\alpha=-1$.

<h3 id="6c/ii">ii</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6c/ii)

Let $e_1,\ldots,e_n$ be the standard [basis](../../../vector-space.md#basis) and define $a_j=f(e_j)$. By linearity,

$$
f(x)=f\!\left(\sum_{j=1}^n x_je_j\right)=\sum_{j=1}^n x_jf(e_j)=a\cdot x.
$$

Thus every [linear functional](../../../linear-algebra.md#linear-functional) has this form. Its representing vector is unique because evaluating $a\cdot x=b\cdot x$ at each $e_j$ gives $a_j=b_j$.

For the prescribed [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map), the third listed vector is the first minus the second, so it adds no independent constraint. The first two require

$$
a_1+a_2+a_3-a_4=0,\qquad2a_1-a_2-2a_4=0.
$$

Taking $a_1=s$ and $a_4=t$ gives $a_2=2s-2t$, $a_3=-3s+3t$. Consequently **all possible representing vectors** are

$$
\boxed{a=s(1,2,-3,0)^T+t(0,-2,3,1)^T,\qquad s,t\in\mathbb R.}
$$

Conversely, every such vector is perpendicular to each of the three prescribed vectors, so its [linear functional](../../../linear-algebra.md#linear-functional) vanishes on them. This also includes the zero [linear functional](../../../linear-algebra.md#linear-functional).

## 7A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7a/i">i</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/i/solution">Solution</h4>

↑ **Parent:** [I](#7a/i)

The [characteristic polynomials](../../../linear-operator-theory.md#characteristic-polynomial), in the convention $\det(\lambda I-T)$, are

$$
\chi_A(\lambda)=(\lambda-1)(\lambda-2)^2,\qquad\chi_B(\lambda)=(\lambda-2)(\lambda-4)(\lambda-6).
$$

Solving the [eigenvalue equations](../../../linear-operator-theory.md#eigenvalue-equation) gives the complete [eigenspaces](../../../linear-operator-theory.md#eigenspace)

$$
\begin{aligned}
E_1(A)&=\operatorname{span}\{(1,1,1)^T\},\\
E_2(A)&=\{(x,y,z)^T:y=x+z\}=\operatorname{span}\{(1,0,-1)^T,(1,2,1)^T\},\\
E_2(B)&=\operatorname{span}\{(1,1,1)^T\},\\
E_4(B)&=\operatorname{span}\{(1,0,-1)^T\},\\
E_6(B)&=\operatorname{span}\{(1,2,1)^T\}.
\end{aligned}
$$

Every nonzero vector in a listed [eigenspace](../../../linear-operator-theory.md#eigenspace) is an [eigenvector](../../../linear-operator-theory.md#eigenvector), and these are all the [eigenvectors](../../../linear-operator-theory.md#eigenvector). For $A$, the repeated [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $2$ has a two-dimensional [eigenspace](../../../linear-operator-theory.md#eigenspace); for $B$, all three [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are simple. The three displayed generating vectors form a [basis](../../../vector-space.md#basis) because their column matrix

$$
S=\begin{pmatrix}1&1&1\\1&0&2\\1&-1&1\end{pmatrix}
$$

has [determinant](../../../linear-algebra.md#determinant) $2$. Thus **both matrices are diagonalizable**, with diagonal entries $(1,2,2)$ for $A$ and $(2,4,6)$ for $B$ in this [basis](../../../vector-space.md#basis).

<h3 id="7a/ii">ii</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7a/ii)

Suppose $C=S\Lambda_CS^{-1}$ and $D=S\Lambda_DS^{-1}$ for an invertible $S$ and diagonal matrices $\Lambda_C,\Lambda_D$. Since diagonal matrices commute,

$$
CD=S\Lambda_C\Lambda_DS^{-1}=S\Lambda_D\Lambda_CS^{-1}=DC.
$$

Therefore **simultaneous diagonalization implies commutation**. This argument works over either $\mathbb R$ or $\mathbb C$ and explains why [simultaneous diagonalization](../../../mathematics.md#simultaneous-diagonalization) produces [commuting operators](../../../vector-space.md#commuting-operators).

<h3 id="7a/iii">iii</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#7a/iii)

Let $Dx=\lambda x$ with $x\ne0$. Commutation gives

$$
D(Cx)=C(Dx)=\lambda Cx.
$$

Thus $Cx$ belongs to the [eigenspace](../../../linear-operator-theory.md#eigenspace) $E_\lambda(D)$, with the zero vector allowed. Since $D$ has $n$ distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue), each [eigenspace](../../../linear-operator-theory.md#eigenspace) is one-dimensional. Hence **$Cx=\mu x$ for some scalar $\mu$**. This is the fact that [commuting maps preserve eigenspaces](../../../vector-space.md#commuting-maps-preserve-eigenspaces).

The standard [linear independence](../../../vector-space.md#linear-independence) theorem for [eigenvectors](../../../linear-operator-theory.md#eigenvector) belonging to distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) supplies a [basis](../../../vector-space.md#basis) $x_1,\ldots,x_n$ of [eigenvectors](../../../linear-operator-theory.md#eigenvector) of $D$. The preceding argument makes every one an [eigenvector](../../../linear-operator-theory.md#eigenvector) of $C$ as well. Their column matrix therefore simultaneously diagonalizes $C$ and $D$. This is [simple spectrum gives simultaneous diagonalization](../../../mathematics.md#simple-spectrum-gives-simultaneous-diagonalization).

For real matrices, this conclusion always holds over $\mathbb C$; a real common [basis](../../../vector-space.md#basis) follows when the distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $D$ are real. Real matrix entries alone do not ensure a real [eigenbasis](../../../linear-operator-theory.md#eigenbasis): a quarter-turn of $\mathbb R^2$, with $C=D$, has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\pm i$. The matrices in this question have real spectra, so their common [basis](../../../vector-space.md#basis) is real.

<h3 id="7a/iv">iv</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#7a/iv)

Direct multiplication gives

$$
AB=BA=\begin{pmatrix}0&10&-8\\-10&22&-10\\-8&10&0\end{pmatrix}.
$$

Take $D=B$ and $C=A$ in the preceding result: $B$ has the three distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $2,4,6$ and the matrices commute. The common [eigenbasis](../../../linear-operator-theory.md#eigenbasis) from part (i) gives

$$
\boxed{S=\begin{pmatrix}1&1&1\\1&0&2\\1&-1&1\end{pmatrix},\quad S^{-1}AS=\operatorname{diag}(1,2,2),\quad S^{-1}BS=\operatorname{diag}(2,4,6).}
$$

Indeed $AS=S\operatorname{diag}(1,2,2)$ and $BS=S\operatorname{diag}(2,4,6)$, and $\det S=2\ne0$. These equalities directly verify the [simultaneous diagonalization](../../../mathematics.md#simultaneous-diagonalization).

## 8A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8a/a">a</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/a/i">i</h4>

↑ **Parent:** [A](#8a/a)

<h5 id="8a/a/i/solution">Solution</h5>

↑ **Parent:** [I](#8a/a/i)

For the standard complex [inner product](../../../linear-algebra.md#inner-product), $\|y\|^2=y^\dagger y$. Using the [conjugate transpose](../../../linear-operator-theory.md#conjugate-transpose) and the defining equality for a [normal matrix](../../../linear-operator-theory.md#normal-matrix),

$$
\|Ax\|^2=x^\dagger A^\dagger Ax=x^\dagger AA^\dagger x=\|A^\dagger x\|^2.
$$

Both [norms](../../../functional-analysis.md#norm) are nonnegative, so **$\|Ax\|=\|A^\dagger x\|$** for every $x$.

<h4 id="8a/a/ii">ii</h4>

↑ **Parent:** [A](#8a/a)

<h5 id="8a/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8a/a/ii)

Set $M=A-\lambda I$. Its [conjugate transpose](../../../linear-operator-theory.md#conjugate-transpose) is $M^\dagger=A^\dagger-\overline\lambda I$, so

$$
\begin{aligned}
M^\dagger M&=A^\dagger A-\lambda A^\dagger-\overline\lambda A+|\lambda|^2I,\\
MM^\dagger&=AA^\dagger-\overline\lambda A-\lambda A^\dagger+|\lambda|^2I.
\end{aligned}
$$

Since $A$ is a [normal matrix](../../../linear-operator-theory.md#normal-matrix), the two products coincide. Therefore **$A-\lambda I$ is normal for every complex $\lambda$**.

<h4 id="8a/a/iii">iii</h4>

↑ **Parent:** [A](#8a/a)

<h5 id="8a/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#8a/a/iii)

If $Ax=\lambda x$, then $M=A-\lambda I$ is a [normal matrix](../../../linear-operator-theory.md#normal-matrix) by part (ii), and $Mx=0$. Part (i), applied to $M$, yields $\|M^\dagger x\|=\|Mx\|=0$. Thus

$$
\boxed{A^\dagger x=\overline\lambda x.}
$$

The nonzero vector $x$ is consequently an [eigenvector](../../../linear-operator-theory.md#eigenvector) of the [conjugate transpose](../../../linear-operator-theory.md#conjugate-transpose) with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\overline\lambda$. This [adjoint eigenvector identity for a normal matrix](../../../linear-operator-theory.md#adjoint-eigenvector-identity-for-a-normal-matrix) will also determine the special spectral restrictions below.

<h4 id="8a/a/iv">iv</h4>

↑ **Parent:** [A](#8a/a)

<h5 id="8a/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#8a/a/iv)

The [adjoint eigenvector identity for a normal matrix](../../../linear-operator-theory.md#adjoint-eigenvector-identity-for-a-normal-matrix) gives $A^\dagger x_\lambda=\overline\lambda x_\lambda$. Hence

$$
\mu x_\lambda^\dagger x_\mu=x_\lambda^\dagger Ax_\mu=(A^\dagger x_\lambda)^\dagger x_\mu=\lambda x_\lambda^\dagger x_\mu.
$$

As $\mu\ne\lambda$, **$x_\lambda^\dagger x_\mu=0$**. Thus [eigenvectors](../../../linear-operator-theory.md#eigenvector) in distinct [eigenspaces](../../../linear-operator-theory.md#eigenspace) of a [normal matrix](../../../linear-operator-theory.md#normal-matrix) are orthogonal in the complex [inner product](../../../linear-algebra.md#inner-product).

<h4 id="8a/a/v">v</h4>

↑ **Parent:** [A](#8a/a)

<h5 id="8a/a/v/solution">Solution</h5>

↑ **Parent:** [V](#8a/a/v)

Start with the assumed [basis](../../../vector-space.md#basis) of [eigenvectors](../../../linear-operator-theory.md#eigenvector), grouping them by [eigenvalue](../../../linear-operator-theory.md#eigenvalue). In each [eigenspace](../../../linear-operator-theory.md#eigenspace), apply the [Gram-Schmidt process](../../../linear-algebra.md#gram-schmidt-process), which replaces a linearly independent list by an orthonormal list with the same span. Every new vector stays within that [eigenspace](../../../linear-operator-theory.md#eigenspace), since an [eigenspace](../../../linear-operator-theory.md#eigenspace) is a vector subspace.

By part (iv), different [eigenspaces](../../../linear-operator-theory.md#eigenspace) are orthogonal. The combined lists therefore form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of the entire space, still consisting of [eigenvectors](../../../linear-operator-theory.md#eigenvector). Let $U$ have these vectors as columns. Then $U$ is a [unitary matrix](../../../linear-operator-theory.md#unitary-matrix), so

$$
\boxed{U^{-1}=U^\dagger,\qquad U^\dagger AU=\operatorname{diag}(\lambda_1,\ldots,\lambda_n).}
$$

This gives the required [unitary diagonalization of a normal matrix](../../../linear-operator-theory.md#unitary-diagonalization-of-a-normal-matrix), including repeated [eigenvalues](../../../linear-operator-theory.md#eigenvalue).

<h3 id="8a/b">b</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/b/solution">Solution</h4>

↑ **Parent:** [B](#8a/b)

For a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator), $A^\dagger=A$, so $A^\dagger A=A^2=AA^\dagger$ and $A$ is a [normal matrix](../../../linear-operator-theory.md#normal-matrix). If $Ax=\lambda x$ with $x\ne0$, part (a)(iii) gives $A^\dagger x=\overline\lambda x$. Since also $A^\dagger x=Ax=\lambda x$, we obtain $\lambda=\overline\lambda$. Thus **every eigenvalue is real**.

<h3 id="8a/c">c</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/c/solution">Solution</h4>

↑ **Parent:** [C](#8a/c)

For a [skew-Hermitian matrix](../../../linear-operator-theory.md#skew-hermitian-matrix), $A^\dagger=-A$, so both $A^\dagger A$ and $AA^\dagger$ equal $-A^2$. It is therefore a [normal matrix](../../../linear-operator-theory.md#normal-matrix). On an [eigenvector](../../../linear-operator-theory.md#eigenvector) with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$, part (a)(iii) gives

$$
\overline\lambda x=A^\dagger x=-Ax=-\lambda x.
$$

Thus $\overline\lambda=-\lambda$, and **every eigenvalue lies in $i\mathbb R$**, including the possible [eigenvalue](../../../linear-operator-theory.md#eigenvalue) zero.

<h3 id="8a/d">d</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/d/solution">Solution</h4>

↑ **Parent:** [D](#8a/d)

For a [unitary matrix](../../../linear-operator-theory.md#unitary-matrix), $A^\dagger=A^{-1}$, so both defining products for a [normal matrix](../../../linear-operator-theory.md#normal-matrix) are $I$. The matrix is invertible, hence no [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is zero. If $Ax=\lambda x$, then $A^{-1}x=\lambda^{-1}x$, while part (a)(iii) gives $A^\dagger x=\overline\lambda x$. Therefore $\overline\lambda=\lambda^{-1}$, and

$$
\boxed{|\lambda|=1.}
$$

Thus **all eigenvalues have unit modulus**.

## 9F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9f/solution">Solution</h3>

↑ **Parent:** [9F](#9f)

Since $a_j=S_j-S_{j-1}$, shifting an index yields the [summation by parts](../../../analytic-number-theory.md#abel-s-summation-formula) identity

$$
\begin{aligned}
\sum_{j=m}^n a_jb_j&=\sum_{j=m}^nS_jb_j-\sum_{j=m}^nS_{j-1}b_j\\
&=S_nb_n-S_{m-1}b_m+\sum_{j=m}^{n-1}S_j(b_j-b_{j+1}).
\end{aligned}
$$

The sum on the last line is empty when $m=n$, so the identity also covers that case.

**The series with a bounded monotone multiplier converges.** Here is a proof that also permits conditional convergence. Choose $M>0$ with $|b_j|\leq M$. The [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) criterion for the convergent series $\sum a_j$ ensures that, for any $\eta>0$ and sufficiently large $m$, all the partial tails $T_j=\sum_{k=m}^j a_k$ satisfy $|T_j|<\eta$. Apply [summation by parts](../../../analytic-number-theory.md#abel-s-summation-formula) to these partial tails:

$$
\sum_{j=m}^n a_jb_j=T_nb_n+\sum_{j=m}^{n-1}T_j(b_j-b_{j+1}).
$$

Since the multiplier is a [monotone sequence](../../../real-analysis.md#monotone-sequence), $\sum_{j=m}^{n-1}|b_j-b_{j+1}|=|b_m-b_n|$. Consequently

$$
\left|\sum_{j=m}^n a_jb_j\right|\leq\eta\bigl(|b_n|+|b_m-b_n|\bigr)\leq3M\eta.
$$

Taking $\eta=\varepsilon/(3M)$ proves that the weighted partial sums form a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence), and hence converge. This is a special case of [bounded-variation multipliers of a convergent series](../../../analytic-number-theory.md#bounded-variation-multipliers-of-a-convergent-series).

**The series $\sum n^{1/n}a_n$ also converges.** The multiplier need only be monotone eventually, since a finite initial segment cannot affect convergence. For $h(x)=\log x/x$,

$$
h'(x)=\frac{1-\log x}{x^2}<0\qquad(x\geq3).
$$

Thus $n^{1/n}=\exp(h(n))$ decreases for $n\geq3$; it is bounded and tends to $1$, because $\log n/n\to0$. Apply the proved multiplier result to the tail beginning at $3$. The fact that the first few values are not monotone causes no difficulty.

## 10D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10d/a">a</h3>

↑ **Parent:** [10D](#10d)

<h4 id="10d/a/solution">Solution</h4>

↑ **Parent:** [A](#10d/a)

We use the [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem): every bounded real sequence has a convergent subsequence. If $f$ were unbounded on $[a,b]$, there would be $x_n\in[a,b]$ with $|f(x_n)|\geq n$. The [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) gives a subsequence $x_{n_k}\to c$, and the closed interval contains $c$. Since $f$ is a [continuous function](../../../calculus.md#continuous-function), $f(x_{n_k})\to f(c)$, contradicting $|f(x_{n_k})|\geq n_k\to\infty$. Thus **$f$ is bounded**.

Let $s=\sup_{x\in[a,b]}f(x)$. By the definition of the [supremum](../../../real-analysis.md#supremum), choose $y_n$ with $s-1/n<f(y_n)\leq s$. Again the [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) gives $y_{n_k}\to d\in[a,b]$. Continuity yields $f(d)=s$. Applying the same argument to $-f$ gives a point where $f$ attains its [infimum](../../../real-analysis.md#infimum). Therefore **both the supremum and the infimum are attained**. This proves the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem) for a closed bounded interval.

<h3 id="10d/b">b</h3>

↑ **Parent:** [10D](#10d)

<h4 id="10d/b/solution">Solution</h4>

↑ **Parent:** [B](#10d/b)

Away from integer multiples of $\pi$, the function is a composition of [continuous functions](../../../calculus.md#continuous-function). At zero, the bound $|g(x)|\leq\sqrt{|x|}$ gives $g(x)\to0=g(0)$ by the [squeeze theorem](../../../calculus.md#squeeze-theorem). This is [oscillation multiplied by a vanishing amplitude](../../../calculus.md#oscillation-multiplied-by-a-vanishing-amplitude).

Fix $n\ne0$ and set $t_k=\pi/2+2\pi k$ and $x_k=n\pi+(-1)^n\arcsin(1/t_k)$. Then $x_k\to n\pi$, $\sin x_k=1/t_k$, and

$$
g(x_k)=\sqrt{|x_k|}\longrightarrow\sqrt{|n\pi|}\ne0=g(n\pi).
$$

So $g$ is discontinuous at every nonzero integer multiple of $\pi$. Its **set of continuity points** is

$$
\boxed{\mathbb R\setminus\{n\pi:n\in\mathbb Z,\ n\ne0\}.}
$$

On $[0,\pi]$, $g(x)\leq\sqrt{x}<\sqrt\pi$ for $x<\pi$, while $g(\pi)=0$. With $x_k=\pi-\arcsin(1/t_k)$ as above, $g(x_k)=\sqrt{x_k}\to\sqrt\pi$. Consequently **the supremum is $\sqrt\pi$ and is not attained**. This illustrates that [supremum can fail to be attained at an oscillatory endpoint](../../../real-analysis.md#supremum-can-fail-to-be-attained-at-an-oscillatory-endpoint).

On $[\pi,3\pi/2]$, set $x_0=\pi+\arcsin(2/(3\pi))$. It lies strictly inside the interval, and $1/\sin x_0=-3\pi/2$, so $g(x_0)=\sqrt{x_0}>\sqrt\pi$. Choose $0<\delta<x_0-\pi$. On $[\pi,\pi+\delta]$,

$$
g(x)\leq\sqrt{\pi+\delta}<\sqrt{x_0}=g(x_0).
$$

On $[\pi+\delta,3\pi/2]$, $g$ is a [continuous function](../../../calculus.md#continuous-function), so the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem) gives a maximum there, at least $g(x_0)$. It exceeds every value on the discarded interval. Therefore **$g$ does attain its supremum on $[\pi,3\pi/2]$**. This is the [interior-value criterion for an attained maximum](../../../real-analysis.md#interior-value-criterion-for-an-attained-maximum).

<a id="10d/b/image-oscillatory-function-near-pi-an-unattained-left-supremum-and-a-right-interior-value-above-the-endpoint-envelope"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-1-oscillatory-suprema.png)

**[Figure 1](#10d/b/image-oscillatory-function-near-pi-an-unattained-left-supremum-and-a-right-interior-value-above-the-endpoint-envelope). Oscillatory function near pi: an unattained left supremum and a right interior value above the endpoint envelope**.

## 11D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11d/i">i</h3>

↑ **Parent:** [11D](#11d)

<h4 id="11d/i/solution">Solution</h4>

↑ **Parent:** [I](#11d/i)

The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) says that if $f:[a,b]\to\mathbb R$ is a [continuous function](../../../calculus.md#continuous-function), then every value between $f(a)$ and $f(b)$ is attained at some point of $[a,b]$.

Endpoint values are already attained. Suppose $f(a)<y<f(b)$ and define $E=\{x\in[a,b]:f(x)<y\}$. It is nonempty and bounded above, so $c=\sup E$ exists. Continuity at $a$ ensures that $E$ contains points to the right of $a$, and continuity at $b$ ensures that no point sufficiently close to $b$ belongs to $E$. Hence $a<c<b$.

By the definition of the [supremum](../../../real-analysis.md#supremum), there are points of $E$ approaching $c$. If $f(c)>y$, continuity would exclude all such nearby points from $E$, a contradiction. If $f(c)<y$, continuity would put some point to the right of $c$ in $E$, again a contradiction. Therefore **$f(c)=y$**. When $f(a)>f(b)$, apply this argument to $-f$. This proves the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) in all cases.

<h3 id="11d/ii">ii</h3>

↑ **Parent:** [11D](#11d)

<h4 id="11d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11d/ii)

For a chord of length $1/2$, consider the [continuous function](../../../calculus.md#continuous-function) $h(x)=f(x+1/2)-f(x)$ on $[0,1/2]$. Since $f(0)=f(1)$,

$$
h(1/2)=f(1)-f(1/2)=-h(0).
$$

An endpoint zero already supplies the chord. Otherwise the endpoint values have opposite signs, so the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) supplies $h(\alpha)=0$ at some $\alpha\in(0,1/2)$. Thus **a horizontal chord of length $1/2$ exists**.

For each integer $n>1$, define $h_n(x)=f(x+1/n)-f(x)$ on $[0,1-1/n]$. The sampled differences telescope:

$$
\sum_{j=0}^{n-1}h_n(j/n)=\sum_{j=0}^{n-1}\bigl(f((j+1)/n)-f(j/n)\bigr)=f(1)-f(0)=0.
$$

If any sampled value is zero, it gives the required chord. Otherwise there must be both a positive and a negative sampled value. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem), applied between their sample points, then gives $h_n(\alpha)=0$. Hence **a horizontal chord of length $1/n$ exists for every positive integer $n$**; for $n=1$, the endpoint chord itself suffices. This proves the [horizontal chord of reciprocal-integer length](../../../calculus.md#horizontal-chord-of-reciprocal-integer-length) result, without restricting $n$ to powers of two.

## 12E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12e/solution">Solution</h3>

↑ **Parent:** [12E](#12e)

For a partition $P$, write $U(f,P)$ and $L(f,P)$ for the [upper Darboux sum](../../../real-analysis.md#upper-darboux-sum) and [lower Darboux sum](../../../real-analysis.md#lower-darboux-sum). The [Riemann integrability criterion](../../../real-analysis.md#riemann-integrability-criterion) for bounded $f$ is that for every $\varepsilon>0$ some partition satisfies $U(f,P)-L(f,P)<\varepsilon$. Thus if the gaps for $D_n$ tend to zero, the [Riemann integrability criterion](../../../real-analysis.md#riemann-integrability-criterion) immediately proves that $f$ is [Riemann integrable](../../../real-analysis.md#riemann-integrable-function).

Conversely, suppose $f$ is [Riemann integrable](../../../real-analysis.md#riemann-integrable-function), and choose a fixed partition $P$ with $U(f,P)-L(f,P)<\varepsilon/2$. Let $r$ be the number of its interior division points and choose $M\geq1$ with $|f|\leq M$. Call a cell of $D_n$ bad when its interior contains a division point of $P$. There are at most $r$ bad cells, and their total length is at most $r/n$.

Every other cell lies in a single cell of $P$, so its oscillation is no larger than that of the containing cell. Summing the contributions of these good cells gives at most $U(f,P)-L(f,P)$, while each bad cell has oscillation at most $2M$. Therefore the [finite bad-cell estimate for Darboux sums](../../../real-analysis.md#finite-bad-cell-estimate-for-darboux-sums) gives

$$
0\leq U(f,D_n)-L(f,D_n)\leq U(f,P)-L(f,P)+\frac{2Mr}{n}.
$$

For large enough $n$, the right-hand side is less than $\varepsilon$. This proves the [uniform-mesh Darboux criterion](../../../real-analysis.md#uniform-mesh-darboux-criterion)

$$
\boxed{f\text{ is Riemann integrable}\quad\Longleftrightarrow\quad U(f,D_n)-L(f,D_n)\longrightarrow0.}
$$

This argument does not assume that the partitions $D_n$ are nested; in general they are not.

For the composition, $f$ takes values in $[-M,M]$. Since $g$ is continuously differentiable, the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem) bounds both $|g|$ and $|g'|$ on that interval. In particular, let $K=\sup_{[-M,M]}|g'|<\infty$. The [mean value theorem](../../../calculus.md#mean-value-theorem) states that a function continuous on the interval between $s,t$ and differentiable in its interior satisfies $g(s)-g(t)=g'(\xi)(s-t)$ for some intermediate $\xi$. Hence

$$
|g(s)-g(t)|\leq K|s-t|\qquad(s,t\in[-M,M]).
$$

On each partition cell, this bounds the oscillation of $g\circ f$ by $K$ times the oscillation of $f$, whether or not the local extrema are attained. It follows that

$$
U(g\circ f,D_n)-L(g\circ f,D_n)\leq K\bigl(U(f,D_n)-L(f,D_n)\bigr)\longrightarrow0.
$$

The composition is bounded, so the proved [uniform-mesh Darboux criterion](../../../real-analysis.md#uniform-mesh-darboux-criterion) applies. Thus **$g\circ f$ is Riemann integrable**. The reusable fact is [Lipschitz composition preserves Riemann integrability](../../../real-analysis.md#lipschitz-composition-preserves-riemann-integrability); continuous differentiability supplies the required bound on the range of $f$.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
