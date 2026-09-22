# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2025/paperia_1_2025.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2025/paperia_1_2025.pdf)

**Table of contents**

- [1B](#1b)
  - [a](#1b/a)
    - [Solution](#1b/a/solution)
  - [b](#1b/b)
    - [Solution](#1b/b/solution)
- [2C](#2c)
  - [a](#2c/a)
    - [Solution](#2c/a/solution)
  - [b](#2c/b)
    - [Solution](#2c/b/solution)
  - [c](#2c/c)
    - [Solution](#2c/c/solution)
- [3E](#3e)
  - [a](#3e/a)
    - [Solution](#3e/a/solution)
  - [b](#3e/b)
    - [Solution](#3e/b/solution)
  - [c](#3e/c)
    - [Solution](#3e/c/solution)
  - [d](#3e/d)
    - [Solution](#3e/d/solution)
- [4E](#4e)
  - [a](#4e/a)
    - [Solution](#4e/a/solution)
  - [b](#4e/b)
    - [Solution](#4e/b/solution)
- [5B](#5b)
  - [Solution](#5b/solution)
  - [i](#5b/i)
    - [Solution](#5b/i/solution)
  - [ii](#5b/ii)
    - [Solution](#5b/ii/solution)
  - [iii](#5b/iii)
    - [Solution](#5b/iii/solution)
- [6C](#6c)
  - [a](#6c/a)
    - [Solution](#6c/a/solution)
  - [b](#6c/b)
    - [Solution](#6c/b/solution)
  - [c](#6c/c)
    - [i](#6c/c/i)
      - [Solution](#6c/c/i/solution)
    - [ii](#6c/c/ii)
      - [Solution](#6c/c/ii/solution)
  - [d](#6c/d)
    - [Solution](#6c/d/solution)
  - [e](#6c/e)
    - [Solution](#6c/e/solution)
- [7A](#7a)
  - [a](#7a/a)
    - [Solution](#7a/a/solution)
  - [b](#7a/b)
    - [Solution](#7a/b/solution)
  - [c](#7a/c)
    - [Solution](#7a/c/solution)
  - [d](#7a/d)
    - [Solution](#7a/d/solution)
- [8A](#8a)
  - [a](#8a/a)
    - [Solution](#8a/a/solution)
  - [b](#8a/b)
    - [Solution](#8a/b/solution)
  - [c](#8a/c)
    - [Solution](#8a/c/solution)
  - [d](#8a/d)
    - [Solution](#8a/d/solution)
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
  - [d](#9e/d)
    - [Solution](#9e/d/solution)
- [10E](#10e)
  - [a](#10e/a)
    - [Solution](#10e/a/solution)
  - [b](#10e/b)
    - [Solution](#10e/b/solution)
  - [c](#10e/c)
    - [Solution](#10e/c/solution)
  - [d](#10e/d)
    - [Solution](#10e/d/solution)
  - [e](#10e/e)
    - [i](#10e/e/i)
      - [Solution](#10e/e/i/solution)
    - [ii](#10e/e/ii)
      - [Solution](#10e/e/ii/solution)
- [11E](#11e)
  - [a](#11e/a)
    - [Solution](#11e/a/solution)
  - [b](#11e/b)
    - [Solution](#11e/b/solution)
  - [c](#11e/c)
    - [Solution](#11e/c/solution)
  - [d](#11e/d)
    - [Solution](#11e/d/solution)
- [12E](#12e)
  - [a](#12e/a)
    - [Solution](#12e/a/solution)
  - [b](#12e/b)
    - [Solution](#12e/b/solution)
  - [c](#12e/c)
    - [Solution](#12e/c/solution)
  - [d](#12e/d)
    - [Solution](#12e/d/solution)

## 1B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1b/a">a</h3>

↑ **Parent:** [1B](#1b)

<h4 id="1b/a/solution">Solution</h4>

↑ **Parent:** [A](#1b/a)

Translate and scale the circle to $|z|=1$. For distinct points $u,v,w$ on it, the angle at $w$ is right exactly when

$$
R=\frac{u-w}{v-w}
$$

is purely imaginary. Since $\bar u=u^{-1}$ and similarly for $v,w$, direct simplification gives $\bar R=(v/u)R$. Thus $\bar R=-R$ exactly when $v=-u$, which says that the opposite side joins antipodal points and is a diameter. The converse is the same calculation in reverse.

<h3 id="1b/b">b</h3>

↑ **Parent:** [1B](#1b)

<h4 id="1b/b/solution">Solution</h4>

↑ **Parent:** [B](#1b/b)

The vertices satisfy

$$
(z+1)^N-1=0.
$$

After removing the root $z=0$, the product of the other roots has [modulus](../../../complex-analysis.md#modulus) equal to the constant term of $((z+1)^N-1)/z$, namely $N$. Hence the product of the $N-1$ chord lengths from one vertex of a unit [regular polygon](../../../geometry-and-topology.md#regular-polygon) is $N$. Multiplying this identity over all $N$ vertices counts every chord twice, so the product of all chord lengths is $N^{N/2}$. Scaling the circle by $R$ scales each of its $N(N-1)/2$ chords by $R$, giving

$$
\boxed{N^{N/2}R^{N(N-1)/2}.}
$$

## 2C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2c/a">a</h3>

↑ **Parent:** [2C](#2c)

<h4 id="2c/a/solution">Solution</h4>

↑ **Parent:** [A](#2c/a)

Expansion gives $\det A=(a-3)(a+2)$. Thus uniqueness fails precisely for $a=-2$ and $a=3$.

<h3 id="2c/b">b</h3>

↑ **Parent:** [2C](#2c)

<h4 id="2c/b/solution">Solution</h4>

↑ **Parent:** [B](#2c/b)

Solvability requires $b$ to be orthogonal to the left nullspace. For $a=-2$ one may take $n=(-3,-2,2)^T$; for $a=3$ one may take $n=(1,-1,1)^T$.

<h3 id="2c/c">c</h3>

↑ **Parent:** [2C](#2c)

<h4 id="2c/c/solution">Solution</h4>

↑ **Parent:** [C](#2c/c)

For $b=(2,b,0)^T$, compatibility gives $b=-3$ when $a=-2$ and $b=2$ when $a=3$. The respective solution families are

$$
x=(1,-1,0)^T+t(1,1,1)^T
$$

and

$$
x=(1,-1,0)^T+t(-3/2,7/2,1)^T,
$$

where $t\in\mathbb R$.

## 3E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3e/a">a</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/a/solution">Solution</h4>

↑ **Parent:** [A](#3e/a)

For every $z\in\mathbb C$,

$$
e^z=\sum_{n=0}^{\infty}\frac{z^n}{n!},\qquad
\sin z=\sum_{n=0}^{\infty}(-1)^n\frac{z^{2n+1}}{(2n+1)!}.
$$

<h3 id="3e/b">b</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/b/solution">Solution</h4>

↑ **Parent:** [B](#3e/b)

Termwise [differentiation](../../../calculus.md#differentiation) gives

$$
f\prime(z)=\sum_{n=1}^{\infty}n a_nz^{n-1}.
$$

The differentiated [series](../../../real-analysis.md#series-mathematics) has the same radius of convergence $R$.

<h3 id="3e/c">c</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/c/solution">Solution</h4>

↑ **Parent:** [C](#3e/c)

Fix $a$ and define $g(b)=e^{a+b}e^{-b}$ using only the power [series](../../../real-analysis.md#series-mathematics). Termwise [differentiation](../../../calculus.md#differentiation) gives $(e^z)\prime=e^z$, and the product rule gives $g\prime(b)=0$. Hence $g$ is constant, so $g(b)=g(0)=e^a$. Multiplication by $e^b$ yields $e^{a+b}=e^ae^b$.

<h3 id="3e/d">d</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/d/solution">Solution</h4>

↑ **Parent:** [D](#3e/d)

The removable definition gives the entire [series](../../../real-analysis.md#series-mathematics)

$$
f(z)=\sum_{n=0}^{\infty}(-1)^n\frac{z^{2n}}{(2n+1)!}.
$$

Therefore

$$
f^{(k)}(0)=\begin{cases}0,&k\text{ odd},\\(-1)^{k/2}/(k+1),&k\text{ even}.
\end{cases}
$$

## 4E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4e/a">a</h3>

↑ **Parent:** [4E](#4e)

<h4 id="4e/a/solution">Solution</h4>

↑ **Parent:** [A](#4e/a)

The Darboux–Riemann criterion says that a [bounded function](../../../function.md#bounded-function) on $[a,b]$ is Riemann integrable exactly when, for every $\varepsilon>0$, some partition $P$ satisfies $U(f,P)-L(f,P)<\varepsilon$. Indeed, every lower sum is at most every upper sum. Taking the supremum of lower sums and infimum of upper sums, the criterion makes their difference smaller than every positive $\varepsilon$, so they are equal; this common value is the Riemann [integral](../../../calculus.md#integral).

<h3 id="4e/b">b</h3>

↑ **Parent:** [4E](#4e)

<h4 id="4e/b/solution">Solution</h4>

↑ **Parent:** [B](#4e/b)

Given $\varepsilon>0$, choose a partition of $[a,d]$ whose upper-minus-lower sum is below $\varepsilon$, and refine it by inserting $b,c$. The contribution from subintervals lying in $[b,c]$ is nonnegative and no larger than the total difference. Restricting the refined partition to $[b,c]$ therefore gives upper-minus-lower sum below $\varepsilon$, so the criterion proves integrability there.

## 5B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5b/solution">Solution</h3>

↑ **Parent:** [5B](#5b)

Taking the parallelogram spanned by $e_2,e_3$ as base gives base area $|e_2\times e_3|$ and height $|e_1\cdot(e_2\times e_3)|/|e_2\times e_3|$. A tetrahedron has one third of the corresponding pyramid volume and the triangle has half the parallelogram base, hence

$$
V=\frac16|\Delta|,\qquad \Delta=e_1\cdot(e_2\times e_3).
$$

The reciprocal [vectors](../../../vector-space.md#vector) are

$$
f_1=\frac{e_2\times e_3}{\Delta},\quad f_2=\frac{e_3\times e_1}{\Delta},\quad f_3=\frac{e_1\times e_2}{\Delta},
$$

which directly satisfy $f_i\cdot e_j=\delta_{ij}$.

<h3 id="5b/i">i</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/i/solution">Solution</h4>

↑ **Parent:** [I](#5b/i)

The final face contains $v_i=v+e_i$, so $c\cdot(v+e_i)+d=0$. Therefore $e_i\cdot c=-(c\cdot v+d)$.

<h3 id="5b/ii">ii</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5b/ii)

The $i$th face through $v$ contains the two edge directions $e_j$ with $j\ne i$, so $a_i\cdot e_j=0$ for those $j$. The one-dimensional space with these two orthogonality conditions is spanned by $f_i$, hence $a_i=\lambda_i f_i$ for some nonzero real $\lambda_i$.

<h3 id="5b/iii">iii</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5b/iii)

Dotting $c=\sum_j\gamma_ja_j$ with $e_i$ gives $e_i\cdot c=\gamma_i\lambda_i$, proving $\gamma_i=(e_i\cdot c)/\lambda_i$. Also

$$
a_1\cdot(a_2\times a_3)=\frac{\lambda_1\lambda_2\lambda_3}{\Delta},\qquad
\gamma_1\gamma_2\gamma_3=-\frac{(c\cdot v+d)^3}{\lambda_1\lambda_2\lambda_3}.
$$

Combining these with $V=|\Delta|/6$ gives the displayed face formula, with the orientation chosen so its signed right-hand side is positive.

## 6C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6c/a">a</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/a/solution">Solution</h4>

↑ **Parent:** [A](#6c/a)

The distinguished unit [vector](../../../vector-space.md#vector) is $n=(1,1,1)/\sqrt3$. Comparing diagonal, symmetric off-diagonal, and antisymmetric parts gives

$$
\alpha=a-\frac{b+c}{2},\qquad \beta=\frac32(b+c),\qquad \gamma=\frac{\sqrt3}{2}(b-c),
$$

so $A_{ij}=\alpha\delta_{ij}+\beta n_in_j+\gamma\varepsilon_{ijk}n_k$.

<h3 id="6c/b">b</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/b/solution">Solution</h4>

↑ **Parent:** [B](#6c/b)

On the line spanned by $n$, $A$ multiplies by $L=\alpha+\beta=a+b+c$. On $n^\perp$, it is the composition of a rotation with a dilation by $r=\sqrt{\alpha^2+\gamma^2}$. Consequently every area in that plane is multiplied by $r^2=\alpha^2+\gamma^2$.

<h3 id="6c/c">c</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/c/i">i</h4>

↑ **Parent:** [C](#6c/c)

<h5 id="6c/c/i/solution">Solution</h5>

↑ **Parent:** [I](#6c/c/i)

For a plane reflection, the $n$ direction is reversed while $n^\perp$ is fixed. Thus $L=-1$, $\alpha=1$, and $\gamma=0$, equivalently

$$
\boxed{a=\frac13,\qquad b=c=-\frac23.}
$$

<h4 id="6c/c/ii">ii</h4>

↑ **Parent:** [C](#6c/c)

<h5 id="6c/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6c/c/ii)

The map is a rotation about the $n$ axis exactly when

$$
a+b+c=1,\qquad \alpha^2+\gamma^2=1,
$$

or explicitly

$$
(2a-b-c)^2+3(b-c)^2=4.
$$

These conditions make the axis fixed and the perpendicular-plane action length preserving; they are also necessary.

<h3 id="6c/d">d</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/d/solution">Solution</h4>

↑ **Parent:** [D](#6c/d)

Let $N=nn^T$ and $K_{ij}=\varepsilon_{ijk}n_k$. Since $K^2=N-I$, inversion separately on $\mathbb Rn$ and $n^\perp$ gives

$$
(A^{-1})_{ij}=\frac{\alpha}{\alpha^2+\gamma^2}\delta_{ij}
+\left(\frac1{\alpha+\beta}-\frac{\alpha}{\alpha^2+\gamma^2}\right)n_in_j
-\frac{\gamma}{\alpha^2+\gamma^2}\varepsilon_{ijk}n_k,
$$

provided $(\alpha+\beta)(\alpha^2+\gamma^2)\ne0$.

<h3 id="6c/e">e</h3>

↑ **Parent:** [6C](#6c)

<h4 id="6c/e/solution">Solution</h4>

↑ **Parent:** [E](#6c/e)

The line/plane decomposition gives

$$
\det A=(\alpha+\beta)(\alpha^2+\gamma^2).
$$

Substituting the values in part (a) and simplifying yields

$$
\boxed{\det A=\frac12(a+b+c)\bigl((a-b)^2+(b-c)^2+(c-a)^2\bigr).}
$$

## 7A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7a/a">a</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/a/solution">Solution</h4>

↑ **Parent:** [A](#7a/a)

An [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$ is a [scalar](../../../vector-space.md#scalar) for which $\ker(A-\lambda I)$ contains a nonzero [vector](../../../vector-space.md#vector); that kernel is its eigenspace. The characteristic [polynomial](../../../polynomial.md) has degree $n$, so the [fundamental theorem of algebra](../../../algebra.md#fundamental-theorem-of-algebra) supplies at least one complex root and hence an [eigenvalue](../../../linear-operator-theory.md#eigenvalue). Its eigenspace dimension can be any integer from $1$ to $n$.

<h3 id="7a/b">b</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/b/solution">Solution</h4>

↑ **Parent:** [B](#7a/b)

With $\chi_A(t)=\det(tI-A)$, direct expansion gives

$$
\chi_A(t)=(t-3)(t-1)^2(t+1)(t+2).
$$

**Thus the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $3,1,-1,-2$. Kernel calculation gives [eigenspace](../../../linear-operator-theory.md#eigenspace) dimensions $1,2,1,1$, respectively.**

<h3 id="7a/c">c</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/c/solution">Solution</h4>

↑ **Parent:** [C](#7a/c)

The [eigenvalue](../../../linear-operator-theory.md#eigenvalue) equation is $u_{i+1}=\lambda u_i$, so

$$
u=c(1,\lambda,\lambda^2,\ldots)^T.
$$

This is a nonzero square-summable [vector](../../../vector-space.md#vector) exactly when $c\ne0$ and $|\lambda|<1$. Hence every point of the open unit disc is an [eigenvalue](../../../linear-operator-theory.md#eigenvalue), with the displayed one-dimensional eigenspace.

<h3 id="7a/d">d</h3>

↑ **Parent:** [7A](#7a)

<h4 id="7a/d/solution">Solution</h4>

↑ **Parent:** [D](#7a/d)

For the transpose shift, $(Cu)_1=0$ and $(Cu)_i=u_{i-1}$ for $i\ge2$. If $Cu=\lambda u$, the first equation and the subsequent recurrence force every component to vanish, both for $\lambda=0$ and for $\lambda\ne0$. Thus $C$ has no [eigenvalues](../../../linear-operator-theory.md#eigenvalue), illustrating that a bounded infinite-dimensional operator need not have one.

## 8A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8a/a">a</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/a/solution">Solution</h4>

↑ **Parent:** [A](#8a/a)

A complex [matrix](../../../vector-space.md#matrix) is diagonalisable when it is similar to a diagonal [matrix](../../../vector-space.md#matrix), equivalently when the [vector space](../../../vector-space.md) has a [basis](../../../vector-space.md#basis) of its [eigenvectors](../../../linear-operator-theory.md#eigenvector).

<h3 id="8a/b">b</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/b/solution">Solution</h4>

↑ **Parent:** [B](#8a/b)

If $Av=\lambda v$, then $p(A)v=p(\lambda)v$, proving one inclusion. Conversely, if $\mu$ is an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of $p(A)$, factor $p(z)-\mu=c\prod_j(z-\lambda_j)$. If none of the $\lambda_j$ were [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $A$, every $A-\lambda_jI$ would be invertible, making $p(A)-\mu I$ invertible, a contradiction. Thus $\mu=p(\lambda)$ for some [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$ of $A$.

<h3 id="8a/c">c</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/c/solution">Solution</h4>

↑ **Parent:** [C](#8a/c)

Write $A=S\operatorname{diag}(\lambda_1,\ldots,\lambda_n)S^{-1}$. The power [series](../../../real-analysis.md#series-mathematics) gives $e^A=S\operatorname{diag}(e^{\lambda_1},\ldots,e^{\lambda_n})S^{-1}$. Therefore

$$
\boxed{\det(e^A)=\prod_i e^{\lambda_i}=e^{\sum_i\lambda_i}=e^{\operatorname{tr}A}.}
$$

<h3 id="8a/d">d</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/d/solution">Solution</h4>

↑ **Parent:** [D](#8a/d)

The [vectors](../../../vector-space.md#vector) $(1,0,1)^T,(0,1,0)^T,(1,0,-1)^T$ are [eigenvectors](../../../linear-operator-theory.md#eigenvector) of $B$ with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $2,1,0$. Applying the exponential to these eigenspaces gives

$$
e^B=\begin{pmatrix}(1+e^2)/2&0&(e^2-1)/2\\0&e&0\\(e^2-1)/2&0&(1+e^2)/2\end{pmatrix}.
$$

## 9E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9e/a">a</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/a/solution">Solution</h4>

↑ **Parent:** [A](#9e/a)

A [sequence](../../../real-analysis.md#sequence) $(a_n)$ is Cauchy when, for every $\varepsilon>0$, some $N$ satisfies $|a_m-a_n|<\varepsilon$ whenever $m,n\ge N$.

<h3 id="9e/b">b</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/b/solution">Solution</h4>

↑ **Parent:** [B](#9e/b)

The general principle of convergence says that a real [sequence](../../../real-analysis.md#sequence) converges exactly when it is Cauchy. Convergent [sequences](../../../real-analysis.md#sequence) are Cauchy by the triangle inequality. Conversely, a Cauchy [sequence](../../../real-analysis.md#sequence) is bounded, so Bolzano–Weierstrass gives a convergent subsequence $a_{n_k}\to a$; the Cauchy property then forces the entire [sequence](../../../real-analysis.md#sequence) to converge to $a$.

<h3 id="9e/c">c</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/c/i">i</h4>

↑ **Parent:** [C](#9e/c)

<h5 id="9e/c/i/solution">Solution</h5>

↑ **Parent:** [I](#9e/c/i)

**True.** For $m>n$, $|a_m-a_n|\le\sum_{j=n}^{m-1}d_j$. Convergence of $\sum d_j$ makes this tail arbitrarily small, so $(a_n)$ is Cauchy and hence convergent.

<h4 id="9e/c/ii">ii</h4>

↑ **Parent:** [C](#9e/c)

<h5 id="9e/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9e/c/ii)

**False.** The [sequence](../../../real-analysis.md#sequence) $a_n=(-1)^n/n$ converges to zero, but $|a_{n+1}-a_n|=1/n+1/(n+1)$, whose [series](../../../real-analysis.md#series-mathematics) diverges.

<h3 id="9e/d">d</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/d/solution">Solution</h4>

↑ **Parent:** [D](#9e/d)

Write

$$
\frac{j}{j^2+j+1}=\frac1j+O(j^{-2})
$$

uniformly for $j\ge1$. The accumulated error from $j=n+1$ to $2n$ tends to zero, while the corresponding [harmonic sum](../../../real-analysis.md#harmonic-sum) tends to $\log2$. Hence $b_n\to\log2$.

## 10E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10e/a">a</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/a/solution">Solution</h4>

↑ **Parent:** [A](#10e/a)

The statement $\lim_{t\to x}f(t)=\ell$ means that for every $\varepsilon>0$ there is $\delta>0$ such that $t\in[0,1]$ and $0<|t-x|<\delta$ imply $|f(t)-\ell|<\varepsilon$.

<h3 id="10e/b">b</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/b/solution">Solution</h4>

↑ **Parent:** [B](#10e/b)

The [function](../../../function.md) is continuous at $x$ exactly when $\lim_{t\to x}f(t)=f(x)$.

<h3 id="10e/c">c</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/c/solution">Solution</h4>

↑ **Parent:** [C](#10e/c)

If $x_n\to x$, continuity of $f$ gives $f(x_n)\to f(x)$, and continuity of $g$ at $f(x)$ then gives $g(f(x_n))\to g(f(x))$. The sequential criterion proves continuity of $g\circ f$ at $x$.

<h3 id="10e/d">d</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/d/solution">Solution</h4>

↑ **Parent:** [D](#10e/d)

Both [functions](../../../function.md) are continuous at every $x>0$. At zero, $f_1(1/(\pi/2+2\pi n))=1$ while $f_1(1/(3\pi/2+2\pi n))=-1$, so $f_1$ is discontinuous. Since $|x\sin(1/x)|\le x\to0$, $f_2$ is continuous at zero and hence everywhere.

<h3 id="10e/e">e</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/e/i">i</h4>

↑ **Parent:** [E](#10e/e)

<h5 id="10e/e/i/solution">Solution</h5>

↑ **Parent:** [I](#10e/e/i)

Let $S=\{0\}\cup\{1/n:n\ge1\}$ and let $D$ be the Dirichlet [function](../../../function.md), equal to $1$ on rationals and $0$ on irrationals. Then $f(x)=d(x,S)D(x)$ is continuous exactly on $S$: the distance factor squeezes it to zero on $S$, while away from $S$ it is a positive continuous factor times an everywhere-discontinuous [function](../../../function.md).

<h4 id="10e/e/ii">ii</h4>

↑ **Parent:** [E](#10e/e)

<h5 id="10e/e/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10e/e/ii)

Using the preceding $f$, define $g(0)=f(0)+1$ and $g(x)=f(x)$ for $x>0$. Changing the value only at zero makes zero discontinuous while preserving continuity at every $1/n$ and discontinuity everywhere else. Thus the continuity set is precisely $\{1/n:n\ge1\}$.

## 11E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11e/a">a</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/a/solution">Solution</h4>

↑ **Parent:** [A](#11e/a)

Differentiability at $x$ means that the [limit](../../../calculus.md#limit-of-a-function)

$$
f\prime(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}h
$$

exists as a finite real number.

<h3 id="11e/b">b</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/b/solution">Solution</h4>

↑ **Parent:** [B](#11e/b)

If $f$ is continuous on $[x,y]$ and [differentiable](../../../analysis.md#differentiable-function) on $(x,y)$, then some $c\in(x,y)$ satisfies $f(y)-f(x)=f\prime(c)(y-x)$.

<h3 id="11e/c">c</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/c/solution">Solution</h4>

↑ **Parent:** [C](#11e/c)

If $f\prime\ge0$, the [mean value theorem](../../../calculus.md#mean-value-theorem) gives $f(y)-f(x)=f\prime(c)(y-x)\ge0$. Conversely, if $f$ is increasing, every difference quotient with positive or negative increment is nonnegative; taking its [limit](../../../calculus.md#limit-of-a-function) gives $f\prime(x)\ge0$.

<h3 id="11e/d">d</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/d/solution">Solution</h4>

↑ **Parent:** [D](#11e/d)

For $x>0$, apply the [mean value theorem](../../../calculus.md#mean-value-theorem) to $[0,x]$: $f(x)/x=f\prime(c)$ for some $c<x$. Since $f\prime$ is increasing, $f(x)/x\le f\prime(x)$. Therefore

$$
\left(\frac{f(x)}x\right)\prime=\frac{xf\prime(x)-f(x)}{x^2}\ge0,
$$

and part (c) proves that the quotient is increasing.

## 12E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12e/a">a</h3>

↑ **Parent:** [12E](#12e)

<h4 id="12e/a/solution">Solution</h4>

↑ **Parent:** [A](#12e/a)

For continuous $f$, the [function](../../../function.md) $F(x)=\int_a^xf(t)dt$ is [differentiable](../../../analysis.md#differentiable-function) with $F\prime=f$. Conversely, if $F\prime$ is continuous, then $\int_a^bF\prime(t)dt=F(b)-F(a)$.

<h3 id="12e/b">b</h3>

↑ **Parent:** [12E](#12e)

<h4 id="12e/b/solution">Solution</h4>

↑ **Parent:** [B](#12e/b)

The fundamental theorem gives

$$
g(b)-f(b)=g(a)-f(a)+\int_a^b(g\prime-f\prime)\,dx\ge0,
$$

which is the desired inequality.

<h3 id="12e/c">c</h3>

↑ **Parent:** [12E](#12e)

<h4 id="12e/c/solution">Solution</h4>

↑ **Parent:** [C](#12e/c)

The assumptions imply $f\ge0$. Since $(f^2)\prime=2ff\prime\le2f$ and both sides vanish at zero, integration gives $f(x)^2\le2F(x)$ where $F(x)=\int_0^xf$. Now

$$
\frac d{dx}\left(F(x)^2-\int_0^xf(t)^3dt\right)=2Ff-f^3=f(2F-f^2)\ge0.
$$

The bracket vanishes at zero, proving $\int_0^xf^3\le(\int_0^xf)^2$.

<h3 id="12e/d">d</h3>

↑ **Parent:** [12E](#12e)

<h4 id="12e/d/solution">Solution</h4>

↑ **Parent:** [D](#12e/d)

**No.** Take the [constant function](../../../function.md#constant-function) $f(t)=c>0$, which has $f\prime=0$. The claimed inequality becomes $c^3x\le c^2x^2$, false whenever $0<x<c$.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
