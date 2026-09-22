# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2021/paperia_1_2021.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2021/paperia_1_2021.pdf)

**Table of contents**

- [1C](#1c)
  - [a](#1c/a)
    - [Solution](#1c/a/solution)
  - [b](#1c/b)
    - [Solution](#1c/b/solution)
- [2B](#2b)
  - [Solution](#2b/solution)
- [3F](#3f)
  - [Solution](#3f/solution)
- [4F](#4f)
  - [Solution](#4f/solution)
- [5C](#5c)
  - [Solution](#5c/solution)
- [6A](#6a)
  - [a](#6a/a)
    - [Solution](#6a/a/solution)
  - [b](#6a/b)
    - [Solution](#6a/b/solution)
  - [c](#6a/c)
    - [i](#6a/c/i)
      - [Solution](#6a/c/i/solution)
    - [ii](#6a/c/ii)
      - [Solution](#6a/c/ii/solution)
  - [d](#6a/d)
    - [Solution](#6a/d/solution)
- [7A](#7a)
  - [Solution](#7a/solution)
- [8B](#8b)
  - [a](#8b/a)
    - [Solution](#8b/a/solution)
  - [b](#8b/b)
    - [i](#8b/b/i)
      - [Solution](#8b/b/i/solution)
    - [ii](#8b/b/ii)
      - [Solution](#8b/b/ii/solution)
    - [iii](#8b/b/iii)
      - [Solution](#8b/b/iii/solution)
- [9F](#9f)
  - [a](#9f/a)
    - [Solution](#9f/a/solution)
  - [b](#9f/b)
    - [i](#9f/b/i)
      - [Solution](#9f/b/i/solution)
    - [ii](#9f/b/ii)
      - [Solution](#9f/b/ii/solution)
    - [iii](#9f/b/iii)
      - [Solution](#9f/b/iii/solution)
    - [iv](#9f/b/iv)
      - [Solution](#9f/b/iv/solution)
- [10F](#10f)
  - [a](#10f/a)
    - [Solution](#10f/a/solution)
  - [b](#10f/b)
    - [Solution](#10f/b/solution)
- [11F](#11f)
  - [a](#11f/a)
    - [Solution](#11f/a/solution)
  - [b](#11f/b)
    - [Solution](#11f/b/solution)
- [12F](#12f)
  - [a](#12f/a)
    - [i](#12f/a/i)
      - [Solution](#12f/a/i/solution)
    - [ii](#12f/a/ii)
      - [Solution](#12f/a/ii/solution)
    - [iii](#12f/a/iii)
      - [Solution](#12f/a/iii/solution)
  - [b](#12f/b)
    - [Solution](#12f/b/solution)

## 1C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1c/a">a</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/a/solution">Solution</h4>

↑ **Parent:** [A](#1c/a)

By [complex exponentiation](../../../analysis.md#complex-exponentiation), a value of $z^i$ has the form

$$
\exp\left(i\bigl(\log|z|+i(\arg z+2\pi k)\bigr)\right).
$$

For this to equal one, its exponent must be $2\pi in$ for some $n\in\mathbb Z$. Hence a logarithm of $z$ must equal $2\pi n$, so $z$ is positive real and

$$
\boxed{z=e^{2\pi n},\qquad n\in\mathbb Z}.
$$

With the principal branch this is the same list; in the multivalued convention these are precisely the $z$ for which one value of $z^i$ equals one.

<h3 id="1c/b">b</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/b/solution">Solution</h4>

↑ **Parent:** [B](#1c/b)

The circle is

$$
\boxed{|z-5i|=5}.
$$

The direction from its center $c=5i$ to $z_0=15/4$ is

$$
z_0-c=\frac{15}{4}-5i,
\qquad
|z_0-c|=\frac{25}{4},
$$

so the corresponding unit direction is $3/5-4i/5$. Moving a distance five from the center in the two directions gives

$$
z=5i\pm5\left(\frac35-\frac45i\right).
$$

Thus the intersections are

$$
\boxed{z=3+i\quad\text{and}\quad z=-3+9i}.
$$

## 2B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2b/solution">Solution</h3>

↑ **Parent:** [2B](#2b)

Let $P_B,P_{B'},P_C,P_{C'}$ have the corresponding basis vectors as columns in standard coordinates. From the PDF,

$$
P_B=\begin{pmatrix}0&-2\\2&0\end{pmatrix},
\quad
P_{B'}=\begin{pmatrix}1&1\\1&-1\end{pmatrix},
\quad
P_C=\begin{pmatrix}1&0&0\\1&1&0\\0&0&1\end{pmatrix},
\quad
P_{C'}=I_3.
$$

The [matrix representation of a linear map](../../../vector-space.md#matrix-representation-of-a-linear-map) in standard coordinates is $P_CAP_B^{-1}$. The [change of basis](../../../linear-algebra.md#change-of-basis) formula therefore gives

$$
A'=P_{C'}^{-1}P_CAP_B^{-1}P_{B'}.
$$

Multiplication yields

$$
\boxed{
A'=
\begin{pmatrix}
3/2&-1/2\\
5/2&-3/2\\
-1&0
\end{pmatrix}}.
$$

## 3F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3f/solution">Solution</h3>

↑ **Parent:** [3F](#3f)

The [alternating series test](../../../real-analysis.md#alternating-series-test) says that if $a_n\geq0$, $a_{n+1}\leq a_n$, and $a_n\to0$, then $\sum_{n\geq1}(-1)^{n+1}a_n$ converges.

To prove it, let $S_N$ be the partial sums. The even sums satisfy

$$
S_{2m+2}-S_{2m}
=a_{2m+1}-a_{2m+2}\geq0,
$$

so $(S_{2m})$ is increasing. The odd sums satisfy

$$
S_{2m+3}-S_{2m+1}
=-a_{2m+2}+a_{2m+3}\leq0,
$$

so $(S_{2m+1})$ is decreasing. Also $S_{2m}\leq S_{2m+1}$, so both are bounded and converge. Their difference is $a_{2m+1}\to0$, hence their limits agree and the whole sequence $(S_N)$ converges.

Taking $a_n=1/n$ proves convergence of the [alternating harmonic series](../../../real-analysis.md#alternating-harmonic-series). Its even partial sums lie below its limit $S$, while its odd partial sums lie above it. Since

$$
S_4=1-\frac12+\frac13-\frac14=\frac7{12}
$$

and

$$
S_5=S_4+\frac15=\frac{47}{60},
$$

we obtain

$$
\boxed{\frac7{12}\leq S\leq\frac{47}{60}}.
$$

## 4F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4f/solution">Solution</h3>

↑ **Parent:** [4F](#4f)

The [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) states that every bounded sequence of real numbers has a convergent subsequence.

For a proof, place all terms in a closed bounded interval $I_1$. Bisect it and choose a closed half $I_2$ containing infinitely many terms. Continue inductively, choosing nested closed intervals

$$
I_1\supseteq I_2\supseteq\cdots
$$

with infinitely many sequence terms and with lengths tending to zero. Choose $n_k>n_{k-1}$ such that $x_{n_k}\in I_k$. The [nested interval theorem](../../../real-analysis.md#nested-interval-theorem) gives a unique point $x$ in every $I_k$. Because both $x_{n_k}$ and $x$ lie in $I_k$,

$$
|x_{n_k}-x|\leq |I_k|\longrightarrow0.
$$

Thus $(x_{n_k})$ is a convergent subsequence.

Now suppose every convergent subsequence of the bounded sequence $(x_n)$ converges to $L$. If $x_n$ did not converge to $L$, there would be an $\epsilon>0$ and a subsequence $(x_{n_k})$ satisfying

$$
|x_{n_k}-L|\geq\epsilon
$$

for every $k$. This subsequence is bounded, so Bolzano--Weierstrass gives a convergent subsubsequence. By hypothesis its limit is $L$, contradicting the displayed inequality. Hence the [unique subsequential limit of a bounded sequence](../../../real-analysis.md#unique-subsequential-limit-of-a-bounded-sequence) principle gives

$$
\boxed{x_n\to L}.
$$

## 5C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5c/solution">Solution</h3>

↑ **Parent:** [5C](#5c)

Using [Einstein notation](../../../linear-algebra.md#einstein-notation) and

$$
\epsilon_{ijk}\epsilon_{klm}
=\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl},
$$

we obtain

$$
\begin{aligned}
[a\times(b\times c)]_i
&=\epsilon_{ijk}a_j\epsilon_{klm}b_lc_m\\
&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})
a_jb_lc_m\\
&=(a\cdot c)b_i-(a\cdot b)c_i.
\end{aligned}
$$

Thus

$$
\boxed{a\times(b\times c)=(a\cdot c)b-(a\cdot b)c}.
$$

The [scalar triple product](../../../linear-algebra.md#scalar-triple-product) is

$$
[a,b,c]=a\cdot(b\times c).
$$

Put $\Delta=[a,b,c]$. When $\Delta\ne0$, the three vectors

$$
e'_1=\frac{b\times c}{\Delta},
\qquad
e'_2=\frac{c\times a}{\Delta},
\qquad
e'_3=\frac{a\times b}{\Delta}
$$

form the [reciprocal basis](../../../linear-algebra.md#reciprocal-basis) to $a,b,c$, so $e'_i\cdot e_j=\delta_{ij}$. Their scalar triple product is $1/\Delta$. Therefore

$$
[a\times b,b\times c,c\times a]
=\Delta^3[e'_3,e'_1,e'_2]
=\boxed{\Delta^2},
$$

since the cyclic permutation preserves orientation. The identity also holds when $\Delta=0$, either by continuity or directly because the cross products are then linearly dependent.

For the given basis $e_1,e_2,e_3$, the same identities give

$$
e'_i\cdot e_j=\delta_{ij}.
$$

If $\sum_i\alpha_ie'_i=0$, dotting with $e_j$ gives $\alpha_j=0$, so the $e'_i$ are linearly independent and hence form a basis. Moreover, $e_i\cdot e'_j=\delta_{ij}$, so the original basis is reciprocal to the primed basis. Uniqueness of a reciprocal basis gives

$$
\boxed{e''_i=e_i\qquad(i=1,2,3)}.
$$

Every vector $K$ has a unique expansion $K=\sum_i\kappa_ie'_i$, and then

$$
K\cdot R
=\sum_{i,j}\kappa_i n_j e'_i\cdot e_j
=\sum_i\kappa_i n_i.
$$

This is an integer for every integer triple $(n_1,n_2,n_3)$ exactly when every $\kappa_i$ is an integer. Hence all such points are

$$
\boxed{K=m_1e'_1+m_2e'_2+m_3e'_3,
\qquad m_1,m_2,m_3\in\mathbb Z}.
$$

They form the reciprocal lattice in the convention without a factor of $2\pi$.

## 6A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6a/a">a</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/a/solution">Solution</h4>

↑ **Parent:** [A](#6a/a)

Using the convention of the question, the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) and characteristic equation are

$$
\chi_A(z)=\det(A-zI),
\qquad
\chi_A(z)=0.
$$

For

$$
A=\begin{pmatrix}a&b\\c&d\end{pmatrix},
$$

one has

$$
\chi_A(z)=z^2-(a+d)z+(ad-bc).
$$

Direct multiplication gives

$$
A^2-(a+d)A+(ad-bc)I=0,
$$

entry by entry. Thus $\chi_A(A)=0$, verifying the [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) for $2\times2$ matrices.

<h3 id="6a/b">b</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/b/solution">Solution</h4>

↑ **Parent:** [B](#6a/b)

If $A_{ji}$ denotes the matrix obtained by deleting row $j$ and column $i$, then the [adjugate matrix](../../../linear-algebra.md#adjugate-matrix) is

$$
\operatorname{adj}(A)_{ij}
=(-1)^{i+j}\det A_{ji}.
$$

For nonsingular $A$,

$$
\operatorname{adj}(A)=\det(A)A^{-1}.
$$

Therefore, when $A$ and $B$ are nonsingular,

$$
\begin{aligned}
\operatorname{adj}(AB)
&=\det(A)\det(B)(AB)^{-1}\\
&=\det(B)B^{-1}\det(A)A^{-1}\\
&=\boxed{\operatorname{adj}(B)\operatorname{adj}(A)}.
\end{aligned}
$$

<h3 id="6a/c">c</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/c/i">i</h4>

↑ **Parent:** [C](#6a/c)

<h5 id="6a/c/i/solution">Solution</h5>

↑ **Parent:** [I](#6a/c/i)

The determinant $\det(M-tI)$ is a polynomial in $t$ with leading term $(-t)^n$, so it is not the zero polynomial and has only finitely many roots. Hence one may choose $\alpha>0$ smaller than every positive root, if any. Then

$$
\boxed{M-tI\text{ is nonsingular for }0<t<\alpha}.
$$

<h4 id="6a/c/ii">ii</h4>

↑ **Parent:** [C](#6a/c)

<h5 id="6a/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6a/c/ii)

Each entry of $\operatorname{adj}(M-tI)$ is, up to sign, the determinant of an $(n-1)\times(n-1)$ minor whose entries are affine polynomials in $t$. The [Leibniz formula for determinants](../../../linear-algebra.md#leibniz-formula-for-determinants) therefore makes each adjugate entry a polynomial in $t$ of degree at most $n-1$.

For arbitrary $A,B$, choose positive sequences $s_j,t_j\to0$ for which $A-s_jI$ and $B-t_jI$ are nonsingular. The nonsingular identity from part (b) applies to their product:

$$
\operatorname{adj}((A-s_jI)(B-t_jI))
=\operatorname{adj}(B-t_jI)\operatorname{adj}(A-s_jI).
$$

Every entry is a polynomial, hence continuous, in the matrix entries. Letting $j\to\infty$ proves

$$
\boxed{\operatorname{adj}(AB)
=\operatorname{adj}(B)\operatorname{adj}(A)}
$$

for all square matrices.

<h3 id="6a/d">d</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/d/solution">Solution</h4>

↑ **Parent:** [D](#6a/d)

Define

$$
P(A)=(-1)^{n-1}A^{n-1}
-c_{n-1}A^{n-2}-\cdots-c_2A-c_1I.
$$

The [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) for

$$
\chi_A(z)=(-1)^nz^n+c_{n-1}z^{n-1}
+\cdots+c_1z+c_0
$$

gives

$$
AP(A)=P(A)A=c_0I=\det(A)I.
$$

If $A$ is nonsingular, multiplication by $A^{-1}$ shows $P(A)=\det(A)A^{-1}=\operatorname{adj}(A)$.

For arbitrary $A$, apply the nonsingular result to $A-tI$ for a sequence of nonzero $t\to0$ avoiding the finitely many singular values. Both the characteristic coefficients and the adjugate entries depend polynomially on the matrix entries, so the limit gives

$$
\boxed{
\operatorname{adj}(A)
=(-1)^{n-1}A^{n-1}
-c_{n-1}A^{n-2}-\cdots-c_2A-c_1I}.
$$

## 7A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7a/solution">Solution</h3>

↑ **Parent:** [7A](#7a)

By the [real spectral theorem](../../../linear-operator-theory.md#real-spectral-theorem), a real symmetric matrix has an orthogonal diagonalization

$$
A=Q\operatorname{diag}(\lambda_1,\ldots,\lambda_n)Q^T.
$$

Writing $y=Q^Tx$ gives

$$
x^TAx=\sum_i\lambda_i y_i^2.
$$

This is nonnegative for every $x$ exactly when every $\lambda_i\geq0$. Thus the quadratic-form and eigenvalue definitions of a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix) agree.

When $A$ is positive semidefinite, define

$$
\boxed{
\sqrt A
=Q\operatorname{diag}(\sqrt{\lambda_1},\ldots,\sqrt{\lambda_n})Q^T}.
$$

This matrix is symmetric and positive semidefinite, and its square is $A$, so it is the [principal square root of a positive semidefinite matrix](../../../linear-algebra.md#principal-square-root-of-a-positive-semidefinite-matrix).

For nonsingular $M$, the matrix $M^TM$ is symmetric and

$$
x^TM^TMx=\|Mx\|^2>0
$$

for every nonzero $x$. Thus $M^TM$ is positive definite, and

$$
P=\sqrt{M^TM}
$$

exists and is nonsingular. Let $R=MP^{-1}$. Since $P$ is symmetric,

$$
R^TR=P^{-1}M^TMP^{-1}
=P^{-1}P^2P^{-1}=I.
$$

Hence $R$ is an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) and

$$
\boxed{M=RP},
$$

the [polar decomposition of an invertible real matrix](../../../linear-algebra.md#polar-decomposition-of-an-invertible-real-matrix).

In three dimensions, $P$ stretches or contracts along three mutually perpendicular eigenvector directions by its positive eigenvalues. The orthogonal map $R$ is then applied: it is a rotation when $\det M>0$, and a rotation combined with a reflection when $\det M<0$.

## 8B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8b/a">a</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/a/solution">Solution</h4>

↑ **Parent:** [A](#8b/a)

The determinant factors as

$$
\det A=-2(\mu-1)(\mu+1).
$$

Thus for $\mu\ne\pm1$, the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is $\{0\}$ and the inhomogeneous system has exactly one solution.

At $\mu=-1$, row reduction gives

$$
\ker A=\operatorname{span}\{(1,-2,3)^T\},
$$

and the augmented matrix has the same rank two as $A$, so there are infinitely many solutions. At $\mu=1$,

$$
\ker A=\operatorname{span}\{(-1,-2,3)^T\},
$$

but the augmented matrix has rank three while $A$ has rank two, so there is no solution. Therefore the number of solutions is

$$
\boxed{
\begin{cases}
1,&\mu\ne\pm1,\\
\infty,&\mu=-1,\\
0,&\mu=1.
\end{cases}}
$$

<h3 id="8b/b">b</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/b/i">i</h4>

↑ **Parent:** [B](#8b/b)

<h5 id="8b/b/i/solution">Solution</h5>

↑ **Parent:** [I](#8b/b/i)

Writing $n$ as a column vector, the reflection is

$$
\Phi(x)=x-2n(n^Tx),
$$

so its [reflection matrix](../../../linear-algebra.md#reflection-matrix) is

$$
\boxed{H=I-2nn^T},
\qquad
H_{ij}=\delta_{ij}-2n_in_j.
$$

<h4 id="8b/b/ii">ii</h4>

↑ **Parent:** [B](#8b/b)

<h5 id="8b/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8b/b/ii)

Choose the $z$-axis along the line of intersection of the two planes. Their unit normals lie in the $xy$-plane; after choosing the $x$-axis, take

$$
n=(1,0,0),
\qquad
m=(\cos\theta,\sin\theta,0),
$$

where $\theta$ is the oriented angle between the planes. The two [reflection matrices](../../../linear-algebra.md#reflection-matrix) restrict to

$$
H_n=\begin{pmatrix}-1&0\\0&1\end{pmatrix},
\qquad
H_m=\begin{pmatrix}
-\cos2\theta&-\sin2\theta\\
-\sin2\theta&\cos2\theta
\end{pmatrix}
$$

on the $xy$-plane and both fix the $z$-axis. Their product is

$$
H_mH_n=
\begin{pmatrix}
\cos2\theta&-\sin2\theta\\
\sin2\theta&\cos2\theta
\end{pmatrix}.
$$

**Thus the [composition of two plane reflections](../../../linear-algebra.md#composition-of-two-plane-reflections) is a rotation about the intersection line through angle $2\theta$.**

<h4 id="8b/b/iii">iii</h4>

↑ **Parent:** [B](#8b/b)

<h5 id="8b/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#8b/b/iii)

A plane reflection has determinant $-1$, while a [rotation matrix](../../../linear-algebra.md#rotation-matrix) has determinant $+1$. The determinant of their product, in either order, is therefore $-1$. Since every rotation has determinant $+1$, such a product can never be another rotation.

## 9F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9f/a">a</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/a/solution">Solution</h4>

↑ **Parent:** [A](#9f/a)

The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) states that if $f:[a,b]\to\mathbb R$ is continuous and $y$ lies between $f(a)$ and $f(b)$, then $f(c)=y$ for some $c\in[a,b]$.

Let $x_1<x_2<x_3$. If, for example, $f(x_2)$ exceeded both $f(x_1)$ and $f(x_3)$, choose $y$ strictly between $f(x_2)$ and $\max\{f(x_1),f(x_3)\}$. Applying the theorem on both $[x_1,x_2]$ and $[x_2,x_3]$ would give two distinct preimages of $y$, contradicting injectivity. The analogous argument excludes $f(x_2)$ below both endpoint values. Since the three values are distinct,

$$
\boxed{
f(x_1)<f(x_2)<f(x_3)
\quad\text{or}\quad
f(x_1)>f(x_2)>f(x_3)}.
$$

Fix $a<b$. If $f(a)<f(b)$, applying the displayed betweenness property to triples containing $a,b$ forces the same increasing order for every pair $x<y$; an order reversal would create a triple whose middle value is not between the other two. Thus $f$ is strictly increasing. If $f(a)>f(b)$, the same argument shows that it is strictly decreasing. This proves that every [continuous bijection of the real line is monotone](../../../calculus.md#continuous-bijection-of-the-real-line-is-monotone).

<h3 id="9f/b">b</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/b/i">i</h4>

↑ **Parent:** [B](#9f/b)

<h5 id="9f/b/i/solution">Solution</h5>

↑ **Parent:** [I](#9f/b/i)

**True.** If $x_n\to x$, continuity of $g$ gives $g(x_n)\to g(x)$, and continuity of $f$ then gives

$$
f(g(x_n))\to f(g(x)).
$$

Equivalently, this is the [composition of continuous functions](../../../calculus.md#composition-of-continuous-functions) theorem.

<h4 id="9f/b/ii">ii</h4>

↑ **Parent:** [B](#9f/b)

<h5 id="9f/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9f/b/ii)

This can be false because a strictly increasing $g$ need not be surjective. Take

$$
g(x)=e^x,
\qquad
f(y)=
\begin{cases}
0,&y>0,\\
1,&y\leq0.
\end{cases}
$$

Then $g$ is strictly increasing and $f\circ g=0$ is continuous, while $f$ is discontinuous at zero.

<h4 id="9f/b/iii">iii</h4>

↑ **Parent:** [B](#9f/b)

<h5 id="9f/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#9f/b/iii)

**True.** Part (a) shows that $f$ is strictly monotone. Suppose it is increasing and let $y_0=f(x_0)$. Given $\epsilon>0$,

$$
f(x_0-\epsilon)<y_0<f(x_0+\epsilon).
$$

Choose $\delta>0$ smaller than both distances from $y_0$ to the two outer values. If $|y-y_0|<\delta$, monotonicity forces

$$
x_0-\epsilon<f^{-1}(y)<x_0+\epsilon.
$$

**Thus $f^{-1}$ is continuous at $y_0$. The decreasing case is identical with inequalities reversed.**

<h4 id="9f/b/iv">iv</h4>

↑ **Parent:** [B](#9f/b)

<h5 id="9f/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#9f/b/iv)

This can be false. The function

$$
f(x)=x^3
$$

is a differentiable bijection of $\mathbb R$, but

$$
f^{-1}(y)=\sqrt[3]y
$$

has an unbounded difference quotient at zero and is not differentiable there. The [inverse function theorem](../../../calculus.md#inverse-function-theorem) requires the additional local condition $f'(x)\ne0$.

## 10F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10f/a">a</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/a/solution">Solution</h4>

↑ **Parent:** [A](#10f/a)

Pointwise on $[a,b]$,

$$
mg(x)\leq f(x)g(x)\leq Mg(x)
$$

because $g(x)>0$. To see the implication directly from the definition, every Riemann sum of the nonnegative continuous function $(f-m)g$ is nonnegative, so its limit is nonnegative:

$$
\int_a^b(f-m)g\geq0.
$$

Applying the same argument to $(M-f)g$ gives $\int_a^b(M-f)g\geq0$. By linearity, these are exactly the [monotonicity of the Riemann integral](../../../real-analysis.md#monotonicity-of-the-riemann-integral) bounds

$$
\boxed{
m\int_a^bg(x)\,dx
\leq\int_a^bf(x)g(x)\,dx
\leq M\int_a^bg(x)\,dx}.
$$

<h3 id="10f/b">b</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/b/solution">Solution</h4>

↑ **Parent:** [B](#10f/b)

Let

$$
m_n=\min_{0\leq x\leq n^{-1/2}}f(x),
\qquad
M_n=\max_{0\leq x\leq n^{-1/2}}f(x).
$$

Continuity at zero gives $m_n,M_n\to f(0)$. Part (a), with the positive weight $ne^{-nx}$, gives

$$
m_n(1-e^{-\sqrt n})
\leq
\int_0^{1/\sqrt n}nf(x)e^{-nx}\,dx
\leq
M_n(1-e^{-\sqrt n}).
$$

The [squeeze theorem](../../../calculus.md#squeeze-theorem) therefore yields

$$
\boxed{
\int_0^{1/\sqrt n}nf(x)e^{-nx}\,dx\to f(0)}.
$$

Since $f$ is bounded on $[0,1]$, say $|f|\leq K$, the omitted tail satisfies

$$
\left|
\int_{1/\sqrt n}^1nf(x)e^{-nx}\,dx
\right|
\leq K(e^{-\sqrt n}-e^{-n})\longrightarrow0.
$$

Adding the tail proves

$$
\boxed{\int_0^1nf(x)e^{-nx}\,dx\to f(0)}.
$$

## 11F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11f/a">a</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/a/solution">Solution</h4>

↑ **Parent:** [A](#11f/a)

The [Taylor theorem with Lagrange remainder](../../../calculus.md#taylor-theorem-with-lagrange-remainder) states that if $f$ is $n$ times differentiable between $a$ and $x$, then some $\xi$ between $a$ and $x$ satisfies

$$
f(x)=\sum_{j=0}^{n-1}
\frac{f^{(j)}(a)}{j!}(x-a)^j
+\frac{f^{(n)}(\xi)}{n!}(x-a)^n.
$$

Let $T_{n-1}$ denote the displayed polynomial and choose $K$ so that

$$
F(t)=f(t)-T_{n-1}(t)-K(t-a)^n
$$

satisfies $F(x)=0$. By construction,

$$
F(a)=F'(a)=\cdots=F^{(n-1)}(a)=0.
$$

Starting with the two zeros $a,x$ and applying [Rolle theorem](../../../calculus.md#rolle-theorem) repeatedly, there is a $\xi$ between them with $F^{(n)}(\xi)=0$. Since

$$
F^{(n)}(\xi)=f^{(n)}(\xi)-n!K,
$$

we have $K=f^{(n)}(\xi)/n!$, proving the theorem.

<h3 id="11f/b">b</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/b/solution">Solution</h4>

↑ **Parent:** [B](#11f/b)

Repeatedly differentiating $f''=-f$ and using $f(0)=1$, $f'(0)=0$ gives

$$
f^{(2k)}(0)=(-1)^k,
\qquad
f^{(2k+1)}(0)=0.
$$

Also,

$$
\frac d{dx}\bigl(f(x)^2+f'(x)^2\bigr)
=2f'f+2f'f''=0,
$$

so $f^2+(f')^2=1$. Every derivative is one of $\pm f,\pm f'$, and hence has absolute value at most one.

Taylor's theorem at zero through degree $2N+1$ gives

$$
f(x)=\sum_{k=0}^N(-1)^k\frac{x^{2k}}{(2k)!}
+R_N(x),
$$

where

$$
|R_N(x)|
\leq\frac{|x|^{2N+2}}{(2N+2)!}\longrightarrow0
$$

for each fixed $x$. Therefore

$$
\boxed{
f(x)=\sum_{k=0}^{\infty}(-1)^k\frac{x^{2k}}{(2k)!}}.
$$

## 12F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12f/a">a</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/a/i">i</h4>

↑ **Parent:** [A](#12f/a)

<h5 id="12f/a/i/solution">Solution</h5>

↑ **Parent:** [I](#12f/a/i)

Let $L=\limsup_{n\to\infty}|a_n|^{1/n}$. The [Cauchy-Hadamard theorem](../../../real-analysis.md#cauchy-hadamard-theorem), proved by applying the root test, gives a [radius of convergence](../../../real-analysis.md#radius-of-convergence)

$$
R=\frac1L
$$

with the usual conventions. For $|z|<R$, choose $q<1$ eventually bounding $|a_nz^n|^{1/n}$, which gives absolute convergence by comparison with a geometric series. For $|z|>R$, infinitely many terms have $n$th root greater than one, so the terms fail to tend to zero and the series diverges.

Here $R=2$ and the assumed limit gives $|a_n|^{1/n}\to1/2$. Therefore

$$
|a_{kn}|^{1/n}
=\left(|a_{kn}|^{1/(kn)}\right)^k
\longrightarrow2^{-k}.
$$

Thus

$$
\boxed{\sum_{n=0}^\infty a_{kn}z^n
\text{ has radius }2^k}.
$$

<h4 id="12f/a/ii">ii</h4>

↑ **Parent:** [A](#12f/a)

<h5 id="12f/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#12f/a/ii)

The series can be written as

$$
\sum_{n=0}^\infty a_n(z^k)^n.
$$

The original power series converges when $|z|^k<2$ and diverges when $|z|^k>2$. Hence its radius as a power series in $z$ is

$$
\boxed{2^{1/k}}.
$$

<h4 id="12f/a/iii">iii</h4>

↑ **Parent:** [A](#12f/a)

<h5 id="12f/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#12f/a/iii)

Apply the root test to the terms $a_nz^{n^2}$:

$$
|a_nz^{n^2}|^{1/n}
=|a_n|^{1/n}|z|^n.
$$

This tends to zero when $|z|<1$ and to infinity when $|z|>1$. On $|z|=1$, the series converges absolutely because $\sum|a_n|$ converges: the point $1$ lies strictly inside the original radius two. Thus the lacunary power series has radius

$$
\boxed{1}
$$

and in fact converges on its entire boundary circle.

<h3 id="12f/b">b</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/b/solution">Solution</h4>

↑ **Parent:** [B](#12f/b)

Set $w=e^z$. Then

$$
\sum_{n=0}^\infty b_ne^{nz}
=\sum_{n=0}^\infty b_nw^n.
$$

The hypothesis that convergence and divergence both occur implies that this ordinary power series has a radius $R$ with $0<R<\infty$. Since $|w|=e^{\operatorname{Re}z}$, the [half-plane of convergence of an exponential power series](../../../real-analysis.md#half-plane-of-convergence-of-an-exponential-power-series) is determined by

$$
\boxed{S=\log R}:
$$

the series converges for $\operatorname{Re}z<S$ and diverges for $\operatorname{Re}z>S$.

For the specified series,

$$
\frac{2^ne^{inz}}{(n+1)^2}
=\frac{(2e^{iz})^n}{(n+1)^2}.
$$

Writing $z=x+iy$ gives $|2e^{iz}|=2e^{-y}$. The series converges absolutely when $y>\log2$ and diverges by the term test when $y<\log2$. On $y=\log2$, its absolute values are $(n+1)^{-2}$, so it still converges absolutely. Therefore the exact convergence set is

$$
\boxed{\{z\in\mathbb C:\operatorname{Im}z\geq\log2\}}.
$$

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
