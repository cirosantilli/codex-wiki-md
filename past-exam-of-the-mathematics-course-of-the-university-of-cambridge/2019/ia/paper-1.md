# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2019/paperia_1_2019.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2019/paperia_1_2019.pdf)

**Table of contents**

- [1C](#1c)
  - [a](#1c/a)
    - [Solution](#1c/a/solution)
  - [b](#1c/b)
    - [Solution](#1c/b/solution)
  - [c](#1c/c)
    - [Solution](#1c/c/solution)
  - [d](#1c/d)
    - [Solution](#1c/d/solution)
- [2A](#2a)
  - [i](#2a/i)
    - [Solution](#2a/i/solution)
  - [ii](#2a/ii)
    - [Solution](#2a/ii/solution)
  - [iii](#2a/iii)
    - [Solution](#2a/iii/solution)
  - [iv](#2a/iv)
    - [Solution](#2a/iv/solution)
- [3E](#3e)
  - [i](#3e/i)
    - [Solution](#3e/i/solution)
  - [ii](#3e/ii)
    - [Solution](#3e/ii/solution)
  - [iii](#3e/iii)
    - [Solution](#3e/iii/solution)
- [4F](#4f)
  - [i](#4f/i)
    - [Solution](#4f/i/solution)
  - [ii](#4f/ii)
    - [Solution](#4f/ii/solution)
- [5C](#5c)
  - [a](#5c/a)
    - [i](#5c/a/i)
      - [Solution](#5c/a/i/solution)
    - [ii](#5c/a/ii)
      - [Solution](#5c/a/ii/solution)
  - [b](#5c/b)
    - [Solution](#5c/b/solution)
  - [c](#5c/c)
    - [Solution](#5c/c/solution)
- [6B](#6b)
  - [Solution](#6b/solution)
- [7B](#7b)
  - [a](#7b/a)
    - [Solution](#7b/a/solution)
  - [b](#7b/b)
    - [Solution](#7b/b/solution)
  - [c](#7b/c)
    - [Solution](#7b/c/solution)
- [8A](#8a)
  - [a](#8a/a)
    - [Solution](#8a/a/solution)
  - [b](#8a/b)
    - [Solution](#8a/b/solution)
  - [c](#8a/c)
    - [i](#8a/c/i)
      - [Solution](#8a/c/i/solution)
    - [ii](#8a/c/ii)
      - [Solution](#8a/c/ii/solution)
  - [d](#8a/d)
    - [i](#8a/d/i)
      - [Solution](#8a/d/i/solution)
    - [ii](#8a/d/ii)
      - [Solution](#8a/d/ii/solution)
- [9D](#9d)
  - [Solution](#9d/solution)
- [10D](#10d)
  - [Solution](#10d/solution)
- [11E](#11e)
  - [a](#11e/a)
    - [Solution](#11e/a/solution)
  - [b](#11e/b)
    - [Solution](#11e/b/solution)
  - [c](#11e/c)
    - [Solution](#11e/c/solution)
- [12F](#12f)
  - [i](#12f/i)
    - [Solution](#12f/i/solution)
  - [ii](#12f/ii)
    - [Solution](#12f/ii/solution)
  - [iii](#12f/iii)
    - [Solution](#12f/iii/solution)

## 1C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1c/a">a</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/a/solution">Solution</h4>

↑ **Parent:** [A](#1c/a)

The powers of the [imaginary unit](../../../complex-analysis.md#imaginary-unit) have period four. Hence

$$
\sum_{a=0}^{200}i^a
=50(1+i-1-i)+i^{200}=1,
$$

while

$$
\prod_{b=1}^{50}i^b=i^{1+2+\cdots+50}=i^{1275}=i^3=-i.
$$

Thus $x+iy=1-i$, so

$$
\boxed{xy=-1}.
$$

<h3 id="1c/b">b</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/b/solution">Solution</h4>

↑ **Parent:** [B](#1c/b)

Since $(1+i)/(1-i)=i$ and $(1+i)^2=2i$,

$$
\frac{(1+i)^{2019}}{(1-i)^{2017}}
=i^{2017}(1+i)^2
=i(2i)=\boxed{-2}.
$$

<h3 id="1c/c">c</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/c/solution">Solution</h4>

↑ **Parent:** [C](#1c/c)

Use the [principal complex logarithm](../../../analysis.md#principal-complex-logarithm), for which $\operatorname{Log}i=i\pi/2$, and set

$$
a=\frac{2\log2}{\pi},
\qquad
\boxed{z=-1-\frac{2i}{\pi}\log a}.
$$

Then the definition of [complex exponentiation](../../../analysis.md#complex-exponentiation) gives

$$
i^z=e^{z\operatorname{Log}i}
=e^{\log a-i\pi/2}=-ia,
$$

and therefore

$$
i^{,i^z}=e^{(-ia)i\pi/2}=e^{a\pi/2}=e^{\log2}=2.
$$

Other choices of [branch of the complex logarithm](../../../analysis.md#branch-of-the-complex-logarithm) produce further valid answers.

<h3 id="1c/d">d</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/d/solution">Solution</h4>

↑ **Parent:** [D](#1c/d)

Write $z=re^{i\theta}$ with $r>0$. On a fixed [branch of the complex logarithm](../../../analysis.md#branch-of-the-complex-logarithm) on which $\log z=\log r+i\theta$ and $\log\bar z=\log r-i\theta$, the equation becomes

$$
\log r+i\theta=i(\log r-i\theta)=\theta+i\log r.
$$

Its real and imaginary parts give the same condition $\log r=\theta$, or

$$
\boxed{r=e^\theta}.
$$

This is a [logarithmic spiral](../../../topology.md#logarithmic-spiral). For the [principal complex logarithm](../../../analysis.md#principal-complex-logarithm), it is the portion parametrized by $-\pi<\theta<\pi$ that avoids the branch cut.

## 2A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2a/i">i</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/i/solution">Solution</h4>

↑ **Parent:** [I](#2a/i)

The [Leibniz formula for determinants](../../../linear-algebra.md#leibniz-formula-for-determinants) is

$$
\boxed{\det A=\sum_{\sigma\in S_n}\operatorname{sgn}(\sigma)
\prod_{r=1}^n A_{r,\sigma(r)}}.
$$

Equivalently, the [determinant](../../../linear-algebra.md#determinant) is the unique alternating function of the rows that is [multilinear](../../../linear-algebra.md#multilinearity-of-the-determinant) and takes value one on the [identity matrix](../../../vector-space.md#identity-matrix). Multiplying one row by $\lambda$ therefore gives

$$
\boxed{\det B=\lambda\det A}.
$$

<h3 id="2a/ii">ii</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2a/ii)

The scalar multiplication $\lambda A$ multiplies every one of the $n$ rows by $\lambda$. Applying [multilinearity of the determinant](../../../linear-algebra.md#multilinearity-of-the-determinant) once to each row gives

$$
\boxed{\det(\lambda A)=\lambda^n\det A}.
$$

<h3 id="2a/iii">iii</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2a/iii)

Interchanging two rows reverses the sign of an [alternating multilinear map](../../../linear-algebra.md#alternating-multilinear-map), so

$$
\boxed{\det C=-\det A}.
$$

In the [Leibniz formula for determinants](../../../linear-algebra.md#leibniz-formula-for-determinants), the same result follows by composing every [permutation](../../../combinatorics.md#permutation) with the corresponding [transposition](../../../combinatorics.md#transposition-permutation), which reverses its [sign](../../../finite-group-theory.md#sign-of-a-permutation).

<h3 id="2a/iv">iv</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2a/iv)

Let the columns be $C_1,\ldots,C_n$, and replace $C_k$ by $C_k+\lambda C_l$, where $k\ne l$. By [multilinearity of the determinant](../../../linear-algebra.md#multilinearity-of-the-determinant),

$$
\det(C_1,\ldots,C_k+\lambda C_l,\ldots,C_n)
=\det A+\lambda\det(C_1,\ldots,C_l,\ldots,C_l,\ldots,C_n).
$$

The second determinant vanishes because it has two equal columns. Hence

$$
\boxed{\det D=\det A}.
$$

## 3E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3e/i">i</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/i/solution">Solution</h4>

↑ **Parent:** [I](#3e/i)

The [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) states that every [bounded sequence](../../../real-analysis.md#bounded-sequence) of real numbers has a [convergent subsequence](../../../real-analysis.md#convergent-subsequence).

Condition (i) is insufficient because the allowed limit may be zero. For example, $a_n=1/n$ is nonzero and converges to zero, whereas $1/a_n=n$ does not converge in $\mathbb R$.

<h3 id="3e/ii">ii</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3e/ii)

Condition (ii) is sufficient. If $a_n\to\ell\ne0$, then eventually $|a_n|\geq|\ell|/2$. Therefore

$$
\left|\frac1{a_n}-\frac1\ell\right|
=\frac{|a_n-\ell|}{|a_n\ell|}
\leq\frac{2}{|\ell|^2}|a_n-\ell|\longrightarrow0,
$$

so

$$
\boxed{\frac1{a_n}\longrightarrow\frac1\ell}.
$$

<h3 id="3e/iii">iii</h3>

↑ **Parent:** [3E](#3e)

<h4 id="3e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3e/iii)

Condition (iii) is also sufficient. If $|a_n|$ did not tend to infinity, some $M>0$ would contain infinitely many terms with $|a_n|\leq M$. Those terms form a [bounded subsequence](../../../real-analysis.md#bounded-subsequence), and the [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) would give it a convergent subsequence, contrary to the hypothesis. Hence $|a_n|\to\infty$ and

$$
\boxed{\frac1{a_n}\longrightarrow0}.
$$

## 4F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4f/i">i</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/i/solution">Solution</h4>

↑ **Parent:** [I](#4f/i)

Let

$$
S=\left\{r\geq0:\sum_{n=1}^\infty |a_n|r^n<\infty\right\}.
$$

The set $S$ contains zero. If $r\in S$ and $0\leq s<r$, then $s\in S$ by comparison. Moreover, if the original [power series](../../../real-analysis.md#power-series) diverges at $x_0$, no $r>|x_0|$ can lie in $S$, because absolute convergence at $r$ would imply absolute convergence at $x_0$. Thus $R=\sup S$ is finite and nonnegative.

If $|x|<R$, choose $r\in S$ with $|x|<r$; comparison gives absolute convergence at $x$. If $|x|>R$ and the series converged at $x$, then its terms $a_nx^n$ would be bounded. For any $y$ with $R<|y|<|x|$,

$$
|a_ny^n|\leq M\left|\frac yx\right|^n,
$$

so the [geometric series](../../../real-analysis.md#geometric-series) comparison would put $|y|$ in $S$, contradicting the definition of $R$. This proves the [radius of convergence](../../../real-analysis.md#radius-of-convergence) property.

For $\sum_{n\geq1}x^n/3^n$, the ratio is $x/3$, so the [geometric series](../../../real-analysis.md#geometric-series) criterion gives

$$
\boxed{R=3}.
$$

<h3 id="4f/ii">ii</h3>

↑ **Parent:** [4F](#4f)

<h4 id="4f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4f/ii)

The inequality $(1+1/n)^n\leq e$ gives, for $|x|<1$,

$$
\sum_{n=1}^\infty |x|^n\left(1+\frac1n\right)^n
\leq e\sum_{n=1}^\infty|x|^n<\infty.
$$

For $|x|>1$, the terms have magnitude at least $|x|^n$ and therefore do not tend to zero, so the series diverges by the [term test for divergence](../../../real-analysis.md#term-test-for-divergence). Hence

$$
\boxed{R=1}.
$$

## 5C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5c/a">a</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/a/i">i</h4>

↑ **Parent:** [A](#5c/a)

<h5 id="5c/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5c/a/i)

Using the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) and the [epsilon-delta identity](../../../calculus.md#contraction-of-two-levi-civita-symbols),

$$
[\mathbf a\times(\mathbf b\times\mathbf c)]_i
=\varepsilon_{ijk}a_j\varepsilon_{klm}b_lc_m
=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})a_jb_lc_m
=b_i(\mathbf a\cdot\mathbf c)-c_i(\mathbf a\cdot\mathbf b).
$$

This proves the [vector triple product identity](../../../calculus.md#vector-triple-product)

$$
\boxed{\mathbf a\times(\mathbf b\times\mathbf c)
=(\mathbf a\cdot\mathbf c)\mathbf b-(\mathbf a\cdot\mathbf b)\mathbf c}.
$$

Applying it inside the [scalar triple product](../../../linear-algebra.md#scalar-triple-product) gives [Lagrange's identity](../../../calculus.md#lagrange-identity-for-the-cross-product)

$$
\boxed{(\mathbf a\times\mathbf b)\cdot(\mathbf c\times\mathbf d)
=(\mathbf a\cdot\mathbf c)(\mathbf b\cdot\mathbf d)
-(\mathbf a\cdot\mathbf d)(\mathbf b\cdot\mathbf c)}.
$$

<h4 id="5c/a/ii">ii</h4>

↑ **Parent:** [A](#5c/a)

<h5 id="5c/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5c/a/ii)

The [vector triple product identity](../../../calculus.md#vector-triple-product) gives

$$
(\mathbf b\times\mathbf c)\times(\mathbf c\times\mathbf a)
=\mathbf c[(\mathbf b\times\mathbf c)\cdot\mathbf a]
-\mathbf a[(\mathbf b\times\mathbf c)\cdot\mathbf c]
=\mathbf c[\mathbf a\cdot(\mathbf b\times\mathbf c)].
$$

Taking the dot product with $\mathbf a\times\mathbf b$ therefore yields

$$
\boxed{(\mathbf a\times\mathbf b)\cdot[(\mathbf b\times\mathbf c)\times(\mathbf c\times\mathbf a)]
=[\mathbf a\cdot(\mathbf b\times\mathbf c)]^2}.
$$

<h3 id="5c/b">b</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/b/solution">Solution</h4>

↑ **Parent:** [B](#5c/b)

Write

$$
\mathbf x=\mathbf a+\mathbf u,
\qquad
\mathbf y=\mathbf a-\mathbf u.
$$

The first equation is then automatic, while the second becomes

$$
\mathbf x\cdot\mathbf y
=\mathbf a\cdot\mathbf a-\mathbf u\cdot\mathbf u=c.
$$

Thus the general solution is

$$
\boxed{\mathbf x=\mathbf a+\mathbf u,
\qquad \mathbf y=\mathbf a-\mathbf u,
\qquad |\mathbf u|=\sqrt{\mathbf a\cdot\mathbf a-c}}.
$$

As $\mathbf u$ varies, $\mathbf x$ and $\mathbf y$ are antipodal points of the [sphere](../../../geometry-and-topology.md#sphere) with center $\mathbf a$ and radius $\sqrt{\mathbf a\cdot\mathbf a-c}$, so they are opposite ends of a diameter.

<h3 id="5c/c">c</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/c/solution">Solution</h4>

↑ **Parent:** [C](#5c/c)

Let the vertex position vectors be $\mathbf a,\mathbf b,\mathbf c,\mathbf d$. Suppose

$$
(\mathbf b-\mathbf a)\cdot(\mathbf d-\mathbf c)=0,
\qquad
(\mathbf c-\mathbf a)\cdot(\mathbf d-\mathbf b)=0.
$$

Subtracting the second scalar product from the first gives

$$
-(\mathbf d-\mathbf a)\cdot(\mathbf c-\mathbf b)=0,
$$

so the remaining pair of [opposite edges of a tetrahedron](../../../geometry-and-topology.md#opposite-edges-of-a-tetrahedron) is also perpendicular.

Put

$$
S_1=|\mathbf b-\mathbf a|^2+|\mathbf d-\mathbf c|^2,
\quad
S_2=|\mathbf c-\mathbf a|^2+|\mathbf d-\mathbf b|^2,
\quad
S_3=|\mathbf d-\mathbf a|^2+|\mathbf c-\mathbf b|^2.
$$

Direct expansion gives, cyclically,

$$
S_1-S_2=-2(\mathbf d-\mathbf a)\cdot(\mathbf c-\mathbf b),
$$

with the other two differences equal to minus twice the scalar products of the other opposite-edge pairs. All three scalar products vanish, hence

$$
\boxed{S_1=S_2=S_3}.
$$

## 6B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6b/solution">Solution</h3>

↑ **Parent:** [6B](#6b)

The columns of $P$ are the coordinates of the vectors $\mathbf f_j$, so they form a basis exactly when

$$
\boxed{\det P\ne0}.
$$

For a [linear transformation](../../../vector-space.md#linear-map) $\alpha$, define its [matrix representation](../../../representation-theory.md#matrix-representation) in the standard basis by

$$
[\alpha(\mathbf v)]_{\mathbf e}=A[\mathbf v]_{\mathbf e},
\qquad A_{ij}=[\alpha(\mathbf e_j)]_i.
$$

The [change-of-basis matrix](../../../linear-algebra.md#change-of-basis-matrix) satisfies $[\mathbf v]_{\mathbf e}=P[\mathbf v]_{\mathbf f}$. Therefore

$$
P[\alpha(\mathbf v)]_{\mathbf f}
=A P[\mathbf v]_{\mathbf f},
$$

and multiplication by $P^{-1}$ gives the [similar matrix](../../../linear-algebra.md#matrix-similarity) relation

$$
\boxed{\widetilde A=P^{-1}AP}.
$$

The characteristic polynomial of the displayed $A$ is

$$
(\lambda-1)(\lambda-2)^2.
$$

Eigenvectors $(2,-1,2)^T$, $(1,0,0)^T$, and $(0,-1,3)^T$ give

$$
P=\begin{pmatrix}2&1&0\\-1&0&-1\\2&0&3\end{pmatrix},
\qquad
B=\begin{pmatrix}1&0&0\\0&2&0\\0&0&2\end{pmatrix}.
$$

Indeed, $\det P=1$ and

$$
AP=\begin{pmatrix}2&2&0\\-1&0&-2\\2&0&6\end{pmatrix}=PB,
$$

so $P^{-1}AP=B$. Finally, the [diagonalization of a matrix](../../../linear-operator-theory.md#diagonalization-of-a-matrix) gives

$$
A^nP=PB^n
=\boxed{\begin{pmatrix}
2&2^n&0\\
-1&0&-2^n\\
2&0&3\,2^n
\end{pmatrix}}.
$$

## 7B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7b/a">a</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/a/solution">Solution</h4>

↑ **Parent:** [A](#7b/a)

Choose

$$
\boxed{\chi_A(z)=\det(A-zI)}.
$$

The [Leibniz formula for determinants](../../../linear-algebra.md#leibniz-formula-for-determinants) shows that its leading term is $(-z)^n$, as required. A scalar $\lambda$ is an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) exactly when $A-\lambda I$ has a nonzero kernel, equivalently when it is singular, so

$$
\boxed{\lambda\text{ is an eigenvalue of }A\iff\chi_A(\lambda)=0}.
$$

The [fundamental theorem of algebra](../../../algebra.md#fundamental-theorem-of-algebra) gives a complex root of the degree-$n$ polynomial $\chi_A$, so every nonempty complex square matrix has at least one complex eigenvalue.

<h3 id="7b/b">b</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/b/solution">Solution</h4>

↑ **Parent:** [B](#7b/b)

Eigenvectors belonging to distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are [linearly independent](../../../vector-space.md#linear-independence). Under the hypothesis they therefore form a basis $v_1,\ldots,v_n$. For every $j$,

$$
\chi_A(A)v_j=\chi_A(\lambda_j)v_j=0
$$

because $\chi_A(\lambda_j)=0$. A linear map that vanishes on a basis is zero, hence

$$
\boxed{\chi_A(A)=0}.
$$

This proves the [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) in the distinct-eigenvalue case.

<h3 id="7b/c">c</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/c/solution">Solution</h4>

↑ **Parent:** [C](#7b/c)

Over $\mathbb C$, triangularize $B$ and denote its eigenvalues, with algebraic multiplicity, by $\beta_1,\ldots,\beta_n$. Then

$$
\chi_{B^m}(z^m)=\prod_{j=1}^n(\beta_j^m-z^m).
$$

The numbers $\omega_l=e^{2\pi il/m}$ are all the [root of unity](../../../algebra.md#root-of-unity) solutions of $w^m=1$, so

$$
\prod_{l=1}^m(t-\omega_lz)=t^m-z^m.
$$

Consequently

$$
\begin{aligned}
\prod_{l=1}^m\chi_B(\omega_lz)
&=\prod_{j=1}^n\prod_{l=1}^m(\beta_j-\omega_lz)\\
&=\prod_{j=1}^n(\beta_j^m-z^m)
=\boxed{\chi_{B^m}(z^m)}.
\end{aligned}
$$

If $\lambda$ is an eigenvalue of $B^m$, choose $z$ with $z^m=\lambda$. The displayed identity makes at least one factor $\chi_B(\omega_lz)$ zero. Thus $\mu=\omega_lz$ is an eigenvalue of $B$ and

$$
\boxed{\mu^m=\lambda}.
$$

## 8A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8a/a">a</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/a/solution">Solution</h4>

↑ **Parent:** [A](#8a/a)

Let

$$
J_-=\begin{pmatrix}0&-1\\1&0\end{pmatrix},
\qquad
J_+=\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

Since $J_-^2=-I$ and $J_+^2=I$, separating the even and odd terms of the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) gives

$$
\boxed{R=e^{\theta J_-}
=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}},
$$

and

$$
\boxed{S=e^{\theta J_+}
=\begin{pmatrix}\cosh\theta&\sinh\theta\\\sinh\theta&\cosh\theta\end{pmatrix}}.
$$

<h3 id="8a/b">b</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/b/solution">Solution</h4>

↑ **Parent:** [B](#8a/b)

Direct multiplication and the identities $\cos^2\theta+\sin^2\theta=1$ and $\cosh^2\theta-\sinh^2\theta=1$ give

$$
\boxed{RR^T=I},
\qquad
\boxed{SJS=J},
\qquad
J=\begin{pmatrix}1&0\\0&-1\end{pmatrix}.
$$

**Thus $R$ is an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix), while $S$ preserves the indefinite [quadratic form](../../../linear-algebra.md#quadratic-form) $x_1^2-x_2^2$.**

<h3 id="8a/c">c</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/c/i">i</h4>

↑ **Parent:** [C](#8a/c)

<h5 id="8a/c/i/solution">Solution</h5>

↑ **Parent:** [I](#8a/c/i)

The matrix $A$ fixes the first coordinate and restricts to one half of the rotation generator on the last two coordinates. Hence

$$
\boxed{e^{xA}=\begin{pmatrix}
1&0&0\\
0&\cos(x/2)&-\sin(x/2)\\
0&\sin(x/2)&\cos(x/2)
\end{pmatrix}}.
$$

<h4 id="8a/c/ii">ii</h4>

↑ **Parent:** [C](#8a/c)

<h5 id="8a/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8a/c/ii)

The matrix $B$ fixes the second coordinate and satisfies the hyperbolic-generator relation on the first and third coordinates. Therefore

$$
\boxed{e^{xB}=\begin{pmatrix}
\cosh x&0&\sinh x\\
0&1&0\\
\sinh x&0&\cosh x
\end{pmatrix}}.
$$

<h3 id="8a/d">d</h3>

↑ **Parent:** [8A](#8a)

<h4 id="8a/d/i">i</h4>

↑ **Parent:** [D](#8a/d)

<h5 id="8a/d/i/solution">Solution</h5>

↑ **Parent:** [I](#8a/d/i)

The [rotation matrix](../../../linear-algebra.md#rotation-matrix) $e^{xA}$ commutes with $C$ and is [orthogonal](../../../linear-algebra.md#orthogonal-matrix), so

$$
e^{xA}C(e^{xA})^T=C.
$$

Since $C^n=\operatorname{diag}(1,(-1)^n,(-1)^n)$,

$$
\boxed{\sum_{n=1}^N\left(e^{xA}C(e^{xA})^T\right)^n
=\operatorname{diag}\left(N,\frac{(-1)^N-1}{2},\frac{(-1)^N-1}{2}\right)}.
$$

<h4 id="8a/d/ii">ii</h4>

↑ **Parent:** [D](#8a/d)

<h5 id="8a/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8a/d/ii)

On the first and third coordinates, the identity $SJS=J$ from part (b) gives $e^{xB}Ce^{xB}=C$; the second coordinate is also unchanged. Thus

$$
\boxed{\sum_{n=1}^N\left(e^{xB}Ce^{xB}\right)^n
=\operatorname{diag}\left(N,\frac{(-1)^N-1}{2},\frac{(-1)^N-1}{2}\right)}.
$$

## 9D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9d/solution">Solution</h3>

↑ **Parent:** [9D](#9d)

The [Cauchy functional equation](../../../analysis.md#cauchy-s-functional-equation) first gives $g(0)=0$ and $g(-x)=-g(x)$. If $h\to0$, then continuity at the given point $z$ gives

$$
g(h)=g(z+h)-g(z)\longrightarrow0,
$$

so $g$ is continuous at zero. For every $x$,

$$
g(x+h)-g(x)=g(h)\longrightarrow0,
$$

so $g$ is continuous everywhere.

Put $c=g(1)$. Additivity gives $g(n)=nc$ for integers $n$ and then $g(m/n)=(m/n)c$ for [rational numbers](../../../number-theory.md#rational-number). For any real $x$, choose rationals $q_j\to x$; continuity gives

$$
\boxed{g(x)=\lim_jg(q_j)=\lim_jcq_j=cx}.
$$

For the multiplicative equation, $h(0)=h(0)^2$. If $h(0)=0$, then $h(x)=h(x)h(0)=0$ for every $x$. Otherwise $h(0)=1$. In that case

$$
h(x)=h(x/2)^2\geq0,
$$

and $h(x)$ cannot vanish because $1=h(0)=h(x)h(-x)$. Hence $h$ is everywhere positive. The continuous function $g=\log h$ satisfies the [Cauchy functional equation](../../../analysis.md#cauchy-s-functional-equation), so $g(x)=cx$. Therefore the complete family is

$$
\boxed{h\equiv0\quad\text{or}\quad h(x)=e^{cx}\ \text{for some }c\in\mathbb R}.
$$

## 10D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10d/solution">Solution</h3>

↑ **Parent:** [10D](#10d)

The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) states that if $f:[a,b]\to\mathbb R$ is [continuous](../../../calculus.md#continuous-function) and $y$ lies between $f(a)$ and $f(b)$, then some $c\in[a,b]$ satisfies $f(c)=y$.

Assume $f(a)<y<f(b)$ and let

$$
S=\{x\in[a,b]:f(x)\leq y\},
\qquad c=\sup S.
$$

The [least-upper-bound property](../../../real-analysis.md#least-upper-bound-property) makes $c$ well defined. If $f(c)<y$, continuity gives points immediately to the right of $c$ in $S$, contradicting that $c$ is an upper bound. If $f(c)>y$, continuity gives a left neighborhood of $c$ disjoint from $S$, contradicting the definition of the [supremum](../../../real-analysis.md#supremum). Thus $f(c)=y$. The endpoint and reversed-order cases follow directly or by replacing $f$ with $-f$.

The [mean value theorem](../../../calculus.md#mean-value-theorem) states that if $g$ is continuous on $[\alpha,\beta]$ and differentiable on $(\alpha,\beta)$, then some $c\in(\alpha,\beta)$ satisfies

$$
g'(c)=\frac{g(\beta)-g(\alpha)}{\beta-\alpha}.
$$

For the functions in the question, the definition of the [derivative](../../../calculus.md#derivative) makes $h$ continuous at $a$ and $f$ continuous at $b$, with

$$
h(a)=g'(a)<k,
\qquad
h(b)=\frac{g(b)-g(a)}{b-a}=f(a),
\qquad
f(b)=g'(b)>k.
$$

If the middle secant slope equals $k$, take $[\alpha,\beta]=[a,b]$. If it exceeds $k$, the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) applied to $h$ gives $\beta\in(a,b)$ with $h(\beta)=k$, and we take $\alpha=a$. If it is below $k$, apply the theorem to $f$ to obtain $\alpha\in(a,b)$ with $f(\alpha)=k$, and take $\beta=b$. In every case

$$
\frac{g(\beta)-g(\alpha)}{\beta-\alpha}=k.
$$

The [mean value theorem](../../../calculus.md#mean-value-theorem) on this subinterval then produces $c\in(\alpha,\beta)\subset(a,b)$ with

$$
\boxed{g'(c)=k}.
$$

This is the [Darboux theorem for derivatives](../../../calculus.md#darboux-s-theorem-analysis) for the stated pair of derivative values.

## 11E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11e/a">a</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/a/solution">Solution</h4>

↑ **Parent:** [A](#11e/a)

For positive $a_n,b_n$,

$$
\sqrt{a_n^2+b_n^2}\leq a_n+b_n.
$$

The [comparison test for series](../../../real-analysis.md#comparison-test-for-series) therefore gives

$$
\boxed{\sum_n\sqrt{a_n^2+b_n^2}
\leq\sum_na_n+\sum_nb_n<\infty.}
$$

<h3 id="11e/b">b</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/b/solution">Solution</h4>

↑ **Parent:** [B](#11e/b)

The [arithmetic-geometric mean inequality](../../../mathematical-optimization.md#arithmetic-geometric-mean-inequality) gives

$$
\sqrt{a_na_{n+1}}\leq\frac{a_n+a_{n+1}}2.
$$

Thus convergence of $\sum_na_n$ implies convergence of $\sum_n\sqrt{a_na_{n+1}}$ by the [comparison test for series](../../../real-analysis.md#comparison-test-for-series).

The converse is false. Define

$$
a_{2n}=\frac1n,
\qquad
a_{2n-1}=\frac1{n^3}.
$$

The even terms make $\sum_na_n$ diverge, while

$$
\sqrt{a_{2n-1}a_{2n}}=\frac1{n^2},
\qquad
\sqrt{a_{2n}a_{2n+1}}=\frac1{\sqrt{n(n+1)^3}}\leq\frac1{n^2},
$$

so the neighboring geometric-mean series converges.

<h3 id="11e/c">c</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/c/solution">Solution</h4>

↑ **Parent:** [C](#11e/c)

Suppose $\sum_na_n$ diverges. Positivity implies $s_n\to\infty$. Put $t_n=a_n/s_n\in(0,1)$ for $n\geq2$. Since $s_{n-1}=s_n-a_n$,

$$
\frac{s_n}{s_{n-1}}=\frac1{1-t_n}.
$$

If $\sum_nt_n$ converged, then eventually $t_n\leq1/2$ and

$$
\log\frac{s_n}{s_{n-1}}=-\log(1-t_n)\leq2t_n.
$$

Summing would bound the telescoping quantity $\log(s_n/s_1)$, contradicting $s_n\to\infty$. Therefore

$$
\boxed{\sum_{n=1}^\infty\frac{a_n}{s_n}=\infty}.
$$

The converse is true. If $\sum_na_n<\infty$, then $s_n\geq s_1>0$ and

$$
\sum_n\frac{a_n}{s_n}\leq\frac1{s_1}\sum_na_n<\infty.
$$

Taking the contrapositive shows that divergence of the ratio series forces divergence of $\sum_na_n$.

## 12F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12f/i">i</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/i/solution">Solution</h4>

↑ **Parent:** [I](#12f/i)

For a [partition of an interval](../../../real-analysis.md#partition-of-an-interval) $P:0=x_0<\cdots<x_m=1$, put

$$
M_j=\sup_{x\in[x_{j-1},x_j]}f(x),
\qquad
m_j=\inf_{x\in[x_{j-1},x_j]}f(x).
$$

The [upper Darboux sum](../../../real-analysis.md#upper-darboux-sum) and [lower Darboux sum](../../../real-analysis.md#lower-darboux-sum) are

$$
U(f,P)=\sum_{j=1}^mM_j(x_j-x_{j-1}),
\qquad
L(f,P)=\sum_{j=1}^mm_j(x_j-x_{j-1}).
$$

The upper and lower integrals are

$$
\overline{\int_0^1}f=\inf_PU(f,P),
\qquad
\underline{\int_0^1}f=\sup_PL(f,P).
$$

The bounded function is [Riemann integrable](../../../real-analysis.md#riemann-integrable-function) when these values agree, and their common value is its [Riemann integral](../../../real-analysis.md#riemann-integral).

For the indicator of the rational numbers, every nondegenerate interval contains both a [rational number](../../../number-theory.md#rational-number) and an [irrational number](../../../algebra.md#irrational-number). Hence every upper sum is one and every lower sum is zero. The function is not Riemann integrable.

<h3 id="12f/ii">ii</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#12f/ii)

Let $C_n$ be the union of the $2^n$ closed intervals remaining after $n$ steps of the [Cantor set](../../../geometry-and-topology.md#cantor-set) construction. Their total length is $(2/3)^n$. Any point outside $C_n$ has a ternary expansion with a $1$ among its first $n$ digits, so $A^c\subseteq C_n$. Endpoints of deleted intervals also belong to $A$ because they have an alternative ternary expansion containing a $1$, as in $2/3=0.1222\ldots{}_3$.

A partition using all endpoints of $C_n$ has lower Darboux sum at least

$$
1-\left(\frac23\right)^n.
$$

Since $A$ is dense, every upper Darboux sum is one. Letting $n\to\infty$ gives equal upper and lower integrals, and therefore

$$
\boxed{f\text{ is Riemann integrable and }\int_0^1f(x)\,dx=1}.
$$

<h3 id="12f/iii">iii</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#12f/iii)

Both $B$ and its complement are dense. Indeed, inside any sufficiently small ternary cylinder, extend its finite digit prefix by a tail containing infinitely many $1$s to obtain a point of $B$, or by a tail of all zeros to obtain a point outside $B$. Therefore every nondegenerate interval has supremum one and infimum zero for the indicator function. Its upper integral is one and its lower integral is zero, so

$$
\boxed{f\text{ is not Riemann integrable}}.
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
