# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2008/PaperIA_1.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2008/PaperIA_1.pdf)

**Table of contents**

- [1B](#1b)
  - [Solution](#1b/solution)
- [2A](#2a)
  - [Solution](#2a/solution)
  - [i](#2a/i)
    - [Solution](#2a/i/solution)
  - [ii](#2a/ii)
    - [Solution](#2a/ii/solution)
- [3F](#3f)
  - [Solution](#3f/solution)
- [4E](#4e)
  - [Solution](#4e/solution)
- [5B](#5b)
  - [a](#5b/a)
    - [Solution](#5b/a/solution)
    - [i](#5b/a/i)
      - [Solution](#5b/a/i/solution)
    - [ii](#5b/a/ii)
      - [Solution](#5b/a/ii/solution)
  - [b](#5b/b)
    - [Solution](#5b/b/solution)
- [6A](#6a)
  - [Solution](#6a/solution)
- [7C](#7c)
  - [Solution](#7c/solution)
- [8C](#8c)
  - [Solution](#8c/solution)
- [9F](#9f)
  - [i](#9f/i)
    - [Solution](#9f/i/solution)
  - [ii](#9f/ii)
    - [Solution](#9f/ii/solution)
- [10D](#10d)
  - [a](#10d/a)
    - [Solution](#10d/a/solution)
  - [b](#10d/b)
    - [Solution](#10d/b/solution)
  - [c](#10d/c)
    - [i](#10d/c/i)
      - [Solution](#10d/c/i/solution)
    - [ii](#10d/c/ii)
      - [Solution](#10d/c/ii/solution)
    - [iii](#10d/c/iii)
      - [Solution](#10d/c/iii/solution)
- [11D](#11d)
  - [a](#11d/a)
    - [Solution](#11d/a/solution)
  - [b](#11d/b)
    - [Solution](#11d/b/solution)
  - [c](#11d/c)
    - [Solution](#11d/c/solution)
    - [i](#11d/c/i)
      - [Solution](#11d/c/i/solution)
    - [ii](#11d/c/ii)
      - [Solution](#11d/c/ii/solution)
- [12E](#12e)
  - [Solution](#12e/solution)
  - [i](#12e/i)
    - [Solution](#12e/i/solution)
  - [ii](#12e/ii)
    - [Solution](#12e/ii/solution)

## 1B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1b/solution">Solution</h3>

↑ **Parent:** [1B](#1b)

[De Moivre's theorem](../../../analysis.md#de-moivre-s-theorem) says that, for a real angle $\theta$ and an integer $m$,

$$
(\cos\theta+i\sin\theta)^m=\cos(m\theta)+i\sin(m\theta).
$$

For a [complex number](../../../complex-analysis.md#complex-number) $z=\rho(\cos\theta+i\sin\theta)$, the corresponding formula is $z^m=\rho^m[\cos(m\theta)+i\sin(m\theta)]$, with $z\ne0$ required for negative powers.

Put $q=e^{i\theta}$. If $\theta\notin2\pi\mathbb Z$, the [finite geometric series](../../../real-analysis.md#finite-geometric-series) gives

$$
S=\sum_{r=1}^nq^r=\frac{q-q^{n+1}}{1-q}.
$$

To extract the real part, multiply numerator and denominator by $1-q^{-1}$. The denominator becomes $2(1-\cos\theta)$, and the numerator is $q-1-q^{n+1}+q^n$. Thus this [finite trigonometric sum](../../../real-analysis.md#finite-trigonometric-sum) is

$$
\boxed{\sum_{r=1}^n\cos(r\theta)
=\frac{\cos(n\theta)-\cos((n+1)\theta)}{2(1-\cos\theta)}-\frac12.}
$$

At $\theta\in2\pi\mathbb Z$, the sum equals $n$; the printed quotient is undefined there, though its continuous limiting value is $n$.

Now take $\theta=2p\pi/(n+1)$ with $1\leq p\leq n$. This is not a multiple of $2\pi$, while $(n+1)\theta=2p\pi$ and $\cos(n\theta)=\cos(2p\pi-\theta)=\cos\theta$. Substitution gives

$$
\boxed{\sum_{r=1}^n\cos\left(\frac{2p\pi r}{n+1}\right)
=\frac{\cos\theta-1}{2(1-\cos\theta)}-\frac12=-1.}
$$

## 2A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2a/solution">Solution</h3>

↑ **Parent:** [2A](#2a)

Taking the [conjugate transpose](../../../linear-operator-theory.md#conjugate-transpose) of $U=A+iB$ and using that both parts are [Hermitian matrices](../../../hilbert-space.md#hermitian-operator) gives $U^\dagger=A-iB$. Addition and subtraction recover the [Hermitian parts of a unitary matrix](../../../linear-operator-theory.md#hermitian-parts-of-a-unitary-matrix):

$$
\boxed{A=\frac{U+U^\dagger}{2},\qquad
B=\frac{U-U^\dagger}{2i}.}
$$

These depend only on $U$, so any such decomposition has the same $A,B$ and is unique. Conversely the displayed expressions are [Hermitian matrices](../../../hilbert-space.md#hermitian-operator) and sum to $U$ in the form $A+iB$, establishing existence as well as uniqueness. Their commutation and quadratic relation are proved in the two labelled parts.

<h3 id="2a/i">i</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/i/solution">Solution</h4>

↑ **Parent:** [I](#2a/i)

By the [unitary matrix](../../../linear-operator-theory.md#unitary-matrix) identities,

$$
\begin{aligned}
U^\dagger U&=(A-iB)(A+iB)=A^2+B^2+i(AB-BA)=I,\\
UU^\dagger&=(A+iB)(A-iB)=A^2+B^2-i(AB-BA)=I.
\end{aligned}
$$

Subtracting the two equations yields $2i(AB-BA)=0$. Therefore

$$
\boxed{AB=BA.}
$$

The subtraction is important: entrywise real and imaginary parts cannot generally be used to separate these terms, since the [Hermitian matrices](../../../hilbert-space.md#hermitian-operator) need not have real entries.

<h3 id="2a/ii">ii</h3>

↑ **Parent:** [2A](#2a)

<h4 id="2a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2a/ii)

Adding the two expanded [unitary matrix](../../../linear-operator-theory.md#unitary-matrix) identities instead cancels the commutator and gives $2(A^2+B^2)=2I$. Hence

$$
\boxed{A^2+B^2=I.}
$$

Together with part (i), this characterizes the commuting [Hermitian parts of a unitary matrix](../../../linear-operator-theory.md#hermitian-parts-of-a-unitary-matrix).

## 3F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3f/solution">Solution</h3>

↑ **Parent:** [3F](#3f)

The [ratio test](../../../real-analysis.md#ratio-test) states that, for a [series](../../../real-analysis.md#series-mathematics) $\sum a_n$ with nonzero terms eventually, if $|a_{n+1}/a_n|\to L<1$, the [series](../../../real-analysis.md#series-mathematics) converges absolutely; if $L>1$, including $L=\infty$, it diverges because its terms do not tend to zero. At $L=1$ the test is inconclusive: the [harmonic series](../../../real-analysis.md#harmonic-series) diverges while $\sum n^{-2}$ converges.

For $|x|<1$, the [ratio test](../../../real-analysis.md#ratio-test) applied to $x^n/n$ gives [absolute convergence](../../../real-analysis.md#absolute-convergence) when $x\ne0$, and at $x=0$ every such term vanishes. Thus

$$
\sum_{n=1}^N\frac{x^n-1}{n}
=\sum_{n=1}^N\frac{x^n}{n}-\sum_{n=1}^N\frac1n\longrightarrow-\infty.
$$

At $x=1$ all terms are zero, so the [series](../../../real-analysis.md#series-mathematics) converges to zero. At $x=-1$, the even terms vanish and the odd terms are $-2/n$, whose [partial sums](../../../real-analysis.md#partial-sum) tend to $-\infty$. Finally, if $|x|>1$, then $|x^n-1|/n\geq(|x|^n-1)/n\to\infty$, so the [term test for divergence](../../../real-analysis.md#term-test-for-divergence) applies. Consequently

$$
\boxed{\text{The series converges exactly for }x=1,\text{ and its sum there is }0.}
$$

## 4E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4e/solution">Solution</h3>

↑ **Parent:** [4E](#4e)

Fix $x\in(0,1)$. For any sufficiently small nonzero $h$, the additivity of the [Riemann integral](../../../real-analysis.md#riemann-integral) gives

$$
\frac{F(x+h)-F(x)}h-f(x)
=\frac1h\int_x^{x+h}[f(t)-f(x)]\,dt.
$$

Taking absolute values, for either sign of $h$,

$$
\left|\frac{F(x+h)-F(x)}h-f(x)\right|
\leq\sup_{|t-x|\leq|h|}|f(t)-f(x)|.
$$

Because $f$ is [continuous](../../../calculus.md#continuous-function) at $x$, the right side tends to zero. Thus the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) here follows directly from the difference quotient:

$$
\boxed{F'(x)=f(x)\quad(0<x<1).}
$$

Only [continuity](../../../calculus.md#continuous-function) at the point under consideration was used.

Without [continuity](../../../calculus.md#continuous-function), the assertion is false. Take the [Riemann integrable](../../../real-analysis.md#riemann-integrable-function) step function $f(t)=0$ for $t<1/2$ and $f(t)=1$ for $t\geq1/2$. Its primitive is $F(x)=0$ for $x\leq1/2$ and $F(x)=x-1/2$ for $x\geq1/2$. The left and right difference quotients at $1/2$ are respectively zero and one, so **the primitive need not be differentiable at every interior point**. A function with this single jump is [Riemann integrable](../../../real-analysis.md#riemann-integrable-function); changing its value at the jump does not change the [integral](../../../calculus.md#integral) or the counterexample.

## 5B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5b/a">a</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/a/solution">Solution</h4>

↑ **Parent:** [A](#5b/a)

In [suffix notation](../../../linear-algebra.md#einstein-notation), repeated indices are summed from one to three. The [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) and [Kronecker delta](../../../linear-algebra.md#kronecker-delta) contraction is

$$
\epsilon_{ijk}\epsilon_{k\ell m}=\delta_{i\ell}\delta_{jm}-\delta_{im}\delta_{j\ell}.
$$

For distinct free index pairs this follows from the two possible matching permutations and their signs; if either pair repeats an index both sides vanish. Therefore

$$
\begin{aligned}
[a\times(b\times c)]_i
&=\epsilon_{ijk}a_j\epsilon_{k\ell m}b_\ell c_m\\
&=(\delta_{i\ell}\delta_{jm}-\delta_{im}\delta_{j\ell})a_jb_\ell c_m\\
&=b_i a_jc_j-c_i a_jb_j.
\end{aligned}
$$

Recognizing the [dot products](../../../linear-algebra.md#dot-product) proves the [vector triple product identity](../../../calculus.md#vector-triple-product):

$$
\boxed{a\times(b\times c)=(a\cdot c)b-(a\cdot b)c.}
$$

<h4 id="5b/a/i">i</h4>

↑ **Parent:** [A](#5b/a)

<h5 id="5b/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5b/a/i)

Use the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) contraction $\epsilon_{ijk}\epsilon_{i\ell m}=\delta_{j\ell}\delta_{km}-\delta_{jm}\delta_{k\ell}$ in [suffix notation](../../../linear-algebra.md#einstein-notation):

$$
\begin{aligned}
(a\times b)\cdot(c\times d)
&=\epsilon_{ijk}a_jb_k\epsilon_{i\ell m}c_\ell d_m\\
&=(\delta_{j\ell}\delta_{km}-\delta_{jm}\delta_{k\ell})a_jb_kc_\ell d_m.
\end{aligned}
$$

Thus the [cross product](../../../vector-space.md#cross-product) contraction expands as

$$
\boxed{(a\times b)\cdot(c\times d)=(a\cdot c)(b\cdot d)-(a\cdot d)(b\cdot c).}
$$

<h4 id="5b/a/ii">ii</h4>

↑ **Parent:** [A](#5b/a)

<h5 id="5b/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5b/a/ii)

Put $\tau=a\cdot(b\times c)$. The [vector triple product identity](../../../calculus.md#vector-triple-product) gives

$$
(b\times c)\times(c\times a)
=[(b\times c)\cdot a]c-[(b\times c)\cdot c]a=\tau c.
$$

Cyclic invariance of the [scalar triple product](../../../linear-algebra.md#scalar-triple-product) gives $(a\times b)\cdot c=\tau$. Hence the [squared scalar triple product from cyclic cross products](../../../linear-algebra.md#squared-scalar-triple-product-from-cyclic-cross-products) is

$$
\boxed{(a\times b)\cdot[(b\times c)\times(c\times a)]=[a\cdot(b\times c)]^2.}
$$

If an expansion entirely in pairwise [dot products](../../../linear-algebra.md#dot-product) is desired, expand the [Gram determinant](../../../linear-algebra.md#gram-determinant) of $a,b,c$:

$$
\boxed{|a|^2|b|^2|c|^2+2(a\cdot b)(b\cdot c)(c\cdot a)
-|a|^2(b\cdot c)^2-|b|^2(c\cdot a)^2-|c|^2(a\cdot b)^2.}
$$

Both expressions remain valid for degenerate, including linearly dependent, vectors.

<h3 id="5b/b">b</h3>

↑ **Parent:** [5B](#5b)

<h4 id="5b/b/solution">Solution</h4>

↑ **Parent:** [B](#5b/b)

The [parametric equation of a straight line](../../../geometry-and-topology.md#parametric-equation-of-a-straight-line) through $a$ with unit direction $\widehat t$ is

$$
\boxed{r=a+s\widehat t,\qquad s\in\mathbb R.}
$$

If the two lines meet, then $a_1+s\widehat t_1=a_2+t\widehat t_2$ for some real $s,t$, so $a_1-a_2$ lies in the [linear span](../../../vector-space.md#linear-span) of their direction vectors. Its [dot product](../../../linear-algebra.md#dot-product) with their [cross product](../../../vector-space.md#cross-product) is consequently zero:

$$
\boxed{(a_1-a_2)\cdot(\widehat t_1\times\widehat t_2)=0.}
$$

This is not sufficient without excluding parallel lines. For instance $a_1=(0,0,0)$, $a_2=(0,1,0)$ and $\widehat t_1=\widehat t_2=(1,0,0)$ satisfy it, but the lines are distinct and never meet. For nonparallel lines the condition is sufficient, because the two directions span the plane perpendicular to their nonzero [cross product](../../../vector-space.md#cross-product).

For nonparallel [skew lines](../../../geometry-and-topology.md#skew-lines), put $n=(\widehat t_1\times\widehat t_2)/|\widehat t_1\times\widehat t_2|$. Every joining vector is $a_1-a_2+s\widehat t_1-t\widehat t_2$, with fixed component $(a_1-a_2)\cdot n$ along $n$. Its length is at least the absolute value of that component. Its perpendicular component can be canceled by a unique choice of $s,t$, since the two independent directions span $n^\perp$. This lower bound is attained, proving the [distance between skew lines](../../../geometry-and-topology.md#distance-between-skew-lines):

$$
\boxed{d=\frac{|(a_1-a_2)\cdot(\widehat t_1\times\widehat t_2)|}{|\widehat t_1\times\widehat t_2|}.}
$$

## 6A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6a/solution">Solution</h3>

↑ **Parent:** [6A](#6a)

For two [upper triangular matrices](../../../linear-algebra.md#upper-triangular-matrix) and $i>j$,

$$
(AB)_{ij}=\sum_{k=1}^3A_{ik}B_{kj}=0.
$$

Indeed a potentially nonzero factor $A_{ik}$ requires $k\geq i$, while a potentially nonzero $B_{kj}$ requires $k\leq j$. These requirements cannot both hold when $i>j$. Thus their [matrix product](../../../vector-space.md#matrix-product) is upper triangular.

Direct [matrix multiplication](../../../vector-space.md#matrix-multiplication) for the given $A$ gives

$$
A^2=\begin{pmatrix}1&0&2\\0&1&-2\\0&0&1\end{pmatrix},\qquad
A^3=\begin{pmatrix}1&2&-2\\0&-1&3\\0&0&-1\end{pmatrix}.
$$

Adding $A^3+A^2-A$ yields $I$, so $A(A^2+A-I)=(A^2+A-I)A=I$. Hence

$$
\boxed{A^{-1}=A^2+A-I=\begin{pmatrix}1&2&2\\0&-1&-1\\0&0&-1\end{pmatrix}.}
$$

Every nonnegative [matrix power](../../../vector-space.md#matrix-power) is in $\operatorname{span}\{I,A,A^2\}$: reduce powers of degree at least three using $A^3=-A^2+A+I$. More formally, repeated reduction shows that products of any two polynomials of degree at most two in $A$ again lie in this span. Since $A^{-1}$ also lies in it, positive powers of $A^{-1}$ prove the same assertion for all negative integers. This is an instance of the [integer powers for an annihilating polynomial with roots one and minus one](../../../linear-operator-theory.md#integer-powers-for-an-annihilating-polynomial-with-roots-one-and-minus-one), because $A^3+A^2-A-I=(A-I)(A+I)^2=0$.

To find the required entries for every integer, use the block upper-triangular structure. The top-left entry of $A^n$ is $1$ for positive and negative powers. Its lower-right block is

$$
J=-I_2+N=-(I_2-N),\qquad
N=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad N^2=0.
$$

The identity $(I_2-N)^n=I_2-nN$ holds for all integers: multiplication adds the coefficients of $N$, and $(I_2-N)^{-1}=I_2+N$ proves the negative cases. Therefore

$$
\boxed{(A^n)_{11}=1,\quad(A^n)_{22}=(-1)^n,\quad(A^n)_{23}=n(-1)^{n-1}.}
$$

Write $s=(-1)^n$ and $A^n=\alpha_nA^2+\beta_nA+\gamma_nI$. Comparing those three entries gives

$$
\alpha_n+\beta_n+\gamma_n=1,\qquad
\alpha_n-\beta_n+\gamma_n=s,\qquad
-2\alpha_n+\beta_n=-ns.
$$

Subtracting the first two equations finds $\beta_n$; the third then finds $\alpha_n$, and the first finds $\gamma_n$. The unique solution is

$$
\boxed{\alpha_n=\frac{1-s}{4}+\frac{ns}{2},\quad
\beta_n=\frac{1-s}{2},\quad
\gamma_n=\frac{1+3s}{4}-\frac{ns}{2},\qquad s=(-1)^n.}
$$

For clarity, substituting also gives the full [matrix power](../../../vector-space.md#matrix-power)

$$
\boxed{A^n=\begin{pmatrix}
1&1-s&(1-s)/2+ns\\0&s&-ns\\0&0&s
\end{pmatrix}\quad(n\in\mathbb Z).}
$$

## 7C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7c/solution">Solution</h3>

↑ **Parent:** [7C](#7c)

If $e_1,\ldots,e_n$ are [orthonormal](../../../linear-algebra.md#orthonormal-set), any relation $\sum_i c_ie_i=0$ gives $c_j=0$ on taking the [dot product](../../../linear-algebra.md#dot-product) with $e_j$. Thus the vectors are [linearly independent](../../../vector-space.md#linear-independence). A linearly independent set of $n$ vectors in the $n$-dimensional [vector space](../../../vector-space.md) $\mathbb R^n$ is a [basis](../../../vector-space.md#basis), proving the claim.

Expand both $x$ and $f$ in this [orthonormal basis](../../../linear-algebra.md#orthonormal-basis), writing $f_i=e_i\cdot f$. Since $Ae_i=\lambda_ie_i$, the linear equation becomes

$$
\sum_i(\lambda_i-\mu)a_ie_i=\sum_if_ie_i.
$$

Comparing the unique [basis](../../../vector-space.md#basis) coefficients gives, when $\mu$ is not an [eigenvalue](../../../linear-operator-theory.md#eigenvalue),

$$
\boxed{a_i=\frac{e_i\cdot f}{\lambda_i-\mu},\qquad
x=\sum_i\frac{e_i\cdot f}{\lambda_i-\mu}e_i.}
$$

If $\mu=\lambda_1$, the equation is solvable exactly when $e_i\cdot f=0$ for every $i$ with $\lambda_i=\mu$. For those indices $a_i$ is arbitrary; for all other indices the displayed formula still applies. Thus repeated [eigenvalues](../../../linear-operator-theory.md#eigenvalue) require orthogonality to the entire corresponding [eigenspace](../../../linear-operator-theory.md#eigenspace), not merely to one chosen [eigenvector](../../../linear-operator-theory.md#eigenvector). This is the finite-dimensional [Fredholm solvability condition for a self-adjoint operator](../../../linear-operator-theory.md#fredholm-solvability-condition-for-a-self-adjoint-operator).

For the specific real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix), choose

$$
e_1=\frac1{\sqrt2}(1,-1,0),\quad\lambda_1=1;\qquad
e_2=\frac1{\sqrt2}(1,1,0),\quad\lambda_2=3;\qquad
e_3=(0,0,1),\quad\lambda_3=3.
$$

Their [dot products](../../../linear-algebra.md#dot-product) with $f$ are $-1/\sqrt2$, $3/\sqrt2$ and $3$. At $\mu=2$ this gives

$$
\boxed{a_1=1/\sqrt2,\quad a_2=3/\sqrt2,\quad a_3=3,\qquad x=(2,1,3).}
$$

One can check $(A-2I)x=f$ directly. At $\mu=1$, the first coefficient equation would require $0\cdot a_1=-1/\sqrt2$, which is impossible. Hence **there is no solution when $\mu=1$**; the nonzero projection onto its [eigenspace](../../../linear-operator-theory.md#eigenspace) is the obstruction.

## 8C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8c/solution">Solution</h3>

↑ **Parent:** [8C](#8c)

Let $H$ be a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) and $He=\lambda e$ with $e\ne0$. The [inner product](../../../linear-algebra.md#inner-product) $e^\dagger He$ is real because its conjugate equals $e^\dagger H^\dagger e=e^\dagger He$. But it also equals $\lambda e^\dagger e$, with $e^\dagger e>0$. Thus every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is real. For two [eigenvectors](../../../linear-operator-theory.md#eigenvector),

$$
e_i^\dagger He_j=\lambda_j e_i^\dagger e_j
=(He_i)^\dagger e_j=\lambda_i e_i^\dagger e_j.
$$

When $\lambda_i\ne\lambda_j$, this proves $e_i^\dagger e_j=0$, so the [eigenvectors](../../../linear-operator-theory.md#eigenvector) are orthogonal.

For a real [antisymmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix), $(iA)^\dagger=-iA^T=iA$, so $iA$ is a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator). Its real [eigenvalues](../../../linear-operator-theory.md#eigenvalue) imply that the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $A$ are purely imaginary. To ensure a nonzero one without assuming it, write

$$
A=\begin{pmatrix}0&-w_3&w_2\\w_3&0&-w_1\\-w_2&w_1&0\end{pmatrix},\qquad w\ne0.
$$

Expansion of the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) gives $\det(tI-A)=t(t^2+|w|^2)$. Therefore the nonzero [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $-i\theta$ exists with $\theta=|w|>0$, and a nonzero complex [eigenvector](../../../linear-operator-theory.md#eigenvector) $e_1=u+iv$ satisfies

$$
A(u+iv)=-i\theta(u+iv)=\theta v-i\theta u.
$$

Separating real and imaginary parts gives

$$
\boxed{Au=\theta v,\qquad Av=-\theta u.}
$$

Neither real vector can vanish, since either vanishing would force the other to vanish. Antisymmetry yields $0=u\cdot Au=\theta u\cdot v$ and

$$
-\theta|u|^2=u\cdot Av=-(Au)\cdot v=-\theta|v|^2.
$$

Thus $u,v$ are orthogonal and have equal length.

In odd dimension $\det A=\det A^T=\det(-A)=-\det A$, so $\det A=0$. Its real homogeneous system therefore has a nonzero real [eigenvector](../../../linear-operator-theory.md#eigenvector) $e_3$ with $Ae_3=0$. It is perpendicular to $u,v$, because $e_3\cdot Au=-(Ae_3)\cdot u=0$ and similarly for $Av$. Normalize it and choose its sign so $(u/|u|,v/|v|,e_3)$ is positively oriented; this is an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis).

The [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) series converges absolutely, allowing even and odd terms to be grouped. Since $A^2u=-\theta^2u$ and $A^2v=-\theta^2v$, it acts as

$$
Ru=u\cos\theta+v\sin\theta,\qquad
Rv=v\cos\theta-u\sin\theta,\qquad Re_3=e_3.
$$

Consequently the [skew-symmetric exponential as an axial rotation](../../../linear-operator-theory.md#skew-symmetric-exponential-as-an-axial-rotation) has, in the displayed [orthonormal basis](../../../linear-algebra.md#orthonormal-basis), the matrix

$$
\boxed{\begin{pmatrix}\cos\theta&-\sin\theta&0\\\sin\theta&\cos\theta&0\\0&0&1\end{pmatrix}.}
$$

It is orthogonal with determinant one, fixes its axis and rotates the perpendicular plane. Hence **$R=e^A$ is a rotation matrix**, with angle $\theta$ about the chosen oriented axis.

## 9F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9f/i">i</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/i/solution">Solution</h4>

↑ **Parent:** [I](#9f/i)

The [comparison test for series](../../../real-analysis.md#comparison-test-for-series) says that an eventual upper bound by a convergent positive [series](../../../real-analysis.md#series-mathematics) proves convergence, while an eventual lower bound by a divergent positive [series](../../../real-analysis.md#series-mathematics) proves divergence. The [p-series](../../../real-analysis.md#p-series) $\sum n^{-s}$ converges exactly when $s>1$.

If $p>1$, then $(\log n)^q\geq1$ for all sufficiently large $n$, so

$$
0<\frac1{n^p(\log n)^q}\leq\frac1{n^p},
$$

and the [series](../../../real-analysis.md#series-mathematics) converges. If $0<p<1$, choose $\eta=(1-p)/2>0$. The allowed logarithmic bound, applied with exponent $\eta/q$, gives $(\log n)^q<n^\eta$ eventually. Thus

$$
\frac1{n^p(\log n)^q}>\frac1{n^{p+\eta}},\qquad p+\eta=(p+1)/2<1,
$$

and the [series](../../../real-analysis.md#series-mathematics) diverges.

For $p=1$, use the [integral test for convergence](../../../real-analysis.md#integral-test-for-convergence): for an eventually positive decreasing function $g$, $\sum g(n)$ and $\int g(x)\,dx$ either both converge or both diverge. Here $g(x)=1/[x(\log x)^q]$ is decreasing for $x>1$, and the substitution $u=\log x$ gives

$$
\int_2^\infty\frac{dx}{x(\log x)^q}
=\int_{\log2}^\infty u^{-q}\,du.
$$

This integral converges exactly when $q>1$. Hence the [polynomial-logarithmic series convergence](../../../real-analysis.md#polynomial-logarithmic-series-convergence) classification is

$$
\boxed{\text{Convergence iff }p>1\text{ or }(p=1\text{ and }q>1).}
$$

All other allowed positive $p,q$ give divergence.

<h3 id="9f/ii">ii</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9f/ii)

For any fixed $r>0$, $\log y=o(y^{1/r})$ as $y\to\infty$. For example, l'Hôpital's rule applied to $\log y/y^{1/r}$ gives the limit zero. With $y=\log n$, this implies $(\log\log n)^r<\log n$ eventually. Therefore

$$
\frac1{n(\log\log n)^r}>\frac1{n\log n}
$$

for all sufficiently large $n$. The comparison [series](../../../real-analysis.md#series-mathematics) diverges by the [integral test for convergence](../../../real-analysis.md#integral-test-for-convergence), since

$$
\int^M\frac{dx}{x\log x}=\log\log M+\text{constant}\longrightarrow\infty.
$$

The [comparison test for series](../../../real-analysis.md#comparison-test-for-series) gives

$$
\boxed{\sum_{n=3}^\infty\frac1{n(\log\log n)^r}\text{ diverges for every }r>0.}
$$

One may obtain the same growth bound by extending the given logarithmic estimate to real $y$ through $\lceil y\rceil$ and choosing any exponent smaller than $1/r$; no special convergence test for iterated logarithms is needed.

## 10D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10d/a">a</h3>

↑ **Parent:** [10D](#10d)

<h4 id="10d/a/solution">Solution</h4>

↑ **Parent:** [A](#10d/a)

The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) states that, if $f$ is a [continuous function](../../../calculus.md#continuous-function) on a [closed interval](../../../real-analysis.md#closed-real-interval) $[a,b]$, every value between $f(a)$ and $f(b)$ equals $f(c)$ for some $c\in[a,b]$. If the value is strictly between the endpoint values, $c$ may be chosen in $(a,b)$.

Here is a proof from the [supremum](../../../real-analysis.md#supremum) property of the real numbers. Suppose $f(a)<y<f(b)$; the reverse inequality is reduced to this case by replacing $f,y$ with $-f,-y$. Let

$$
E=\{t\in[a,b]:f(t)\leq y\},\qquad c=\sup E.
$$

The set is nonempty because it contains $a$ and is bounded above by $b$. [Continuity](../../../calculus.md#continuous-function) at $a$ supplies points of $E$ to the right of $a$, while [continuity](../../../calculus.md#continuous-function) at $b$ excludes a neighborhood of $b$ from $E$. Hence $a<c<b$. By the definition of [supremum](../../../real-analysis.md#supremum), there are $t_n\in E$ with $t_n\to c$. [Continuity](../../../calculus.md#continuous-function) gives $f(c)=\lim f(t_n)\leq y$. If $f(c)<y$, [continuity](../../../calculus.md#continuous-function) would give a point just to the right of $c$ still satisfying $f(t)<y$, contradicting that $c$ is an upper bound for $E$. Thus $f(c)=y$. Values equal to either endpoint are attained at that endpoint, completing the proof.

<h3 id="10d/b">b</h3>

↑ **Parent:** [10D](#10d)

<h4 id="10d/b/solution">Solution</h4>

↑ **Parent:** [B](#10d/b)

Let $u,v\in f(I)$ with $u<y<v$. Choose preimages $x_u,x_v\in I$, and let $a=\min(x_u,x_v)$, $b=\max(x_u,x_v)$. The defining property of a [real interval](../../../real-analysis.md#interval-mathematics) ensures $[a,b]\subseteq I$. The restriction of $f$ to this [closed interval](../../../real-analysis.md#closed-real-interval) is [continuous](../../../calculus.md#continuous-function), and its endpoint values are $u,v$ in one order or the other. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) supplies $c\in[a,b]\subseteq I$ with $f(c)=y$. Thus every value between two image values lies in the image, proving

$$
\boxed{f(I)\text{ is a real interval}.}
$$

The [continuous image of a real interval](../../../calculus.md#continuous-image-of-a-real-interval) result does not require $I$ itself to be closed or bounded; only the segment between the chosen preimages is used. Empty and single-point images also satisfy the interval property.

<h3 id="10d/c">c</h3>

↑ **Parent:** [10D](#10d)

<h4 id="10d/c/i">i</h4>

↑ **Parent:** [C](#10d/c)

<h5 id="10d/c/i/solution">Solution</h5>

↑ **Parent:** [I](#10d/c/i)

**No such continuous function exists.** The [extreme value theorem](../../../real-analysis.md#extreme-value-theorem) makes every [continuous function](../../../calculus.md#continuous-function) on the [closed interval](../../../real-analysis.md#closed-real-interval) $[0,1]$ bounded and gives it a finite maximum. Its image therefore cannot equal the unbounded [real interval](../../../real-analysis.md#interval-mathematics) $[0,\infty)$.

<h4 id="10d/c/ii">ii</h4>

↑ **Parent:** [C](#10d/c)

<h5 id="10d/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10d/c/ii)

The [continuous function](../../../calculus.md#continuous-function)

$$
\boxed{f(x)=\frac1x-1\qquad(0<x\leq1)}
$$

has the required image. Its values are nonnegative, and for every $y\geq0$ the point $x=1/(y+1)\in(0,1]$ satisfies $f(x)=y$. Thus the image is exactly $[0,\infty)$. The missing left endpoint permits unboundedness without a failure of [continuity](../../../calculus.md#continuous-function) on the domain.

<h4 id="10d/c/iii">iii</h4>

↑ **Parent:** [C](#10d/c)

<h5 id="10d/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#10d/c/iii)

A suitable [continuous function](../../../calculus.md#continuous-function) is

$$
\boxed{f(x)=\frac{\sin(1/x)}x\qquad(0<x\leq1).}
$$

For $t_k=\pi/2+2\pi k$ and $u_k=3\pi/2+2\pi k$,

$$
f(1/t_k)=t_k\longrightarrow+\infty,\qquad
f(1/u_k)=-u_k\longrightarrow-\infty.
$$

All these arguments lie in $(0,1]$. Its image is a [real interval](../../../real-analysis.md#interval-mathematics) by the [continuous image of a real interval](../../../calculus.md#continuous-image-of-a-real-interval) result, and it is unbounded both above and below. Given any real $y$, choose two of the displayed points with function values on opposite sides of $y$, then apply the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) on the segment joining them. Hence **the image is all of $\mathbb R$**. A monotone example would not suffice here; the oscillation gives both directions of unboundedness near the same missing endpoint.

## 11D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11d/a">a</h3>

↑ **Parent:** [11D](#11d)

<h4 id="11d/a/solution">Solution</h4>

↑ **Parent:** [A](#11d/a)

By [differentiability implies continuity](../../../analysis.md#differentiability-implies-continuity), $f(x+h)\to f(x)$. Add and subtract $f(x+h)g(x)$ in the difference quotient:

$$
\frac{f(x+h)g(x+h)-f(x)g(x)}h
=f(x+h)\frac{g(x+h)-g(x)}h
+g(x)\frac{f(x+h)-f(x)}h.
$$

The two quotient limits exist by the given [differentiability](../../../analysis.md#differentiability). Taking the limit and using [continuity](../../../calculus.md#continuous-function) yields the [product rule](../../../calculus.md#product-rule):

$$
\boxed{(fg)'(x)=f(x)g'(x)+g(x)f'(x).}
$$

Thus the product is [differentiable](../../../analysis.md#differentiable-function) at the specified point; differentiability elsewhere is not needed.

<h3 id="11d/b">b</h3>

↑ **Parent:** [11D](#11d)

<h4 id="11d/b/solution">Solution</h4>

↑ **Parent:** [B](#11d/b)

At zero, $g(0)=0$ and

$$
\frac{g(h)-g(0)}h=hf(h)\longrightarrow0
$$

by [continuity](../../../calculus.md#continuous-function) of $f$ at zero. Thus $g$ is always [differentiable](../../../analysis.md#differentiable-function) there, with $g'(0)=0$, regardless of whether $f'(0)$ exists.

At $x\ne0$, if $f$ is [differentiable](../../../analysis.md#differentiable-function), the [product rule](../../../calculus.md#product-rule) applied to $t^2f(t)$ proves that $g$ is [differentiable](../../../analysis.md#differentiable-function). Conversely, if $g$ is [differentiable](../../../analysis.md#differentiable-function) at $x$, the function $t^{-2}$ is [differentiable](../../../analysis.md#differentiable-function) on a neighborhood of $x$. Apply the [product rule](../../../calculus.md#product-rule) to $f(t)=t^{-2}g(t)$ on that neighborhood. This proves the [differentiability restored by a quadratic zero](../../../calculus.md#differentiability-restored-by-a-quadratic-zero) equivalence:

$$
\boxed{g\text{ is differentiable at }x\iff x=0\text{ or }f\text{ is differentiable at }x.}
$$

At a nonzero differentiability point, $g'(x)=2xf(x)+x^2f'(x)$.

<h3 id="11d/c">c</h3>

↑ **Parent:** [11D](#11d)

<h4 id="11d/c/solution">Solution</h4>

↑ **Parent:** [C](#11d/c)

For the necessity in the [differentiability of the square of a continuous function](../../../analysis.md#differentiability-of-the-square-of-a-continuous-function), suppose $g=f^2$ is [differentiable](../../../analysis.md#differentiable-function) at $x$. If $f(x)\ne0$, [continuity](../../../calculus.md#continuous-function) makes $f(x+h)+f(x)$ nonzero for small $h$, and

$$
\frac{f(x+h)-f(x)}h
=\frac{g(x+h)-g(x)}{h[f(x+h)+f(x)]}
\longrightarrow\frac{g'(x)}{2f(x)}.
$$

Hence $f$ is [differentiable](../../../analysis.md#differentiable-function) at $x$, giving alternative (i).

If $f(x)=0$, $g(x)=0$ is a minimum because $g\geq0$. The right difference quotients of $g$ are nonnegative and the left ones are nonpositive; since their common limit exists, it must be zero. Thus $g'(x)=0$, and

$$
\frac{f(x+h)^2}{|h|}
=\operatorname{sgn}(h)\frac{g(x+h)-g(x)}h\longrightarrow0.
$$

Taking square roots of this nonnegative expression shows $f(x+h)/\sqrt{|h|}\to0$, giving alternative (ii). The two labelled parts below establish sufficiency of the respective alternatives. Together they prove the full stated equivalence, including the zero of $f$ where squaring can remove a failure of [differentiability](../../../analysis.md#differentiability).

<h4 id="11d/c/i">i</h4>

↑ **Parent:** [C](#11d/c)

<h5 id="11d/c/i/solution">Solution</h5>

↑ **Parent:** [I](#11d/c/i)

If $f$ is [differentiable](../../../analysis.md#differentiable-function) at $x$, the [product rule](../../../calculus.md#product-rule) applied to $f\cdot f$ gives

$$
\boxed{g'(x)=2f(x)f'(x).}
$$

This proves sufficiency of the first alternative. No additional growth condition is required; if $f(x)=0$, the derivative of the square is zero.

<h4 id="11d/c/ii">ii</h4>

↑ **Parent:** [C](#11d/c)

<h5 id="11d/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11d/c/ii)

Suppose $f(x)=0$ and $f(x+h)/\sqrt{|h|}\to0$. Then

$$
\frac{g(x+h)-g(x)}h
=\operatorname{sgn}(h)\left(\frac{f(x+h)}{\sqrt{|h|}}\right)^2\longrightarrow0.
$$

Therefore

$$
\boxed{g'(x)=0.}
$$

This proves sufficiency of the second alternative even if $f$ itself is not [differentiable](../../../analysis.md#differentiable-function) at $x$. For example, $f(t)=|t|^{3/4}$ is [continuous](../../../calculus.md#continuous-function) and not [differentiable](../../../analysis.md#differentiable-function) at zero, while $g(t)=|t|^{3/2}$ is [differentiable](../../../analysis.md#differentiable-function) there with derivative zero.

## 12E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12e/solution">Solution</h3>

↑ **Parent:** [12E](#12e)

First establish the interior convergence lemma for a [power series](../../../real-analysis.md#power-series). If $\sum a_nw^n$ converges at some $w\ne0$, its terms are bounded: $|a_nw^n|\leq M$ for a finite $M$. For every $|z|<|w|$,

$$
|a_nz^n|\leq M\left(\frac{|z|}{|w|}\right)^n.
$$

Comparison with a convergent [geometric series](../../../real-analysis.md#geometric-series) proves [absolute convergence](../../../real-analysis.md#absolute-convergence) at $z$.

Now let

$$
R=\sup\{|w|:\textstyle\sum a_nw^n\text{ converges}\}\in[0,\infty].
$$

The set contains zero, since at $w=0$ only the constant term remains. If $|z|<R$, the definition of [supremum](../../../real-analysis.md#supremum) gives a point of convergence $w$ with $|w|>|z|$. The lemma proves [absolute convergence](../../../real-analysis.md#absolute-convergence) at $z$. If $|z|>R$, convergence would place $|z|$ in the set defining $R$, a contradiction. This proves the existence of a [radius of convergence](../../../real-analysis.md#radius-of-convergence), including $R=0$ and $R=\infty$:

$$
\boxed{\text{Convergence for }|z|<R,\qquad\text{divergence for }|z|>R.}
$$

The proof leaves behavior on $|z|=R$ open; it need not be uniform around that circle. The two examples illustrate opposite possibilities.

<h3 id="12e/i">i</h3>

↑ **Parent:** [12E](#12e)

<h4 id="12e/i/solution">Solution</h4>

↑ **Parent:** [I](#12e/i)

For $z\ne0$, the ratio of successive absolute terms is

$$
\frac{|z^{n+1}|/(n+1)^2}{|z^n|/n^2}
=|z|\left(\frac n{n+1}\right)^2\longrightarrow|z|.
$$

The [ratio test](../../../real-analysis.md#ratio-test) therefore gives [absolute convergence](../../../real-analysis.md#absolute-convergence) for $|z|<1$ and divergence for $|z|>1$, while at zero the series is trivially convergent. Hence $R=1$. On the boundary, $|z^n/n^2|=1/n^2$, and the convergent [p-series](../../../real-analysis.md#p-series) proves

$$
\boxed{R=1;\quad\text{absolute convergence at every point of }|z|=1.}
$$

<h3 id="12e/ii">ii</h3>

↑ **Parent:** [12E](#12e)

<h4 id="12e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#12e/ii)

For $|z|=r<1$, the inequality $n!\geq n$ for $n\geq1$ gives

$$
\sum_{n=0}^\infty|z|^{n!}
\leq r+\sum_{n=1}^\infty r^n<\infty.
$$

The first $r$ comes from $0!=1$; both initial terms have exponent one. Thus the [factorial-gap power series](../../../real-analysis.md#factorial-gap-power-series) converges absolutely inside the unit circle. For $|z|>1$, its terms have magnitudes $|z|^{n!}\to\infty$, so the [term test for divergence](../../../real-analysis.md#term-test-for-divergence) proves divergence and $R=1$.

At every point with $|z|=1$, each term has magnitude one, so the terms cannot tend to zero, regardless of their phases. Hence

$$
\boxed{R=1;\quad\text{divergence at every point of }|z|=1.}
$$

The large gaps between exponents make this a [lacunary power series](../../../real-analysis.md#lacunary-power-series); cancellation cannot overcome the necessary condition that the terms of a convergent [series](../../../real-analysis.md#series-mathematics) tend to zero.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
