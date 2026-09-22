# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2011/PaperIA_1.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2011/PaperIA_1.pdf)

**Table of contents**

- [1C](#1c)
  - [Solution](#1c/solution)
  - [i](#1c/i)
    - [Solution](#1c/i/solution)
  - [ii](#1c/ii)
    - [Solution](#1c/ii/solution)
- [2A](#2a)
  - [Solution](#2a/solution)
- [3F](#3f)
  - [a](#3f/a)
    - [Solution](#3f/a/solution)
  - [b](#3f/b)
    - [Solution](#3f/b/solution)
  - [c](#3f/c)
    - [Solution](#3f/c/solution)
  - [d](#3f/d)
    - [Solution](#3f/d/solution)
- [4D](#4d)
  - [i](#4d/i)
    - [Solution](#4d/i/solution)
  - [ii](#4d/ii)
    - [Solution](#4d/ii/solution)
- [5C](#5c)
  - [Solution](#5c/solution)
- [6A](#6a)
  - [a](#6a/a)
    - [Solution](#6a/a/solution)
  - [b](#6a/b)
    - [Solution](#6a/b/solution)
  - [c](#6a/c)
    - [Solution](#6a/c/solution)
  - [d](#6a/d)
    - [Solution](#6a/d/solution)
- [7B](#7b)
  - [a](#7b/a)
    - [Solution](#7b/a/solution)
  - [b](#7b/b)
    - [Solution](#7b/b/solution)
  - [c](#7b/c)
    - [Solution](#7b/c/solution)
- [8B](#8b)
  - [a](#8b/a)
    - [i](#8b/a/i)
      - [Solution](#8b/a/i/solution)
    - [ii](#8b/a/ii)
      - [Solution](#8b/a/ii/solution)
    - [iii](#8b/a/iii)
      - [Solution](#8b/a/iii/solution)
  - [b](#8b/b)
    - [Solution](#8b/b/solution)
- [9F](#9f)
  - [a](#9f/a)
    - [Solution](#9f/a/solution)
  - [b](#9f/b)
    - [Solution](#9f/b/solution)
  - [c](#9f/c)
    - [Solution](#9f/c/solution)
- [10E](#10e)
  - [Solution](#10e/solution)
  - [i](#10e/i)
    - [Solution](#10e/i/solution)
  - [ii](#10e/ii)
    - [Solution](#10e/ii/solution)
  - [iii](#10e/iii)
    - [Solution](#10e/iii/solution)
  - [iv](#10e/iv)
    - [Solution](#10e/iv/solution)
- [11E](#11e)
  - [Solution](#11e/solution)
  - [i](#11e/i)
    - [Solution](#11e/i/solution)
  - [ii](#11e/ii)
    - [Solution](#11e/ii/solution)
- [12D](#12d)
  - [Solution](#12d/solution)

## 1C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1c/solution">Solution</h3>

↑ **Parent:** [1C](#1c)

For a nonzero [complex number](../../../complex-analysis.md#complex-number), write $z=re^{i\theta}$ with $r=|z|>0$ and principal [complex argument](../../../complex-analysis.md#argument-complex-analysis) $-\pi<\theta\le\pi$. The [principal complex logarithm](../../../analysis.md#principal-complex-logarithm) and corresponding [complex exponentiation](../../../analysis.md#complex-exponentiation) are

$$
\boxed{\operatorname{Log}z=\log r+i\theta,\qquad z^a=\exp(a\operatorname{Log}z).}
$$

The value at zero is not defined by this formula. The choice of [complex argument](../../../complex-analysis.md#argument-complex-analysis) matters: these are single-valued principal powers, rather than all values of a multivalued [complex logarithm](../../../analysis.md#complex-logarithm).

For the requested sketch, $(1+i)\operatorname{Log}z=(\log r-\theta)+i(\log r+\theta)$. Its [complex exponential](../../../calculus.md#complex-exponential-function) has [complex modulus](../../../complex-analysis.md#complex-modulus) $e^{\log r-\theta}$, so

$$
\boxed{|z^{1+i}|=1\quad\Longleftrightarrow\quad r=e^\theta,\qquad-\pi<\theta\le\pi.}
$$

This is one turn of a [logarithmic spiral](../../../topology.md#logarithmic-spiral), with increasing radius as the polar angle increases. It passes through $1$ at $\theta=0$, approaches the excluded endpoint $-e^{-\pi}$ from below the negative real axis, and ends at the included endpoint $-e^\pi$ from above that axis. The endpoint distinction follows from the chosen principal [complex argument](../../../complex-analysis.md#argument-complex-analysis).<a id="1c/image-one-turn-of-the-principal-power-logarithmic-spiral-with-open-inner-and-closed-outer-endpoints"></a>


![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1-principal-spiral.png)

**[Figure 1](#1c/image-one-turn-of-the-principal-power-logarithmic-spiral-with-open-inner-and-closed-outer-endpoints). One turn of the principal-power logarithmic spiral, with open inner and closed outer endpoints**.

<h3 id="1c/i">i</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/i/solution">Solution</h4>

↑ **Parent:** [I](#1c/i)

The principal [complex exponentiation](../../../analysis.md#complex-exponentiation) gives $z^i=e^{-\theta}e^{i\log r}$. Equality to one requires its [complex modulus](../../../complex-analysis.md#complex-modulus) to be one, hence $\theta=0$, and then its [complex argument](../../../complex-analysis.md#argument-complex-analysis) requires $\log r\in2\pi\mathbb Z$. Thus **all solutions are positive real**, namely

$$
\boxed{z=e^{2\pi k},\qquad k\in\mathbb Z.}
$$

Substitution verifies every value, and the modulus condition excludes every nonreal value.

<h3 id="1c/ii">ii</h3>

↑ **Parent:** [1C](#1c)

<h4 id="1c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1c/ii)

Away from the negative real axis, the [complex conjugate](../../../complex-analysis.md#complex-conjugate) has principal [complex argument](../../../complex-analysis.md#argument-complex-analysis) $-\theta$. Consequently

$$
z^i+\overline z^{\,i}=(e^{-\theta}+e^\theta)e^{i\log r}=2\cosh\theta\,e^{i\log r}.
$$

Taking the [complex modulus](../../../complex-analysis.md#complex-modulus) gives $\cosh\theta=1$, hence $\theta=0$. The remaining equation is $e^{i\log r}=i$, so

$$
\boxed{z=e^{\pi/2+2\pi k},\qquad k\in\mathbb Z.}
$$

On the negative real axis, both $z$ and $\overline z$ have principal [complex argument](../../../complex-analysis.md#argument-complex-analysis) $\pi$, so the left-hand side has modulus $2e^{-\pi}$, not two. There are no additional solutions there. The printed second term is the principal power of $\overline z$, not the [complex conjugate](../../../complex-analysis.md#complex-conjugate) of $z^i$.

## 2A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2a/solution">Solution</h3>

↑ **Parent:** [2A](#2a)

Use [change of basis](../../../linear-algebra.md#change-of-basis) matrices whose columns are the respective [basis vectors](../../../vector-space.md#basis-vector) in standard coordinates:

$$
S_B=\begin{pmatrix}1&1\\1&-1\end{pmatrix},\quad
S_C=\begin{pmatrix}1&0&0\\1&1&1\\0&0&1\end{pmatrix},\quad
S_{B'}=\begin{pmatrix}0&2\\2&0\end{pmatrix},\quad
S_{C'}=\begin{pmatrix}1&0&1\\0&1&2\\-1&0&1\end{pmatrix}.
$$

The coordinate relation is $[\Phi(x)]_C=A[x]_B$. Therefore the standard-coordinate [matrix of a linear map](../../../vector-space.md#matrix-representation-of-a-linear-map) is $T=S_CAS_B^{-1}$, and the new coordinate matrix is $A'=S_{C'}^{-1}TS_{B'}$. Multiplying gives

$$
T=\begin{pmatrix}0&1\\2&0\\0&-1\end{pmatrix},\qquad
TS_{B'}=\begin{pmatrix}2&0\\0&4\\-2&0\end{pmatrix},\qquad
\boxed{A'=\begin{pmatrix}2&0\\0&4\\0&0\end{pmatrix}.}
$$

One can also read off the columns: the two new domain [basis vectors](../../../vector-space.md#basis-vector) map to twice the first and four times the second new codomain [basis vector](../../../vector-space.md#basis-vector). All four [change of basis](../../../linear-algebra.md#change-of-basis) matrices are invertible. In particular the printed codomain vectors are three-dimensional; retaining their third coordinates is essential.

## 3F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3f/a">a</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/a/solution">Solution</h4>

↑ **Parent:** [A](#3f/a)

The [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) states that **every bounded [sequence](../../../real-analysis.md#sequence) in $\mathbb R$ has a convergent [subsequence](../../../real-analysis.md#subsequence)**. More generally, a bounded [sequence](../../../real-analysis.md#sequence) in $\mathbb R^d$ has a [subsequence](../../../real-analysis.md#subsequence) converging to a point of $\mathbb R^d$.

<h3 id="3f/b">b</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/b/solution">Solution</h4>

↑ **Parent:** [B](#3f/b)

Take $a_n=n$. Every [subsequence](../../../real-analysis.md#subsequence) has the form $a_{n_k}=n_k$, with $n_k\ge k$, so it tends to positive infinity and cannot converge to a real number. Thus **this [sequence](../../../real-analysis.md#sequence) has no convergent [subsequence](../../../real-analysis.md#subsequence)**.

<h3 id="3f/c">c</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/c/solution">Solution</h4>

↑ **Parent:** [C](#3f/c)

Define $a_{2k}=0$ and $a_{2k-1}=k$. The odd-indexed terms are unbounded, while the even-indexed [subsequence](../../../real-analysis.md#subsequence) is identically zero and hence converges to zero. This gives **an unbounded [sequence](../../../real-analysis.md#sequence) with a convergent [subsequence](../../../real-analysis.md#subsequence)**.

<h3 id="3f/d">d</h3>

↑ **Parent:** [3F](#3f)

<h4 id="3f/d/solution">Solution</h4>

↑ **Parent:** [D](#3f/d)

The [floor function](../../../calculus.md#floor-function) has even value on indices congruent to zero or one modulo four, and odd value on indices congruent to two or three. Accordingly the displayed [sequence](../../../real-analysis.md#sequence) has terms $2+1/n$ in the first two residue classes and $-1/n$ in the other two. In particular,

$$
\boxed{a_{4k}=2+\frac1{4k}\longrightarrow2,\qquad
a_{4k+2}=-\frac1{4k+2}\longrightarrow0.}
$$

Every term is within $1/n$ of the set $\{0,2\}$. If a [subsequence](../../../real-analysis.md#subsequence) converged to $c\notin\{0,2\}$, its eventual distance from that set would be bounded below by a positive constant, contradicting this bound. **The complete set of subsequential limits is $\{0,2\}$.**

## 4D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4d/i">i</h3>

↑ **Parent:** [4D](#4d)

<h4 id="4d/i/solution">Solution</h4>

↑ **Parent:** [I](#4d/i)

For the [power series](../../../real-analysis.md#power-series) coefficient $c_n=n^2$, the [Cauchy-Hadamard theorem](../../../real-analysis.md#cauchy-hadamard-theorem) gives

$$
R^{-1}=\limsup_{n\to\infty}|c_n|^{1/n}
=\lim_{n\to\infty}\exp\!\left(\frac{2\log n}{n}\right)=1.
$$

Thus the **[radius of convergence](../../../real-analysis.md#radius-of-convergence) is $\boxed{R=1}$**. The [power series](../../../real-analysis.md#power-series) converges absolutely for $|z|<1$ and diverges for $|z|>1$. On $|z|=1$ its terms have modulus $n^2$, so they do not tend to zero and the series diverges there as well.

<h3 id="4d/ii">ii</h3>

↑ **Parent:** [4D](#4d)

<h4 id="4d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4d/ii)

The original PDF has coefficient $c_n=n^{\,n^{1/3}}$. Its $n$th root is

$$
|c_n|^{1/n}=n^{n^{-2/3}}
=\exp\!\left(\frac{\log n}{n^{2/3}}\right)\longrightarrow1.
$$

The [Cauchy-Hadamard theorem](../../../real-analysis.md#cauchy-hadamard-theorem) therefore gives **$\boxed{R=1}$**. Again the [power series](../../../real-analysis.md#power-series) converges absolutely inside the unit circle, while on that circle its terms do not tend to zero. The converted TeX loses the outer exponent and writes $n^{1/3}$; the calculation here uses the printed coefficient.

## 5C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5c/solution">Solution</h3>

↑ **Parent:** [5C](#5c)

In the parametric description, $a$ is a point of the [straight line](../../../geometry-and-topology.md#straight-line) and the nonzero [vector](../../../vector-space.md#vector) $b$ gives its direction. The real parameter runs through every point of that line. For the [cross product](../../../vector-space.md#cross-product) description, take another [cross product](../../../vector-space.md#cross-product) with $c$ and use the [vector triple product identity](../../../calculus.md#vector-triple-product):

$$
c\times(x\times c)=|c|^2x-(c\cdot x)c=c\times d.
$$

Hence every solution has the representation

$$
\boxed{x=a+\lambda(x)b,\qquad
a=\frac{c\times d}{|c|^2},\qquad b=c,\qquad
\lambda(x)=\frac{c\cdot x}{|c|^2}.}
$$

Here $a\cdot b=0$ and $|b|=|c|$, as required. Conversely,

$$
(a+\lambda c)\times c
=\frac{(c\times d)\times c}{|c|^2}
=d-\frac{(c\cdot d)c}{|c|^2}=d.
$$

Thus the perpendicularity assumption is sufficient, and the solutions form a [straight line](../../../geometry-and-topology.md#straight-line) parallel to $c$. When $d\ne0$, the [vector](../../../vector-space.md#vector) $d$ is perpendicular both to $c$ and to every position [vector](../../../vector-space.md#vector) on the line; it is the normal to the plane through the origin containing that line. The point $a=c\times d/|c|^2$ is the perpendicular foot from the origin. Its distance from the origin is $|d|/|c|$, since $c\cdot d=0$.

For a general parametric [straight line](../../../geometry-and-topology.md#straight-line), minimize the squared [Euclidean distance](../../../topological-analysis.md#euclidean-distance)

$$
|a+\lambda b-y|^2=|a-y|^2+2\lambda b\cdot(a-y)+\lambda^2|b|^2.
$$

This strictly convex [quadratic function](../../../polynomial.md#quadratic-function) has its unique minimum at $\lambda=b\cdot(y-a)/|b|^2$, giving the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection)

$$
\boxed{x_{\rm nearest}=a+\frac{b\cdot(y-a)}{|b|^2}b.}
$$

For the [cross product](../../../vector-space.md#cross-product) description, $a\cdot c=0$, so this becomes

$$
\boxed{x_{\rm nearest}=\frac{c\times d}{|c|^2}+\frac{c\cdot y}{|c|^2}c.}
$$

For the two planes, put $s=m\cdot n$ and $c=m\times n$. Nonparallel unit normals give $|s|<1$ and $|c|^2=1-s^2$. Seek the perpendicular foot in their span, $a=um+vn$. Its two [dot products](../../../linear-algebra.md#dot-product) impose $u+sv=\mu$ and $su+v=\nu$. Solving gives both requested descriptions of the intersection:

$$
\boxed{x=\frac{(\mu-s\nu)m+(\nu-s\mu)n}{1-s^2}+\lambda(m\times n),\qquad\lambda\in\mathbb R,}
$$

and

$$
\boxed{x\times(m\times n)=\nu m-\mu n.}
$$

Indeed the [vector triple product identity](../../../calculus.md#vector-triple-product) gives $x\times(m\times n)=m(x\cdot n)-n(x\cdot m)$. Conversely, since $m,n$ are linearly independent, equality to $\nu m-\mu n$ forces both plane equations. Thus neither description introduces extra points.

## 6A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6a/a">a</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/a/solution">Solution</h4>

↑ **Parent:** [A](#6a/a)

The [vector triple product identity](../../../calculus.md#vector-triple-product) gives $n\times(x\times n)=x-(n\cdot x)n$. Decompose $x=x_\perp+x_\parallel$, where $x_\parallel=(n\cdot x)n$ and $x_\perp\cdot n=0$. Then

$$
\Phi(x)=x_\perp+\alpha x_\parallel.
$$

The [linear map](../../../vector-space.md#linear-map) acts as the identity on $n^\perp$ and as multiplication by $\alpha$ along $n$. Consequently **it is invertible exactly when $\alpha\ne0$**, with

$$
\boxed{\Phi^{-1}(y)=y+\left(\alpha^{-1}-1\right)(n\cdot y)n.}
$$

Applying $\Phi$ to this expression recovers the perpendicular and parallel components of $y$ separately.

<h3 id="6a/b">b</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/b/solution">Solution</h4>

↑ **Parent:** [B](#6a/b)

At $\alpha=0$, $\Phi$ is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto the plane perpendicular to $n$. Its [image of a linear map](../../../vector-space.md#image-of-a-linear-map) and [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) are

$$
\boxed{\operatorname{im}\Phi=n^\perp,\qquad \ker\Phi=\operatorname{span}\{n\}.}
$$

Every perpendicular [vector](../../../vector-space.md#vector) is unchanged and every parallel [vector](../../../vector-space.md#vector) is annihilated. The image plane is perpendicular to the kernel axis by the definition of $n^\perp$; their dimensions two and one also agree with the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem).

<h3 id="6a/c">c</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/c/solution">Solution</h4>

↑ **Parent:** [C](#6a/c)

Expanding the formula from part (a) in components gives $y_i=x_i+(\alpha-1)n_i n_jx_j$, with repeated indices summed. Hence the [matrix of a linear map](../../../vector-space.md#matrix-representation-of-a-linear-map) and its inverse, when $\alpha\ne0$, have entries

$$
\boxed{A_{ij}=\delta_{ij}+(\alpha-1)n_i n_j,\qquad
B_{ij}=\delta_{ij}+(\alpha^{-1}-1)n_i n_j.}
$$

Here $\delta_{ij}$ is the [Kronecker delta](../../../linear-algebra.md#kronecker-delta). To check the [matrix inverse](../../../linear-algebra.md#matrix-inverse), write $P=nn^T$; $P^2=P$ because $|n|=1$. Thus $A=(I-P)+\alpha P$ and $B=(I-P)+\alpha^{-1}P$, whose product is the [identity matrix](../../../vector-space.md#identity-matrix).

<h3 id="6a/d">d</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/d/solution">Solution</h4>

↑ **Parent:** [D](#6a/d)

For the specified unit [vector](../../../vector-space.md#vector),

$$
A-C=\frac13\begin{pmatrix}
\alpha&\alpha-3&\alpha\\
\alpha&\alpha&\alpha-3\\
\alpha-3&\alpha&\alpha
\end{pmatrix}.
$$

For a cyclic [matrix](../../../vector-space.md#matrix) with first row $(a,b,c)$, its [determinant](../../../linear-algebra.md#determinant) is $a^3+b^3+c^3-3abc$. Here it gives

$$
\det(A-C)=\frac{2\alpha^3+(\alpha-3)^3-3\alpha^2(\alpha-3)}{27}=\alpha-1.
$$

Therefore $Ax=Cx$ has only the zero solution if $\alpha\ne1$. At $\alpha=1$, $A=I$ and $A-C$ has kernel consisting of the equal-coordinate [vectors](../../../vector-space.md#vector). The complete answer is

$$
\boxed{\alpha\ne1:\ x=0;\qquad \alpha=1:\ x=t(1,1,1),\quad t\in\mathbb R.}
$$

Geometrically, $C^TC=I$, $\det C=1$ and $Cn=n$, so $C$ is a [rotation matrix](../../../linear-algebra.md#rotation-matrix) about the $n$ axis. Its [matrix trace](../../../linear-algebra.md#matrix-trace) is two, giving $\cos\theta=(\operatorname{tr}C-1)/2=1/2$; its skew part selects angle $-\pi/3$ about the oriented axis $n$. It has no fixed nonzero perpendicular [vector](../../../vector-space.md#vector). Meanwhile $A$ preserves perpendicular components and scales the axial component by $\alpha$. Comparing these components first forces $x_\perp=0$, and then $(\alpha-1)x_\parallel=0$, exactly matching the [determinant](../../../linear-algebra.md#determinant) calculation, including the noninvertible case $\alpha=0$.

## 7B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7b/a">a</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/a/solution">Solution</h4>

↑ **Parent:** [A](#7b/a)

Expanding the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) gives

$$
\det(M-tI)=(2-t)\bigl[(1-t)(3-t)+2\bigr]-2(2-t)
=(2-t)(1-t)(3-t).
$$

Thus the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $1,2,3$. Solving the corresponding [homogeneous linear systems](../../../linear-algebra.md#homogeneous-linear-system) gives

$$
\boxed{E_1=\operatorname{span}\{(-1,0,1)^T\},\quad
E_2=\operatorname{span}\{(1,1,0)^T\},\quad
E_3=\operatorname{span}\{(1,1,1)^T\}.}
$$

Every nonzero [vector](../../../vector-space.md#vector) in the displayed [eigenspace](../../../linear-operator-theory.md#eigenspace) is an [eigenvector](../../../linear-operator-theory.md#eigenvector). Direct multiplication verifies the three eigenvalue equations. The distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) imply these [eigenvectors](../../../linear-operator-theory.md#eigenvector) are linearly independent and form a [basis](../../../vector-space.md#basis) of $\mathbb R^3$.

<h3 id="7b/b">b</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/b/solution">Solution</h4>

↑ **Parent:** [B](#7b/b)

The equation is solvable exactly when $b\in\operatorname{im}A$, the [image of a linear map](../../../vector-space.md#image-of-a-linear-map), equivalently when the [rank of a matrix](../../../vector-space.md#matrix-rank) satisfies $\operatorname{rank}A=\operatorname{rank}[A\mid b]$. If it is solvable and $x_0$ is one solution, every solution is precisely

$$
x=x_0+v,\qquad v\in\ker A.
$$

Indeed differences of solutions lie in the [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map), and adding a kernel [vector](../../../vector-space.md#vector) preserves the equation. Hence **there are no solutions** when $b\notin\operatorname{im}A$; **one solution** when $A$ is invertible; and **infinitely many solutions** when $b\in\operatorname{im}A$ and $A$ is singular. In the last case the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) gives a nonzero kernel [vector](../../../vector-space.md#vector) $v$, and $x_0+tv$ gives distinct solutions for every real $t$. This proves that a finite number greater than one is impossible.

<h3 id="7b/c">c</h3>

↑ **Parent:** [7B](#7b)

<h4 id="7b/c/solution">Solution</h4>

↑ **Parent:** [C](#7b/c)

Use the [eigenvector](../../../linear-operator-theory.md#eigenvector) [basis](../../../vector-space.md#basis) $v_1=(-1,0,1)^T$, $v_2=(1,1,0)^T$, $v_3=(1,1,1)^T$. The forcing has decomposition $b=-v_1+3v_3$. If $x=c_1v_1+c_2v_2+c_3v_3$, the [linear system](../../../linear-algebra.md#system-of-linear-equations) reduces to

$$
(1-\lambda)c_1=-1,\qquad(2-\lambda)c_2=0,\qquad(3-\lambda)c_3=3.
$$

For $\lambda=0$, all coefficients are determined, giving

$$
\boxed{x=(2,1,0)^T.}
$$

For $\lambda=1$, the first equation would say $0=-1$, so **there are no solutions**. For $\lambda=2$, $c_1=1$, $c_3=3$, and $c_2$ is arbitrary. Thus **all solutions** are

$$
\boxed{x=(2,3,4)^T+t(1,1,0)^T,\qquad t\in\mathbb R.}
$$

These outcomes illustrate respectively an invertible [matrix](../../../vector-space.md#matrix), incompatible forcing outside its [image of a linear map](../../../vector-space.md#image-of-a-linear-map), and a compatible forcing with a nontrivial [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map).

## 8B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="8b/a">a</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/a/i">i</h4>

↑ **Parent:** [A](#8b/a)

<h5 id="8b/a/i/solution">Solution</h5>

↑ **Parent:** [I](#8b/a/i)

Let $Mv=\lambda v$ with $v\in\mathbb C^n$ nonzero. For a real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix), $M^*=M$, where the star denotes the [conjugate transpose](../../../linear-operator-theory.md#conjugate-transpose). Consequently $v^*Mv$ equals its [complex conjugate](../../../complex-analysis.md#complex-conjugate) and is real. The [eigenvalue equation](../../../linear-operator-theory.md#eigenvalue-equation) gives

$$
\boxed{\lambda=\frac{v^*Mv}{v^*v}\in\mathbb R,}
$$

since $v^*v>0$. Allowing a complex [eigenvector](../../../linear-operator-theory.md#eigenvector) in this argument is essential: reality of an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) must be proved, rather than assumed in advance.

<h4 id="8b/a/ii">ii</h4>

↑ **Parent:** [A](#8b/a)

<h5 id="8b/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8b/a/ii)

Write a complex [eigenvector](../../../linear-operator-theory.md#eigenvector) as $v=u+iw$, where $u,w\in\mathbb R^n$. Since $M$ and its [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$ are real,

$$
Mu=\lambda u,\qquad Mw=\lambda w.
$$

At least one of $u,w$ is nonzero, and it is a real [eigenvector](../../../linear-operator-theory.md#eigenvector) for the same [eigenvalue](../../../linear-operator-theory.md#eigenvalue). More generally every complex [eigenvector](../../../linear-operator-theory.md#eigenvector) is a complex linear combination of real ones: its real and imaginary parts lie in the real [eigenspace](../../../linear-operator-theory.md#eigenspace). Thus **each [eigenspace](../../../linear-operator-theory.md#eigenspace) has a [basis](../../../vector-space.md#basis) chosen over the reals**. The conclusion does not assert that every arbitrary complex [eigenvector](../../../linear-operator-theory.md#eigenvector) is itself real.

<h4 id="8b/a/iii">iii</h4>

↑ **Parent:** [A](#8b/a)

<h5 id="8b/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#8b/a/iii)

Choose real [eigenvectors](../../../linear-operator-theory.md#eigenvector) $u,v$ with distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda,\mu$. Symmetry gives

$$
\lambda u^Tv=(Mu)^Tv=u^TMv=\mu u^Tv.
$$

Therefore $(\lambda-\mu)u^Tv=0$, and **$\boxed{u\cdot v=0}$**. For complex choices, replace transpose by [conjugate transpose](../../../linear-operator-theory.md#conjugate-transpose); the reality proved in part (i) gives the same conclusion for the [Hermitian inner product](../../../linear-algebra.md#hermitian-form). Thus different [eigenspaces](../../../linear-operator-theory.md#eigenspace) are [orthogonal](../../../linear-algebra.md#orthogonal-vectors).

<h3 id="8b/b">b</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/b/solution">Solution</h4>

↑ **Parent:** [B](#8b/b)

For a real [antisymmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix), $A^T=-A$, so $(A^2)^T=A^2$. The previous result makes every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\eta$ of $A^2$ real, with a real nonzero [eigenvector](../../../linear-operator-theory.md#eigenvector) $v$. Moreover,

$$
\eta|v|^2=v^TA^2v=-(Av)^TAv=-|Av|^2\le0.
$$

Thus **every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of $A^2$ is real and nonpositive**.

Take real unit [eigenvectors](../../../linear-operator-theory.md#eigenvector) $u,w$ of $A^2$ for the respective distinct nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $-\lambda^2,-\mu^2$, where the real parameters $\lambda,\mu$ are nonzero. Define

$$
u'=\frac{Au}{\lambda},\qquad w'=\frac{Aw}{\mu}.
$$

The displayed quadratic identity gives $|u'|=|w'|=1$. Also $u\cdot Au=0$ and $w\cdot Aw=0$, because a real [antisymmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix) has zero [quadratic form](../../../linear-algebra.md#quadratic-form). Thus $u\perp u'$ and $w\perp w'$. Since $A$ commutes with $A^2$, $u'$ lies in the same [eigenspace](../../../linear-operator-theory.md#eigenspace) of $A^2$ as $u$, and $w'$ in the same one as $w$. Distinct [eigenspaces](../../../linear-operator-theory.md#eigenspace) of the real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) $A^2$ are [orthogonal](../../../linear-algebra.md#orthogonal-vectors), so all four [vectors](../../../vector-space.md#vector) are [orthonormal](../../../linear-algebra.md#orthonormal-set). Finally,

$$
\boxed{Au=\lambda u',\quad Au'=-\lambda u,\qquad
Aw=\mu w',\quad Aw'=-\mu w.}
$$

Thus on each of the two perpendicular planes, $A$ acts as a scaled quarter-turn. This constructs the required [vectors](../../../vector-space.md#vector), rather than merely counting dimensions.

## 9F

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="9f/a">a</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/a/solution">Solution</h4>

↑ **Parent:** [A](#9f/a)

For a positive-term [series](../../../real-analysis.md#series-mathematics), the [ratio test](../../../real-analysis.md#ratio-test) says that if $a_{n+1}/a_n\to L<1$, the series converges; if the ratio tends to $L>1$, including positive infinity, it diverges. More generally $\limsup a_{n+1}/a_n<1$ suffices for convergence and $\liminf a_{n+1}/a_n>1$ for divergence. **A limiting ratio of one gives no conclusion.**

The [P-series](../../../real-analysis.md#p-series) $\sum n^{-2}$ converges and the [harmonic series](../../../real-analysis.md#harmonic-series) $\sum n^{-1}$ diverges. Both have strictly decreasing positive terms, and their successive ratios, $(n/(n+1))^2$ and $n/(n+1)$, tend to one. These supply the two requested possibilities.

<h3 id="9f/b">b</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/b/solution">Solution</h4>

↑ **Parent:** [B](#9f/b)

The [function](../../../function.md) $1/x$ is decreasing and positive. Therefore on $[k,k+1]$ it is at most $1/k$, and the [Riemann integral](../../../real-analysis.md#riemann-integral) gives

$$
\int_k^{k+1}\frac{dx}{x}\le\frac1k.
$$

Summing from $k=1$ to $n-1$ yields

$$
\boxed{\log n=\int_1^n\frac{dx}{x}\le\sum_{k=1}^{n-1}\frac1k.}
$$

For $n=1$ both sides are zero; for $n>1$ the inequality is actually strict. The same [integral test for convergence](../../../real-analysis.md#integral-test-for-convergence) gives $\sum_{k=N}^{n-1}1/k\ge\log(n/N)$.

<h3 id="9f/c">c</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/c/solution">Solution</h4>

↑ **Parent:** [C](#9f/c)

First, for $0<x<1$, the [derivative](../../../calculus.md#derivative) of $h(x)=\log(1-x)+x$ is $-x/(1-x)<0$, while $h(0)=0$. Hence $\log(1-x)<-x$.

Choose $N>c$ large enough that the given ratio bound holds for every $n\ge N$. Positivity permits taking [logarithms](../../../calculus.md#logarithm), and the preceding inequality gives

$$
\log a_{k+1}-\log a_k\le\log(1-c/k)<-c/k.
$$

Summing, and using the [integral test for convergence](../../../real-analysis.md#integral-test-for-convergence) from part (b), gives for $n>N$

$$
\log a_n\le\log a_N-c\sum_{k=N}^{n-1}\frac1k
\le\log a_N-c\log(n/N).
$$

Thus $a_n\le a_NN^c n^{-c}$. Since $c>1$, the [P-series](../../../real-analysis.md#p-series) $\sum n^{-c}$ converges, so the [comparison test for series](../../../real-analysis.md#comparison-test-for-series) proves

$$
\boxed{\sum_{n=1}^\infty a_n<\infty.}
$$

The finitely many initial terms do not affect convergence. This [power-law comparison from a refined ratio bound](../../../real-analysis.md#power-law-comparison-from-a-refined-ratio-bound) supplies information when the ordinary [ratio test](../../../real-analysis.md#ratio-test) can be inconclusive.

## 10E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="10e/solution">Solution</h3>

↑ **Parent:** [10E](#10e)

The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) states that if $f:[a,b]\to\mathbb R$ is [continuous](../../../calculus.md#continuous-function), then every real value between $f(a)$ and $f(b)$ is attained at some $c\in[a,b]$. Here is a proof using [completeness of the real numbers](../../../real-analysis.md#completeness-of-the-real-numbers). Endpoint values are immediate, so suppose $f(a)<y<f(b)$; reversing the sign of $f$ handles the other ordering. Let

$$
S=\{x\in[a,b]:f(x)<y\},\qquad c=\sup S.
$$

The set is nonempty and bounded above. [Continuity](../../../calculus.md#continuous-function) at $a$ puts points to the right of $a$ in $S$, while [continuity](../../../calculus.md#continuous-function) at $b$ excludes an entire interval to the left of $b$, so $a<c<b$. If $f(c)<y$, [continuity](../../../calculus.md#continuous-function) puts some point larger than $c$ in $S$, contradicting its [supremum](../../../real-analysis.md#supremum). If $f(c)>y$, [continuity](../../../calculus.md#continuous-function) excludes $S$ in a neighborhood of $c$, contradicting the existence of points of $S$ arbitrarily close to its [supremum](../../../real-analysis.md#supremum) from below. Therefore $f(c)=y$, proving the theorem.

For the fixed-point assertion, put $g(x)=f(x)-x$. This is [continuous](../../../calculus.md#continuous-function), with $g(0)=f(0)\ge0$ and $g(1)=f(1)-1\le0$. If either endpoint value is zero it already gives a [fixed point](../../../function.md#fixed-point); otherwise the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) gives an interior zero. Hence

$$
\boxed{\text{Every continuous self-map of }[0,1]\text{ has a fixed point.}}
$$

The proof needs both [continuity](../../../calculus.md#continuous-function) and the closed-interval endpoint information; the following counterexamples separate those hypotheses.

<h3 id="10e/i">i</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/i/solution">Solution</h4>

↑ **Parent:** [I](#10e/i)

**No.** The [continuous function](../../../calculus.md#continuous-function) $f(x)=(x+1)/2$ maps $(0,1)$ into $(0,1)$, but $f(x)-x=(1-x)/2>0$ throughout the domain. Its only possible [fixed point](../../../function.md#fixed-point) is the excluded endpoint one.

<h3 id="10e/ii">ii</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10e/ii)

**No.** The [continuous function](../../../calculus.md#continuous-function) $f(x)=x+1$ is a self-map of $\mathbb R$, but the [fixed point](../../../function.md#fixed-point) equation would require $x+1=x$, which is impossible.

<h3 id="10e/iii">iii</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#10e/iii)

**No.** Define $f(x)=1$ for $0\le x<1$ and $f(1)=0$. This self-map of $[0,1]$ is discontinuous at one. Every point smaller than one is sent to a different point, and one is sent to zero, so it has no [fixed point](../../../function.md#fixed-point).

<h3 id="10e/iv">iv</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#10e/iv)

**Yes: a tangential zero and a crossing zero can give exactly two [fixed points](../../../function.md#fixed-point).** One explicit [continuous](../../../calculus.md#continuous-function) piecewise linear example is

$$
\boxed{f(x)=\begin{cases}
1-2x,&0\le x\le1/3,\\
\frac52x-\frac12,&1/3\le x\le1/2,\\
1-\frac12x,&1/2\le x\le2/3,\\
2-2x,&2/3\le x\le1.
\end{cases}}
$$

Adjacent formulas agree at each junction. Their endpoint values lie in $[0,1]$, so linear interpolation proves that the whole image lies in $[0,1]$; also $f(0)=1$ and $f(1)=0$. On the four pieces, $f(x)-x$ is respectively $1-3x$, $3x/2-1/2$, $1-3x/2$, and $2-3x$. Their only zeros on their respective intervals are $1/3$ and $2/3$. Thus **the complete [fixed point](../../../function.md#fixed-point) set is $\boxed{\{1/3,2/3\}}$**. Continuity forces at least one zero, but does not force every zero to change sign.

## 11E

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="11e/solution">Solution</h3>

↑ **Parent:** [11E](#11e)

For the first additional construction, modify the rational/irrational example to

$$
\boxed{g(x)=\begin{cases}x^2,&x\in\mathbb Q,\\-x^2,&x\notin\mathbb Q.\end{cases}}
$$

At zero, $|g(h)/h|=|h|\to0$, so $g'(0)=0$. At any nonzero point, [density of the rational numbers](../../../number-theory.md#density-of-the-rational-numbers) and [density of the irrational numbers](../../../algebra.md#density-of-the-irrational-numbers) give incompatible limiting values $x^2$ and $-x^2$. Thus $g$ is discontinuous, and hence not [differentiable](../../../analysis.md#differentiable-function), there. **Its [differentiability](../../../analysis.md#differentiability) set is exactly $\{0\}$.**

For the second construction, use a [summable absolute-value cusp series](../../../real-analysis.md#summable-absolute-value-cusp-series):

$$
\boxed{G(x)=\sum_{n=2}^\infty2^{-n}\left|x-\frac1n\right|.}
$$

On $[-R,R]$, each summand is bounded by $2^{-n}(R+1/2)$. The [Weierstrass M-test](../../../probability-and-statistics.md#weierstrass-m-test) therefore gives [uniform convergence](../../../real-analysis.md#uniform-convergence) on every bounded interval, and the [uniform limit theorem](../../../real-analysis.md#uniform-limit-theorem) makes $G$ [continuous](../../../calculus.md#continuous-function) everywhere.

To justify [differentiability](../../../analysis.md#differentiability), each summand's [difference quotient](../../../calculus.md#difference-quotient) has absolute value at most $2^{-n}$, by the [reverse triangle inequality](../../../topological-analysis.md#reverse-triangle-inequality). The sum of these bounds is finite, uniformly in the increment. Thus the tail of the [difference quotient](../../../calculus.md#difference-quotient) is uniformly small, and limits may be passed through the sum by first retaining finitely many terms and then making the tail small. If $x\ne1/n$ for every $n\ge2$, each individual summand is [differentiable](../../../analysis.md#differentiable-function), giving

$$
G'(x)=\sum_{n=2}^\infty2^{-n}\operatorname{sgn}(x-1/n).
$$

In particular **$G'(0)=-\sum_{n=2}^\infty2^{-n}=-1/2$**. The accumulation of cusp locations at zero does not destroy the [derivative](../../../calculus.md#derivative), because their weights are summable.

At $x=1/m$, the same tail argument applies to both one-sided [derivatives](../../../calculus.md#derivative). Every term except the $m$th has the same derivative from both sides; the $m$th has derivatives $-2^{-m}$ and $2^{-m}$. Consequently

$$
G'_+(1/m)-G'_-(1/m)=2^{1-m}>0.
$$

Therefore **$G$ fails to be [differentiable](../../../analysis.md#differentiable-function) exactly at $1/2,1/3,1/4,\ldots$, and is [differentiable](../../../analysis.md#differentiable-function) everywhere else**.

<h3 id="11e/i">i</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/i/solution">Solution</h4>

↑ **Parent:** [I](#11e/i)

At zero, $|f(x)-f(0)|=|x|\to0$, so the [function](../../../function.md) is [continuous](../../../calculus.md#continuous-function). At a nonzero $x_0$, approach along rational and irrational [sequences](../../../real-analysis.md#sequence); [density of the rational numbers](../../../number-theory.md#density-of-the-rational-numbers) and [density of the irrational numbers](../../../algebra.md#density-of-the-irrational-numbers) give limiting values $x_0$ and $-x_0$, which are different. Thus the **[continuity](../../../calculus.md#continuous-function) set is $\boxed{\{0\}}$**.

At zero, the [difference quotient](../../../calculus.md#difference-quotient) is one for rational nonzero increments and minus one for irrational increments, so the [derivative](../../../calculus.md#derivative) does not exist. Elsewhere [differentiability implies continuity](../../../analysis.md#differentiability-implies-continuity), and continuity already fails. Thus the **[differentiability](../../../analysis.md#differentiability) set is $\boxed{\varnothing}$**.

<h3 id="11e/ii">ii</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11e/ii)

Away from zero, the product and composition of the displayed smooth [functions](../../../function.md) are [continuous](../../../calculus.md#continuous-function) and [differentiable](../../../analysis.md#differentiable-function). At zero,

$$
|f(x)|\le|x|\longrightarrow0,
$$

so $f$ remains [continuous](../../../calculus.md#continuous-function). Hence the **[continuity](../../../calculus.md#continuous-function) set is $\boxed{\mathbb R}$**.

The [difference quotient](../../../calculus.md#difference-quotient) at zero is $f(h)/h=\sin(1/h)$. For $h_n=(\pi/2+2\pi n)^{-1}$ it equals one, and for $k_n=(3\pi/2+2\pi n)^{-1}$ it equals minus one. Both [sequences](../../../real-analysis.md#sequence) tend to zero, so no [derivative](../../../calculus.md#derivative) exists there. For $x\ne0$, the [product rule](../../../calculus.md#product-rule) and [chain rule](../../../calculus.md#chain-rule) give

$$
\boxed{f'(x)=\sin(1/x)-\frac{\cos(1/x)}x.}
$$

Thus the **[differentiability](../../../analysis.md#differentiability) set is $\boxed{\mathbb R\setminus\{0\}}$**.

## 12D

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="12d/solution">Solution</h3>

↑ **Parent:** [12D](#12d)

The [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) connects the [Riemann integral](../../../real-analysis.md#riemann-integral) with [differentiation](../../../calculus.md#differentiation). Its first part says that for [continuous](../../../calculus.md#continuous-function) $h:[a,b]\to\mathbb R$, the accumulation function $H(x)=\int_a^xh(t)\,dt$ is [continuous](../../../calculus.md#continuous-function) on $[a,b]$ and [differentiable](../../../analysis.md#differentiable-function) inside it, with

$$
\boxed{H'(x)=h(x).}
$$

To prove this, boundedness of $h$ gives $|H(y)-H(x)|\le\|h\|_\infty|y-x|$, proving [continuity](../../../calculus.md#continuous-function). For an interior point and a sufficiently small nonzero increment $u$,

$$
\frac{H(x+u)-H(x)}u-h(x)
=\frac1u\int_x^{x+u}(h(t)-h(x))\,dt.
$$

Its absolute value is at most $\sup_{|t-x|\le|u|}|h(t)-h(x)|$, which tends to zero by [continuity](../../../calculus.md#continuous-function) of $h$ at $x$. This proves the [derivative](../../../calculus.md#derivative) formula. The same estimate gives the appropriate one-sided endpoint [derivatives](../../../calculus.md#derivative).

The second part says that if $Q$ is [continuous](../../../calculus.md#continuous-function) on $[a,b]$, [differentiable](../../../analysis.md#differentiable-function) on $(a,b)$, and $Q'=h$ with $h$ [continuous](../../../calculus.md#continuous-function), then

$$
\boxed{\int_a^b h(t)\,dt=Q(b)-Q(a).}
$$

Indeed $(Q-H)'=0$, so the [mean value theorem](../../../calculus.md#mean-value-theorem) makes $Q-H$ constant, and evaluating at the endpoints proves the formula. A useful stronger version only requires $Q'$ to be [Riemann integrable](../../../real-analysis.md#riemann-integrable-function). For a partition $a=x_0<\cdots<x_N=b$, the [mean value theorem](../../../calculus.md#mean-value-theorem) on each subinterval provides $\xi_j\in(x_{j-1},x_j)$ such that

$$
Q(b)-Q(a)=\sum_{j=1}^NQ'(\xi_j)(x_j-x_{j-1}).
$$

As the mesh tends to zero, these tagged [Riemann sums](../../../real-analysis.md#riemann-sum) converge to $\int_a^b Q'$, proving that version too. Its integrability hypothesis must not be omitted.

**An integrable integrand need not give an everywhere [differentiable](../../../analysis.md#differentiable-function) accumulation function.** For a counterexample, let $f(t)=0$ for $t<1/2$ and $f(t)=1$ for $t\ge1/2$. This bounded step [function](../../../function.md) is [Riemann integrable](../../../real-analysis.md#riemann-integrable-function), but

$$
F(x)=\int_0^xf(t)\,dt=\begin{cases}0,&x\le1/2,\\x-1/2,&x\ge1/2.
\end{cases}
$$

Its left and right [derivatives](../../../calculus.md#derivative) at $1/2$ are zero and one. Thus **$F$ need not be [differentiable](../../../analysis.md#differentiable-function) at every interior point**. The first part of the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) does apply at every point where the integrand is [continuous](../../../calculus.md#continuous-function).

**A [derivative](../../../calculus.md#derivative) need not have a [Riemann integral](../../../real-analysis.md#riemann-integral).** Define on all of $\mathbb R$

$$
f(x)=\begin{cases}x^2\sin(1/x^2),&x\ne0,\\0,&x=0.
\end{cases}
$$

At zero $f(h)/h=h\sin(1/h^2)\to0$, so $f'(0)=0$; elsewhere the [product rule](../../../calculus.md#product-rule) and [chain rule](../../../calculus.md#chain-rule) give

$$
f'(x)=2x\sin(1/x^2)-\frac2x\cos(1/x^2).
$$

At $x_n=(2\pi n)^{-1/2}$, this equals $-2/x_n\to-\infty$. Hence $f'$ is unbounded on $[0,1]$, whereas a properly [Riemann integrable](../../../real-analysis.md#riemann-integrable-function) [function](../../../function.md) on a compact interval must be bounded. The requested [Riemann integral](../../../real-analysis.md#riemann-integral) therefore **need not exist**, even though $f$ is [differentiable](../../../analysis.md#differentiable-function) everywhere. This example is an [unbounded derivative obstruction to Riemann integrability](../../../real-analysis.md#unbounded-derivative-obstruction-to-riemann-integrability); it does not contradict the theorem's version that explicitly assumes integrability of the derivative.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2011](../../2011.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
