# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2017/paperia_1_0.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2017/paperia_1_0.pdf)

**Table of contents**

- [1A](#1a)
  - [a](#1a/a)
    - [Solution](#1a/a/solution)
  - [b](#1a/b)
    - [Solution](#1a/b/solution)
- [2C](#2c)
  - [Solution](#2c/solution)
- [3F](#3f)
  - [Solution](#3f/solution)
- [4E](#4e)
  - [Solution](#4e/solution)
- [5A](#5a)
  - [a](#5a/a)
    - [Solution](#5a/a/solution)
  - [b](#5a/b)
    - [i](#5a/b/i)
      - [Solution](#5a/b/i/solution)
    - [ii](#5a/b/ii)
      - [Solution](#5a/b/ii/solution)
    - [iii](#5a/b/iii)
      - [Solution](#5a/b/iii/solution)
    - [iv](#5a/b/iv)
      - [Solution](#5a/b/iv/solution)
- [6B](#6b)
  - [a](#6b/a)
    - [i](#6b/a/i)
      - [Solution](#6b/a/i/solution)
    - [ii](#6b/a/ii)
      - [Solution](#6b/a/ii/solution)
  - [b](#6b/b)
    - [i](#6b/b/i)
      - [Solution](#6b/b/i/solution)
    - [ii](#6b/b/ii)
      - [Solution](#6b/b/ii/solution)
- [7B](#7b)
  - [a](#7b/a)
    - [Solution](#7b/a/solution)
  - [b](#7b/b)
    - [Solution](#7b/b/solution)
  - [c](#7b/c)
    - [Solution](#7b/c/solution)
- [8C](#8c)
  - [a](#8c/a)
    - [Solution](#8c/a/solution)
  - [b](#8c/b)
    - [Solution](#8c/b/solution)
- [9D](#9d)
  - [a](#9d/a)
    - [Solution](#9d/a/solution)
  - [b](#9d/b)
    - [Solution](#9d/b/solution)
  - [c](#9d/c)
    - [Solution](#9d/c/solution)
- [10D](#10d)
  - [a](#10d/a)
    - [Solution](#10d/a/solution)
  - [b](#10d/b)
    - [Solution](#10d/b/solution)
- [11F](#11f)
  - [a](#11f/a)
    - [Solution](#11f/a/solution)
  - [b](#11f/b)
    - [Solution](#11f/b/solution)
  - [c](#11f/c)
    - [Solution](#11f/c/solution)
  - [d](#11f/d)
    - [Solution](#11f/d/solution)
- [12E](#12e)
  - [Solution](#12e/solution)

## 1A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1a/a">a</h3>

↑ **Parent:** [1A](#1a)

<h4 id="1a/a/solution">Solution</h4>

↑ **Parent:** [A](#1a/a)

By [Euler's formula](../../../complex-analysis.md#euler-s-formula), $z=e^{i\theta}$. Factoring out the half-angle gives

$$
1+z=e^{i\theta/2}\left(e^{-i\theta/2}+e^{i\theta/2}\right)
=2\cos\frac\theta2\,e^{i\theta/2}.
$$

Since $0\leq\theta<\pi$, the cosine is positive. Therefore

$$
\boxed{|1+z|=2\cos\frac\theta2,
\qquad \arg(1+z)=\frac\theta2}.
$$

On the [Argand diagram](../../../complex-analysis.md#complex-plane), the points $0,1,z,1+z$ form a rhombus. Its diagonal from $0$ to $1+z$ bisects the angle between the unit vectors $1$ and $z$, so its direction is $\theta/2$; resolving either side along the diagonal gives its length $2\cos(\theta/2)$.

<h3 id="1a/b">b</h3>

↑ **Parent:** [1A](#1a)

<h4 id="1a/b/solution">Solution</h4>

↑ **Parent:** [B](#1a/b)

Similarly,

$$
1-z=e^{i\theta/2}\left(e^{-i\theta/2}-e^{i\theta/2}\right)
=-2i\sin\frac\theta2\,e^{i\theta/2}
=2\sin\frac\theta2\,e^{i(\theta/2-\pi/2)}.
$$

Thus, for $0<\theta<\pi$,

$$
\boxed{|1-z|=2\sin\frac\theta2,
\qquad \arg(1-z)=\frac\theta2-\frac\pi2}.
$$

At $\theta=0$, $1-z=0$, whose [complex argument](../../../complex-analysis.md#argument-complex-analysis) is undefined. Geometrically, $|1-z|$ is the chord joining the two unit-circle points $z$ and $1$. The isosceles triangle with vertex angle $\theta$ has half-chord $\sin(\theta/2)$, and the chord direction is perpendicular to the radius through its midpoint, giving the stated argument.

## 2C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2c/solution">Solution</h3>

↑ **Parent:** [2C](#2c)

Componentwise,

$$
[(AB)^T]_{ij}=(AB)_{ji}=\sum_kA_{jk}B_{ki}
=\sum_k(B^T)_{ik}(A^T)_{kj}=(B^TA^T)_{ij},
$$

so

$$
\boxed{(AB)^T=B^TA^T}.
$$

Repeated application gives $(A^k)^T=(A^T)^k$. Transposing the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) term by term therefore yields

$$
\boxed{(e^A)^T=e^{A^T}}.
$$

Multiplication of the two power series gives

$$
e^{tA}e^{tA^T}
=I+t(A+A^T)
+t^2\left(\frac12A^2+AA^T+\frac12(A^T)^2\right)+O(t^3).
$$

Hence

$$
\boxed{Q_0=I,\qquad Q_1=A+A^T,\qquad
Q_2=\frac12A^2+AA^T+\frac12(A^T)^2}.
$$

If $e^{tA}$ is an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) for every real $t$, then

$$
e^{tA}(e^{tA})^T=e^{tA}e^{tA^T}=I.
$$

Its coefficient of $t$ must vanish, so

$$
\boxed{A^T=-A};
$$

that is, $A$ is a [skew-symmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix).

## 3F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3f/solution">Solution</h3>

↑ **Parent:** [3F](#3f)

Because $(a_n)$ is a [monotone sequence](../../../real-analysis.md#monotone-sequence), every one of its first $n$ terms is at most $a_n$, so

$$
s_n\leq a_n.
$$

On the other hand, every term from $a_n$ through $a_{2n}$ is at least $a_n$, and hence

$$
a_n\leq\frac1{n+1}\sum_{k=n}^{2n}a_k
=\frac{2n s_{2n}-(n-1)s_{n-1}}{n+1}.
$$

Both the lower bound and upper bound tend to $x$ because the [Cesaro means](../../../real-analysis.md#cesaro-mean) converge to $x$. The [squeeze theorem](../../../calculus.md#squeeze-theorem) gives

$$
\boxed{a_n\longrightarrow x}.
$$

## 4E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4e/solution">Solution</h3>

↑ **Parent:** [4E](#4e)

Convergence at $z_0$ implies that the terms $a_nz_0^n$ form a [bounded sequence](../../../real-analysis.md#bounded-sequence): $|a_nz_0^n|\leq M$ for some $M$. If $|z|<|z_0|$ and $r=|z/z_0|<1$, then

$$
|a_nz^n|=|a_nz_0^n|r^n\leq Mr^n.
$$

Comparison with the convergent [geometric series](../../../real-analysis.md#geometric-series) $\sum Mr^n$ proves [absolute convergence](../../../real-analysis.md#absolute-convergence). The case $z_0=0$ is vacuous.

The [radius of convergence](../../../real-analysis.md#radius-of-convergence) is the number $R\in[0,\infty]$ such that a [power series](../../../real-analysis.md#power-series) converges absolutely for $|z|<R$ and diverges for $|z|>R$, with boundary behavior considered separately.

Take

$$
v=-1,\qquad w=1.
$$

Then $\sum v^n/n$ is the convergent [alternating harmonic series](../../../real-analysis.md#alternating-harmonic-series), whereas $\sum w^n/n$ is the divergent [harmonic series](../../../real-analysis.md#harmonic-series). Thus $\sum z^n/n$ converges at a point of modulus one and diverges at another point of modulus one. It follows that

$$
\boxed{R=1}.
$$

## 5A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5a/a">a</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/a/solution">Solution</h4>

↑ **Parent:** [A](#5a/a)

The [cross product](../../../vector-space.md#cross-product) $x\times y$ is the vector perpendicular to $x$ and $y$, of magnitude $|x||y|\sin\alpha$ and orientation fixed by the right-hand rule. In [suffix notation](../../../linear-algebra.md#einstein-notation),

$$
(x\times y)_i=\varepsilon_{ijk}x_jy_k,
$$

where $\varepsilon_{ijk}$ is the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol). Therefore

$$
[x\times(x\times y)]_i
=\varepsilon_{ijk}x_j\varepsilon_{klm}x_ly_m.
$$

Using

$$
\varepsilon_{ijk}\varepsilon_{klm}
=\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl}
$$

gives

$$
[x\times(x\times y)]_i=x_i x_jy_j-y_i x_jx_j.
$$

Hence the [vector triple product identity](../../../calculus.md#vector-triple-product) is

$$
\boxed{x\times(x\times y)=x(x\mathbin{\cdot}y)-y(x\mathbin{\cdot}x)}.
$$

<h3 id="5a/b">b</h3>

↑ **Parent:** [5A](#5a)

<h4 id="5a/b/i">i</h4>

↑ **Parent:** [B](#5a/b)

<h5 id="5a/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5a/b/i)

The identity in part (a), together with $|a|=1$, gives

$$
\boxed{x_2=\lambda^2\left[a(a\mathbin{\cdot}x_0)-x_0\right]}.
$$

For every $n\geq1$, $x_n$ is perpendicular to $a$, because it is a scalar multiple of $a\times x_{n-1}$. Therefore

$$
\boxed{x_{n+2}=\lambda^2a\times(a\times x_n)=-\lambda^2x_n}.
$$

Also $|x_1|=\lambda|a\times x_0|$ and $|x_2|=\lambda^2|a\times x_0|$. Induction using the two-step recurrence yields

$$
\boxed{|x_n|=\lambda^n|a\times x_0|\qquad(n\geq1)}.
$$

<h4 id="5a/b/ii">ii</h4>

↑ **Parent:** [B](#5a/b)

<h5 id="5a/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5a/b/ii)

The recurrence $x_{n+2}=-\lambda^2x_n$ shows that every odd-indexed position vector is a scalar multiple of $x_1$, while every positive even-indexed position vector is a scalar multiple of $x_2$. Hence

$$
\boxed{X_1,X_3,X_5,\ldots\text{ lie on }\mathbb Rx_1,
\quad X_2,X_4,X_6,\ldots\text{ lie on }\mathbb Rx_2}.
$$

Moreover $x_2=\lambda a\times x_1$, so these two straight lines through the origin are perpendicular.

<h4 id="5a/b/iii">iii</h4>

↑ **Parent:** [B](#5a/b)

<h5 id="5a/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5a/b/iii)

Let $d_n=x_{n+1}-x_n$ be the direction vector of the segment $X_nX_{n+1}$. Consecutive vectors $x_n,x_{n+1}$ are perpendicular and $|x_{n+1}|=\lambda|x_n|$. Using $x_{n+2}=-\lambda^2x_n$,

$$
d_n\mathbin{\cdot}d_{n+1}
=(x_{n+1}-x_n)\mathbin{\cdot}(x_{n+2}-x_{n+1})
=-|x_{n+1}|^2+\lambda^2|x_n|^2=0.
$$

Thus adjacent segments are perpendicular. Also

$$
d_{n+2}=x_{n+3}-x_{n+2}=-\lambda^2(x_{n+1}-x_n)=-\lambda^2d_n,
$$

so

$$
\boxed{X_nX_{n+1}\parallel X_{n+2}X_{n+3}}.
$$

If $0<\lambda<1$, the norm formula in part (i) gives $x_n\to0$. If $\lambda=1$, then $x_{n+2}=-x_n$: the points $X_1,X_2,-X_1,-X_2$ repeat cyclically and form a square centered at the origin.

<h4 id="5a/b/iv">iv</h4>

↑ **Parent:** [B](#5a/b)

<h5 id="5a/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#5a/b/iv)

Put $L=|x_n|$ and choose perpendicular unit vectors $e,f$ such that $x_n=Le$ and $x_{n+1}=\lambda Lf$. Direction vectors for the two lines are

$$
x_{n+2}-x_{n+1}=-\lambda L(\lambda e+f)
$$

and

$$
x_{n+3}-x_n=-L(e+\lambda^3f).
$$

Their scalar product and norms give

$$
\cos\theta
=\frac{\lambda^2L^2(1+\lambda^2)}
{\lambda L^2\sqrt{1+\lambda^2}\sqrt{1+\lambda^6}}.
$$

Therefore the acute angle between the straight lines satisfies

$$
\boxed{\cos\theta
=\frac{\lambda\sqrt{1+\lambda^2}}{\sqrt{1+\lambda^6}}}.
$$

## 6B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6b/a">a</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/a/i">i</h4>

↑ **Parent:** [A](#6b/a)

<h5 id="6b/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6b/a/i)

A matrix and its [matrix transpose](../../../vector-space.md#transpose) have the same [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial), because

$$
\det(\lambda I-A^T)=\det[(\lambda I-A)^T]=\det(\lambda I-A).
$$

Thus they have the same [eigenvalues](../../../linear-operator-theory.md#eigenvalue), including algebraic multiplicities.

The proposed sum identity is false. For

$$
A=\begin{pmatrix}0&1\\0&0\end{pmatrix},
$$

both eigenvalues $\lambda_i$ are zero, whereas

$$
A^TA=\begin{pmatrix}0&0\\0&1\end{pmatrix}
$$

has eigenvalues $0,1$. Hence

$$
\boxed{\sum_i\mu_i=1\ne0=\sum_i\lambda_i^2}.
$$

Equivalently, the two sides are generally $\operatorname{tr}(A^TA)$ and $\operatorname{tr}(A^2)$, which need not agree.

<h4 id="6b/a/ii">ii</h4>

↑ **Parent:** [A](#6b/a)

<h5 id="6b/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6b/a/ii)

The product identity always holds, since

$$
\prod_i\mu_i=\det(A^TA)=\det(A^T)\det A=(\det A)^2
=\left(\prod_i\lambda_i\right)^2.
$$

Therefore

$$
\boxed{\prod_{i=1}^n\mu_i=\prod_{i=1}^n\lambda_i^2}.
$$

<h3 id="6b/b">b</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/b/i">i</h4>

↑ **Parent:** [B](#6b/b)

<h5 id="6b/b/i/solution">Solution</h5>

↑ **Parent:** [I](#6b/b/i)

If $p=m\times n$, then $n^Tp=0$, and hence $Bp=p$. Also $Bm=m$ because $m\perp n$. Thus $p$ and $m$ are linearly independent eigenvectors with eigenvalue one.

For every vector $v$,

$$
(B-I)v=m(n^Tv),
$$

so $B-I$ is nonzero but has square zero:

$$
(B-I)^2=mn^Tmn^T=0.
$$

Consequently all three eigenvalues are one. The eigenspace is

$$
\ker(B-I)=\{v:n^Tv=0\}=n^\perp,
$$

which has dimension two. It cannot supply three linearly independent eigenvectors, so

$$
\boxed{B\text{ has eigenvalues }1,1,1\text{ and is not diagonalizable}.}
$$

<h4 id="6b/b/ii">ii</h4>

↑ **Parent:** [B](#6b/b)

<h5 id="6b/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6b/b/ii)

Multiplication gives

$$
B^TB=(I+nm^T)(I+mn^T)=I+mn^T+nm^T+nn^T.
$$

The vector $p=m\times n$ is an eigenvector with eigenvalue one. On the plane spanned by the orthonormal pair $m,n$, the matrix is

$$
\begin{pmatrix}1&1\\1&2\end{pmatrix}.
$$

Its eigenvalues are the roots of $\mu^2-3\mu+1$, namely

$$
\mu_\pm=\frac{3\pm\sqrt5}{2}.
$$

For either root, an eigenvector is $m+(\mu_\pm-1)n$. Therefore

$$
\boxed{
\begin{array}{c|c}
\text{eigenvector}&\text{eigenvalue}\\ \hline
m\times n&1\\
m+\frac{1+\sqrt5}{2}n&\frac{3+\sqrt5}{2}\\
m+\frac{1-\sqrt5}{2}n&\frac{3-\sqrt5}{2}
\end{array}}
$$

These positive eigenvalues are the squared [singular values](../../../linear-algebra.md#singular-value) of $B$.

## 7B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7b/a">a</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/a/solution">Solution</h4>

↑ **Parent:** [A](#7b/a)

If $A^T=-A$, then the scalar $x^TAx$ equals its own transpose and hence

$$
x^TAx=(x^TAx)^T=x^TA^Tx=-x^TAx,
$$

so it vanishes.

Conversely, suppose $x^TAx=0$ for every real $x$. Taking $x=e_i$ gives $A_{ii}=0$. Taking $x=e_i+e_j$ then gives $A_{ij}+A_{ji}=0$. Thus every entry satisfies $A^T=-A$, and

$$
\boxed{x^TAx=0\text{ for all }x\quad\Longleftrightarrow\quad A\text{ is skew-symmetric}.}
$$

<h3 id="7b/b">b</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/b/solution">Solution</h4>

↑ **Parent:** [B](#7b/b)

A real [skew-symmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix) satisfies $A^\dagger=A^T=-A$, so it is a [skew-Hermitian matrix](../../../linear-operator-theory.md#skew-hermitian-matrix). If $Ax=\lambda x$, then

$$
\lambda\,x^\dagger x=x^\dagger Ax.
$$

Taking the [complex conjugate](../../../complex-analysis.md#complex-conjugate) and using $A^\dagger=-A$ shows that this scalar is the negative of its conjugate. Hence

$$
\boxed{\lambda^*=-\lambda},
$$

so every eigenvalue is purely imaginary or zero.

If $Ax=\lambda x$ and $Ay=\mu y$, then

$$
\lambda^*x^\dagger y=(Ax)^\dagger y=x^\dagger A^\dagger y=-\mu x^\dagger y.
$$

Since $\lambda^*=-\lambda$, this becomes $(\mu-\lambda)x^\dagger y=0$. Distinct eigenvalues therefore have orthogonal eigenvectors:

$$
\boxed{\lambda\ne\mu\implies x^\dagger y=0}.
$$

<h3 id="7b/c">c</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/c/solution">Solution</h4>

↑ **Parent:** [C](#7b/c)

In odd dimension,

$$
\det A=\det A^T=\det(-A)=-\det A,
$$

so $\det A=0$. Since $A$ is real, its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) contains a nonzero real vector $a$.

The plane $a^\perp$ is invariant under $A$, because $a\mathbin{\cdot}Ab=-(Aa)\mathbin{\cdot}b=0$. On this two-dimensional plane, $Ab$ is perpendicular to $b$. Put $|Ab|=\theta|b|$ with $\theta>0$. Then $A^2b$ is parallel to $b$, and

$$
b\mathbin{\cdot}A^2b=-(Ab)\mathbin{\cdot}(Ab)=-\theta^2|b|^2,
$$

so

$$
\boxed{A^2b=-\theta^2b}.
$$

The [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) fixes the kernel vector:

$$
\boxed{e^Aa=a}.
$$

Separating even and odd powers in its series and using $A^{2j}b=(-1)^j\theta^{2j}b$ gives

$$
\boxed{e^Ab=\cos\theta\,b+\frac{\sin\theta}{\theta}Ab}.
$$

Thus $e^A$ acts as a rotation through angle $\theta$ on $a^\perp$ and fixes its axis $\mathbb Ra$.

## 8C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8c/a">a</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/a/solution">Solution</h4>

↑ **Parent:** [A](#8c/a)

Write $y=(y_1,y_2,y_3)^T$. From the coordinate formula for the [cross product](../../../vector-space.md#cross-product),

$$
\boxed{T=
\begin{pmatrix}
1&y_3&-y_2\\
-y_3&0&y_1\\
y_2&-y_1&0
\end{pmatrix}}.
$$

If $y=c_1e_1$, this becomes

$$
\begin{pmatrix}1&0&0\\0&0&c_1\\0&-c_1&0\end{pmatrix}.
$$

Thus $c_1\ne0$ gives rank three and a zero-dimensional kernel, while $c_1=0$ gives rank one and kernel dimension two.

If $y\mathbin{\cdot}e_1=0$, then $y_1=0$. When $y\ne0$, the equations $Tx=0$ force $x_1=0$ and $y_3x_2-y_2x_3=0$, so

$$
\ker T=\mathbb Ry,
\qquad \operatorname{rank}T=2.
$$

When $y=0$, again $\operatorname{rank}T=1$ and $\dim\ker T=2$. These dimensions also agree with the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem).

<h3 id="8c/b">b</h3>

↑ **Parent:** [8C](#8c)

<h4 id="8c/b/solution">Solution</h4>

↑ **Parent:** [B](#8c/b)

First compute

$$
AB=\begin{pmatrix}
-2&2&2\\
-3&-7&-1\\
-1&-4&-1
\end{pmatrix}.
$$

The vector $\ell=(1,-2,4)^T$ lies in the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) of $(AB)^T$, since $\ell^TAB=0$. If $ABx=d$ is solvable, multiplying by $\ell^T$ gives the necessary compatibility condition

$$
0=\ell^Td=1-2+4k.
$$

Therefore

$$
\boxed{4k=1}.
$$

## 9D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9d/a">a</h3>

↑ **Parent:** [9D](#9d)

<h4 id="9d/a/solution">Solution</h4>

↑ **Parent:** [A](#9d/a)

The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) states that if $f:[a,b]\to\mathbb R$ is [continuous](../../../calculus.md#continuous-function) and $y$ lies between $f(a)$ and $f(b)$, then there exists $c\in[a,b]$ such that $f(c)=y$.

<h3 id="9d/b">b</h3>

↑ **Parent:** [9D](#9d)

<h4 id="9d/b/solution">Solution</h4>

↑ **Parent:** [B](#9d/b)

A function is [differentiable](../../../analysis.md#differentiable-function) at $a$ when the finite [limit](../../../calculus.md#limit-of-a-function)

$$
f'(a)=\lim_{h\to0}\frac{f(a+h)-f(a)}h
$$

exists. A derivative need not be continuous. For example,

$$
f(x)=\begin{cases}x^2\sin(1/x),&x\ne0,\\0,&x=0,
\end{cases}
$$

is differentiable everywhere and $f'(0)=0$, but for $x\ne0$,

$$
f'(x)=2x\sin(1/x)-\cos(1/x),
$$

which has no limit at zero.

The [mean value theorem](../../../calculus.md#mean-value-theorem) states that if $f$ is continuous on $[a,b]$ and differentiable on $(a,b)$, then some $c\in(a,b)$ satisfies

$$
f'(c)=\frac{f(b)-f(a)}{b-a}.
$$

<h3 id="9d/c">c</h3>

↑ **Parent:** [9D](#9d)

<h4 id="9d/c/solution">Solution</h4>

↑ **Parent:** [C](#9d/c)

Set $h(x)=f(x)-yx$. Then

$$
h'(a)=f'(a)-y\leq0,
\qquad h'(b)=f'(b)-y\geq0.
$$

The [extreme value theorem](../../../real-analysis.md#extreme-value-theorem) gives a minimum of $h$ on $[a,b]$. If it occurs in $(a,b)$, the two-sided difference quotient gives $h'(c)=0$. If it occurs at $a$, either $h'(a)=0$ or a negative right derivative contradicts minimality; the endpoint $b$ is analogous. Hence some $c\in[a,b]$ satisfies

$$
\boxed{f'(c)=y}.
$$

This proves the [Darboux theorem for derivatives](../../../calculus.md#darboux-s-theorem-analysis) in the stated case without assuming that $f'$ is continuous.

Because a differentiable function is continuous, define

$$
F(x)=f(x)+\int_a^x f(t)\,dt.
$$

The [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) gives $F'(x)=f'(x)+f(x)$. At the endpoints,

$$
F'(a)=f'(a)+f(a)\leq f'(a)\leq y,
$$

while

$$
F'(b)=f'(b)+f(b)\geq f'(b)\geq y.
$$

Applying the result just proved to $F$ yields $d\in[a,b]$ with

$$
\boxed{f'(d)+f(d)=y}.
$$

## 10D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10d/a">a</h3>

↑ **Parent:** [10D](#10d)

<h4 id="10d/a/solution">Solution</h4>

↑ **Parent:** [A](#10d/a)

The function $f$ is [continuous](../../../calculus.md#continuous-function) at $y_0$ when for every $\varepsilon>0$ there is a $\delta>0$ such that

$$
|x-y_0|<\delta\quad\Longrightarrow\quad|f(x)-f(y_0)|<\varepsilon.
$$

Suppose $f$ has a [local minimum](../../../analysis.md#local-minimum) at $c$ and is differentiable there. For sufficiently small $h>0$,

$$
\frac{f(c+h)-f(c)}h\geq0,
\qquad
\frac{f(c-h)-f(c)}{-h}\leq0.
$$

Both one-sided limits equal $f'(c)$, so it is both nonnegative and nonpositive. Therefore

$$
\boxed{f'(c)=0}.
$$

<h3 id="10d/b">b</h3>

↑ **Parent:** [10D](#10d)

<h4 id="10d/b/solution">Solution</h4>

↑ **Parent:** [B](#10d/b)

The upper bound follows immediately from [convexity](../../../real-analysis.md#convex-function), since

$$
y_0+\lambda r=(1-\lambda)y_0+\lambda(y_0+r).
$$

For the lower bound, write

$$
y_0=\frac1{1+\lambda}(y_0+\lambda r)
+\frac\lambda{1+\lambda}(y_0-r).
$$

Applying convexity and rearranging gives

$$
\boxed{(1+\lambda)f(y_0)-\lambda f(y_0-r)
\leq f(y_0+\lambda r)
\leq(1-\lambda)f(y_0)+\lambda f(y_0+r)}.
$$

Choose a fixed $r_0>0$ with $[y_0-r_0,y_0+r_0]\subset(a,b)$. Applying these bounds with $r=r_0$ and $r=-r_0$ shows that the difference $f(y_0+h)-f(y_0)$ is trapped between quantities of order $|h|/r_0$. Both tend to zero, so every [convex function](../../../real-analysis.md#convex-function) on an open interval is continuous.

Now suppose $c$ is a local minimum but some $x$ satisfies $f(x)<f(c)$. For sufficiently small $\lambda>0$, the point $z=(1-\lambda)c+\lambda x$ lies in the neighbourhood on which $c$ is minimal, whereas convexity gives

$$
f(z)\leq(1-\lambda)f(c)+\lambda f(x)<f(c),
$$

a contradiction. Thus

$$
\boxed{f(x)\geq f(c)\text{ for every }x\in(a,b)}.
$$

Differentiability at the minimizer is unnecessary: $f(x)=|x-c|$ is convex, has its global minimum at $c$, and is not differentiable there.

## 11F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11f/a">a</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/a/solution">Solution</h4>

↑ **Parent:** [A](#11f/a)

For each $k\geq0$, monotonicity gives the dyadic-block bounds

$$
2^k x_{2^{k+1}}
\leq\sum_{n=2^k}^{2^{k+1}-1}x_n
\leq2^k x_{2^k}.
$$

Summing the upper bounds proves convergence of $\sum x_n$ whenever $\sum2^kx_{2^k}$ converges. Summing the lower bounds gives, up to the first term,

$$
\sum_{k\geq0}2^kx_{2^{k+1}}
=\frac12\sum_{j\geq1}2^jx_{2^j},
$$

so convergence of $\sum x_n$ forces convergence of the condensed series. This is the [Cauchy condensation test](../../../real-analysis.md#cauchy-condensation-test):

$$
\boxed{\sum_{n\geq1}x_n\text{ converges}
\iff\sum_{k\geq0}2^kx_{2^k}\text{ converges}.}
$$

<h3 id="11f/b">b</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/b/solution">Solution</h4>

↑ **Parent:** [B](#11f/b)

If $s\leq0$, the terms $n^{-s}$ do not tend to zero, so the series diverges by the [term test for divergence](../../../real-analysis.md#term-test-for-divergence). If $s>0$, the terms form a nonnegative decreasing sequence, and the [Cauchy condensation test](../../../real-analysis.md#cauchy-condensation-test) gives the condensed series

$$
\sum_{k=0}^{\infty}2^k(2^k)^{-s}
=\sum_{k=0}^{\infty}2^{k(1-s)}.
$$

This [geometric series](../../../real-analysis.md#geometric-series) converges exactly when $1-s<0$. Hence the [p-series](../../../real-analysis.md#p-series) criterion is

$$
\boxed{\sum_{n=1}^{\infty}n^{-s}\text{ converges}\iff s>1}.
$$

<h3 id="11f/c">c</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/c/solution">Solution</h4>

↑ **Parent:** [C](#11f/c)

For $u_n=2^{-n}n^k$,

$$
\frac{u_{n+1}}{u_n}=\frac12\left(1+\frac1n\right)^k\longrightarrow\frac12.
$$

Thus for all sufficiently large $n$ the ratio is, for example, at most $3/4$. Comparison with a decaying [geometric sequence](../../../real-analysis.md#geometric-progression), equivalently the [ratio test](../../../real-analysis.md#ratio-test), yields

$$
\boxed{\lim_{n\to\infty}2^{-n}n^k=0}.
$$

<h3 id="11f/d">d</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/d/solution">Solution</h4>

↑ **Parent:** [D](#11f/d)

We first prove by induction that

$$
a_n\geq2^n\qquad(n\geq1).
$$

It holds for $n=1$, and if it holds at $n$, then

$$
a_{n+1}=2^{a_n}\geq2^{2^n}\geq2^{n+1}.
$$

Consequently

$$
0\leq\frac{2n^k}{a_n}\leq2^{1-n}n^k.
$$

Part (c) and the [squeeze theorem](../../../calculus.md#squeeze-theorem) now give

$$
\boxed{\lim_{n\to\infty}\frac{2n^k}{a_n}=0}.
$$

## 12E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12e/solution">Solution</h3>

↑ **Parent:** [12E](#12e)

Let $L$ be the supremum of all [lower Darboux sums](../../../real-analysis.md#lower-darboux-sum) and $U$ the infimum of all [upper Darboux sums](../../../real-analysis.md#upper-darboux-sum). The assumed comparison of arbitrary lower and upper sums gives $L\leq U$. For the partition supplied for a given $\varepsilon$,

$$
0\leq U-L\leq S_{\mathcal D}(f)-s_{\mathcal D}(f)<\varepsilon.
$$

Since this holds for every positive $\varepsilon$, $U=L$. Thus the [Riemann integrability criterion](../../../real-analysis.md#riemann-integrability-criterion) gives

$$
\boxed{f\text{ is Riemann integrable}.}
$$

If $f$ is continuous on $[a,b]$, the [Heine-Cantor theorem](../../../topological-analysis.md#heine-cantor-theorem) makes it uniformly continuous. Given $\varepsilon>0$, choose $\delta$ so that intervals of length below $\delta$ have oscillation below $\varepsilon/(b-a)$. A partition of mesh below $\delta$ then satisfies

$$
S_{\mathcal D}(f)-s_{\mathcal D}(f)<\varepsilon,
$$

proving that [Continuous functions are Riemann integrable](../../../real-analysis.md#continuous-functions-are-riemann-integrable).

For the function defined using $g$, choose $K$ with $|f|\leq K$. Given $\varepsilon>0$, choose $\delta>0$ so small that $2K\delta<\varepsilon/2$. On $[\delta,1]$, the function $g$ is continuous and therefore has a partition whose upper-minus-lower sum is below $\varepsilon/2$. Adding the interval $[0,\delta]$ contributes at most $2K\delta$, regardless of the value $f(0)=\lambda$. Hence the full Darboux-sum difference is below $\varepsilon$, and

$$
\boxed{f\text{ is Riemann integrable for every }\lambda\in\mathbb R}.
$$

Finally, for any partition $a=x_0<\cdots<x_n=b$, the [mean value theorem](../../../calculus.md#mean-value-theorem) supplies $\xi_i\in(x_{i-1},x_i)$ such that

$$
f(x_i)-f(x_{i-1})=f'(\xi_i)(x_i-x_{i-1}).
$$

Summing telescopes to

$$
f(b)-f(a)=\sum_{i=1}^nf'(\xi_i)(x_i-x_{i-1}),
$$

a [Riemann sum](../../../real-analysis.md#riemann-sum) for the Riemann-integrable function $f'$. Equivalently, every lower derivative sum is at most this telescoping value and every upper derivative sum is at least it. Taking the common [upper and lower Darboux integrals](../../../real-analysis.md#upper-and-lower-darboux-integrals) proves the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) conclusion

$$
\boxed{\int_a^bf'(x)\,dx=f(b)-f(a)}.
$$

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
