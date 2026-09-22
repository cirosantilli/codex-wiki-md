# Paper 339

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_339.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_339.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
    - [iv](#2/c/iv)
      - [Solution](#2/c/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 339](paper-339.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Suppose $y$ in the [capped simplex](../../../mathematical-optimization.md#capped-simplex) has a coordinate strictly between zero and one. Since $\sum_i y_i=k$ is an integer, it cannot have exactly one such coordinate: the other coordinates would contribute an integer sum. Hence there are distinct $i,j$ with $0<y_i,y_j<1$.

Choose $0<\varepsilon<\min\{y_i,1-y_i,y_j,1-y_j\}$ and set $y^{\pm}=y\pm\varepsilon(e_i-e_j)$, where $e_i,e_j$ are [standard basis](../../../vector-space.md#standard-basis) vectors. Both perturbed [vectors](../../../vector-space.md#vector) satisfy the coordinate bounds and have the same coordinate sum. They are distinct and $y=(y^++y^-)/2$, so $y$ is not an [extreme point](../../../mathematical-optimization.md#extreme-point).

Conversely, every zero-one [vector](../../../vector-space.md#vector) in this [convex polytope](../../../mathematical-optimization.md#convex-polytope) is an [extreme point](../../../mathematical-optimization.md#extreme-point). If it were a nontrivial [convex combination](../../../mathematical-optimization.md#convex-combination) of two feasible [vectors](../../../vector-space.md#vector), each coordinate equal to zero would force both corresponding coordinates to be zero, and each coordinate equal to one would force both to be one. Thus the two [vectors](../../../vector-space.md#vector) would equal the original one. The [extreme points](../../../mathematical-optimization.md#extreme-point) are therefore exactly the indicators of $k$-element subsets.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The required [linear program](../../../mathematical-optimization.md#linear-programming) is

$$
\boxed{f_k(x)=\max_{y\in\mathbb R^n}\left\{x^Ty:y_i\geq0,\ y_i\leq1\ (1\leq i\leq n),\ \sum_i y_i=k\right\}.}
$$

There are $2n$ inequality constraints and one equality constraint, all independent of $x$.

The feasible set is the [capped simplex](../../../mathematical-optimization.md#capped-simplex), a nonempty [compact set](../../../topology.md#compact-space). A [linear function](../../../vector-space.md#linear-function) attains its maximum at an [extreme point](../../../mathematical-optimization.md#extreme-point); the previous part identifies these as the indicators of $k$-element subsets. At such a [vector](../../../vector-space.md#vector), the objective is the sum of the selected coordinates. Maximizing selects the $k$ largest coordinates, including when some are negative or tied. Equivalently, $f_k$ is the [support function](../../../mathematical-optimization.md#support-function) called the [sum of the largest components](../../../mathematical-optimization.md#sum-of-the-largest-components).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Keep $y\geq0$ as the domain restriction, introduce nonnegative [Lagrange multipliers](../../../mathematical-optimization.md#lagrange-multiplier) $s_i$ for $y_i\leq1$, and introduce a free multiplier $t\in\mathbb R$ for $\sum_i y_i=k$. The maximizing [Lagrangian](../../../calculus-of-variations.md#lagrangian) is

$$
L(y,s,t)=x^Ty+s^T(\mathbf1-y)+t(k-\mathbf1^Ty)
=\mathbf1^Ts+kt+(x-s-t\mathbf1)^Ty.
$$

Its supremum over $y\geq0$ is finite exactly when $s+t\mathbf1\geq x$, and then equals $kt+\sum_i s_i$. By [linear programming duality](../../../mathematical-optimization.md#linear-programming-duality), since the primal is feasible and bounded,

$$
\boxed{f_k(x)=\min_{t\in\mathbb R,\ s\in\mathbb R^n}\left\{kt+\sum_i s_i:s_i\geq0,\ s_i+t\geq x_i\right\}.}
$$

Minimizing over $s$ for fixed $t$ gives $s_i=(x_i-t)_+$, the [positive part of a real-valued function](../../../function.md#positive-part-of-a-real-valued-function). Thus the [threshold formula for the sum of the largest components](../../../mathematical-optimization.md#threshold-formula-for-the-sum-of-the-largest-components) is

$$
\boxed{f_k(x)=\min_{t\in\mathbb R}\left[kt+\sum_i(x_i-t)_+\right].}
$$

For a direct attainment check, order the coordinates $x_{[1]}\geq\cdots\geq x_{[n]}$. Any $t\in[x_{[k+1]},x_{[k]}]$ is optimal for $k<n$, while any $t\leq x_{[n]}$ is optimal for $k=n$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Substitute the [dual linear program](../../../mathematical-optimization.md#dual-linear-program) from the previous part and optimize jointly over $x,t,s$. The result is

$$
\boxed{
\begin{aligned}
\operatorname{minimize}\quad&kt+\sum_{i=1}^n s_i\\
\text{over}\quad&x\in\mathbb R^n,\ t\in\mathbb R,\ s\in\mathbb R^n\\
\text{subject to}\quad&Ax=b,\\
&s_i\geq0,\quad s_i+t\geq x_i\quad(1\leq i\leq n).
\end{aligned}}
$$

The objective is linear, and the constraints are equalities or inequalities between [affine functions](../../../vector-space.md#affine-function), so this is a [linear program](../../../mathematical-optimization.md#linear-programming). For each fixed feasible $x$, minimizing over $t,s$ gives exactly $f_k(x)$ by the [threshold formula for the sum of the largest components](../../../mathematical-optimization.md#threshold-formula-for-the-sum-of-the-largest-components); hence the reformulation preserves the optimal value and optimal $x$ whenever an optimum exists.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Replace coordinate inequalities by the [Loewner order](../../../linear-algebra.md#loewner-order) and coordinate sums by [matrix trace](../../../linear-algebra.md#matrix-trace). The maximizing [semidefinite program](../../../convex-optimization.md#semidefinite-programming) is

$$
\boxed{F_k(X)=\max_{Y\in\mathbb S^n}\{\operatorname{tr}(XY):Y\succeq0,\ I-Y\succeq0,\ \operatorname{tr}Y=k\}.}
$$

Its feasible set is the [fantope](../../../mathematical-optimization.md#fantope). In an [orthonormal eigenbasis](../../../linear-operator-theory.md#orthonormal-eigenbasis) of $X$, its objective is $\sum_i\lambda_i(X)Y_{ii}$, and the diagonal entries of $Y$ belong to the [capped simplex](../../../mathematical-optimization.md#capped-simplex). Choosing $Y$ as the [orthogonal projection matrix](../../../linear-algebra.md#orthogonal-projection-matrix) onto the largest $k$ [eigenvectors](../../../linear-operator-theory.md#eigenvector) attains the [sum of the largest eigenvalues](../../../mathematical-optimization.md#sum-of-the-largest-eigenvalues), as in the [Ky Fan maximum principle](../../../mathematical-optimization.md#ky-fan-maximum-principle).

The minimizing [semidefinite program](../../../convex-optimization.md#semidefinite-programming) is

$$
\boxed{F_k(X)=\min_{t\in\mathbb R,\ S\in\mathbb S^n}\{kt+\operatorname{tr}S:S\succeq0,\ S+tI-X\succeq0\}.}
$$

For example, its [Lagrangian](../../../calculus-of-variations.md#lagrangian) arises by assigning $S\succeq0$ to $I-Y\succeq0$, keeping $Y\succeq0$ in the domain, and using free $t$ for $\operatorname{tr}Y=k$. Finiteness of the supremum over $Y$ requires $S+tI-X\succeq0$.

Equality follows directly by choosing $S$ to have [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $(\lambda_i(X)-t)_+$ in the same [orthonormal eigenbasis](../../../linear-operator-theory.md#orthonormal-eigenbasis), with $t$ between the $k$th and $(k+1)$st [eigenvalues](../../../linear-operator-theory.md#eigenvalue), or below the smallest one for $k=n$. This is the [threshold semidefinite program for the largest eigenvalues](../../../mathematical-optimization.md#threshold-semidefinite-program-for-the-largest-eigenvalues), and it also verifies the endpoint case $k=n$.

## 2

↑ **Parent:** [Paper 339](paper-339.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $J=\mathbf1\mathbf1^T$ be the [all-ones matrix](../../../vector-space.md#all-ones-matrix). Every feasible block [matrix](../../../vector-space.md#matrix) in the first formulation has $t\geq1$, because its principal $2\times2$ [submatrix](../../../vector-space.md#submatrix) on indices $0,i$ is $\begin{pmatrix}t&1\\1&1\end{pmatrix}$ and is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix). In particular, $t>0$.

By the [Schur complement](../../../linear-algebra.md#schur-complement),

$$
\begin{pmatrix}t&\mathbf1^T\\\mathbf1&Z\end{pmatrix}\succeq0
\quad\Longleftrightarrow\quad
Z-\frac1tJ\succeq0.
$$

Set $U=tZ-J$. Then $U\succeq0$, $U_{ii}=t-1$, and $U_{ij}=-1$ on every [edge](../../../graph-theory.md#edge-of-a-graph). Conversely, for a feasible $(t,U)$ in the second formulation, its nonnegative diagonal gives $t\geq1$, and $Z=(U+J)/t$ has $Z_{ii}=1$, $Z_{ij}=0$ on [edges](../../../graph-theory.md#edge-of-a-graph), and $Z-J/t=U/t\succeq0$.

Both transformations preserve the objective $t$. Hence the two [semidefinite programs](../../../convex-optimization.md#semidefinite-programming) defining the [complement theta number](../../../graph-theory.md#complement-theta-number) have the same feasible objective values and the same minimum.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For a proper three-[graph colouring](../../../graph-theory.md#graph-coloring) $c$, associate the colors with the three [roots of unity](../../../algebra.md#root-of-unity) $d(i)=\exp(2\pi i(c(i)-1)/3)$, viewed as [unit vectors](../../../vector-space.md#unit-vector) in $\mathbb R^2$. Define $U_{ij}=2\langle d(i),d(j)\rangle$ using the real [inner product](../../../linear-algebra.md#inner-product).

This is twice a [Gram matrix](../../../linear-algebra.md#gram-matrix), so it is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix). Its diagonal is $2$. On every [edge](../../../graph-theory.md#edge-of-a-graph), the endpoint colors differ, so their [vectors](../../../vector-space.md#vector) make angle $2\pi/3$ or $4\pi/3$ and $U_{ij}=2\cos(2\pi/3)=-1$. Thus $t=3$ and this $U$ are feasible in the second [semidefinite program](../../../convex-optimization.md#semidefinite-programming), proving

$$
\boxed{\bar\vartheta(G)\leq3.}
$$

This is the [regular simplex](../../../algebraic-topology.md#regular-simplex) construction of a [strict vector coloring](../../../graph-theory.md#strict-vector-coloring).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

For an [edge](../../../graph-theory.md#edge-of-a-graph) $ij$, put $\rho=\langle v_i,v_j\rangle$ and $\theta=\arccos\rho$. Since $\rho\leq-1/2$, we have $\theta\geq2\pi/3$.

The random normal $a$ has the isotropic [Gaussian distribution](../../../probability-theory.md#normal-distribution) $N(0,I_p)$. Its distribution is invariant under [orthogonal transformations](../../../linear-algebra.md#orthogonal-transformation); if $v_i,v_j$ are linearly independent, its projection onto their [plane](../../../geometry-and-topology.md#plane) has a uniformly distributed direction. The signs of its [inner products](../../../linear-algebra.md#inner-product) with $v_i,v_j$ differ in two sectors of total angle $2\theta$, out of $2\pi$. Thus [random hyperplane rounding](../../../graph-theory.md#random-hyperplane-rounding) gives

$$
\boxed{\mathbb P(H\text{ cuts }ij)=\frac{\theta}{\pi}\geq\frac23.}
$$

If $v_j=-v_i$, the signs differ with probability one and the same formula holds with $\theta=\pi$. Zero [inner products](../../../linear-algebra.md#inner-product) have probability zero, since each $v_i$ is a [unit vector](../../../vector-space.md#unit-vector).

If the [graph](../../../graph.md) has an [edge](../../../graph-theory.md#edge-of-a-graph), its corresponding principal $2\times2$ block of $U$ forces $t\geq2$, so the division by $t-1$ used to obtain the [Gram matrix](../../../linear-algebra.md#gram-matrix) is valid. An edgeless [graph](../../../graph.md) can instead be colored with one color directly.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

A fixed [edge](../../../graph-theory.md#edge-of-a-graph) is monochromatic exactly when none of the $r$ hyperplanes separates its endpoints. Each hyperplane fails to cut it with probability at most $1/3$, and the hyperplanes are independent. Therefore

$$
\mathbb P\{c(i)=c(j)\}\leq3^{-r}.
$$

Let $B=\sum_{ij\in E}\mathbf1_{\{c(i)=c(j)\}}$ count monochromatic [edges](../../../graph-theory.md#edge-of-a-graph). Applying [linearity of expectation](../../../probability-theory.md#linearity-of-expectation) to these [indicator random variables](../../../probability-theory.md#indicator-random-variable) gives

$$
\boxed{\mathbb E B\leq m3^{-r}.}
$$

Independence between different [edges](../../../graph-theory.md#edge-of-a-graph) is unnecessary; only the independently sampled hyperplanes are used. The $r$ signs provide at most $2^r$ colors, whether or not every sign region is nonempty.

<h4 id="2/c/iv">iv</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/c/iv)

If $m=0$, use a single color. Otherwise choose

$$
r=\max\left\{0,\left\lceil\log_3\frac{4m}{n}\right\rceil\right\}.
$$

The previous bound gives $\mathbb E B\leq n/4$, including the case $r=0$. By [Markov inequality](../../../probability-inequality.md#markov-inequality), $\mathbb P(B>n/2)\leq1/2$. Sample the hyperplanes, count the monochromatic [edges](../../../graph-theory.md#edge-of-a-graph), and repeat if $B>n/2$. The success probability is at least $1/2$, so at most two draws are needed on average.

For a successful draw, select one endpoint of each monochromatic [edge](../../../graph-theory.md#edge-of-a-graph) and let $D$ be the union of the selected [vertices](../../../graph.md#vertex-graph-theory). Then $|D|\leq B\leq n/2$. Every monochromatic [edge](../../../graph-theory.md#edge-of-a-graph) meets $D$, so the original colors give a proper [graph colouring](../../../graph-theory.md#graph-coloring) on the [induced subgraph](../../../graph-theory.md#induced-subgraph) with vertex set $W=V\setminus D$. Since $|W|\geq n/2$, the coloring of all [vertices](../../../graph.md#vertex-graph-theory) is a [semicoloring](../../../graph-theory.md#semicoloring). This is a [random alteration method](../../../probabilistic-combinatorics.md#random-alteration-method); no additional colors for $D$ are required.

The number of available colors satisfies $2^r\leq2\max\{1,(4m/n)^{\log_3 2}\}$. A simple [graph](../../../graph.md) has $m\leq n(n-1)/2$, hence [semicoloring by independent hyperplanes](../../../graph-theory.md#semicoloring-by-independent-hyperplanes) gives

$$
\boxed{k=O(n^\gamma),\qquad\gamma=\log_3 2=\frac{\log2}{\log3}\approx0.63093<1.}
$$

## 3

↑ **Parent:** [Paper 339](paper-339.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For $z\in\mathbb R^n$, define $x_i=z_i^2$. Then $x$ lies in the [nonnegative orthant](../../../mathematical-optimization.md#nonnegative-orthant) and

$$
p(z)=\sum_{i,j}A_{ij}z_i^2z_j^2=x^TAx.
$$

If $A$ is a [copositive matrix](../../../linear-algebra.md#copositive-matrix), this is nonnegative for every $z$, so $p$ is a globally [nonnegative polynomial](../../../polynomial.md#nonnegative-polynomial). Conversely, every $x\geq0$ has the form $x_i=z_i^2$ by taking $z_i=\sqrt{x_i}$. If $p$ is globally nonnegative, then $x^TAx=p(z)\geq0$ for every such $x$, proving that $A$ is a [copositive matrix](../../../linear-algebra.md#copositive-matrix). The map $z\mapsto(z_i^2)_i$ covers the entire [nonnegative orthant](../../../mathematical-optimization.md#nonnegative-orthant), which is the key to both directions.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

First suppose $A=P+N$, with $P$ a real [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix) and $N$ a symmetric [nonnegative matrix](../../../vector-space.md#nonnegative-matrix). Factor $P=B^TB$, and write $v(z)=(z_1^2,\ldots,z_n^2)^T$. Then

$$
p(z)=\|Bv(z)\|^2+\sum_i N_{ii}(z_i^2)^2+\sum_{i<j}2N_{ij}(z_iz_j)^2.
$$

Each term is a square multiplied by a nonnegative scalar, so $p$ is a [sum of squares polynomial](../../../polynomial.md#polynomial-sos).

Conversely, suppose $p=\sum_\ell q_\ell^2$. Because $p$ is a degree-four [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial), the [homogeneous sum of squares representation](../../../polynomial.md#homogeneous-sum-of-squares-representation) allows every $q_\ell$ to be quadratic and homogeneous. Explicitly, higher-degree parts cannot cancel in a sum of squares; constant parts vanish because $p(0)=0$, and the degree-two part $\sum_\ell(q_\ell^{(1)})^2$ forces all linear parts to vanish. Write

$$
q_\ell(z)=\sum_i a_{\ell i}z_i^2+\sum_{i<j}b_{\ell ij}z_iz_j.
$$

Since $p$ is invariant under every coordinate sign change, [sign averaging of a sum of squares](../../../polynomial.md#sign-averaging-of-a-sum-of-squares) over independent [Rademacher random variables](../../../probability-theory.md#rademacher-distribution) gives

$$
p(z)=\sum_\ell\left(\sum_i a_{\ell i}z_i^2\right)^2
+\sum_{i<j}\left(\sum_\ell b_{\ell ij}^2\right)z_i^2z_j^2.
$$

The cross terms vanish because their sign products contain an [odd](../../../calculus.md#odd-function) power of at least one independent sign. Set

$$
P=\sum_\ell a_\ell a_\ell^T,\qquad N_{ii}=0,\qquad N_{ij}=N_{ji}=\frac12\sum_\ell b_{\ell ij}^2\quad(i<j).
$$

Then $P$ is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix) and $N$ is a symmetric [nonnegative matrix](../../../vector-space.md#nonnegative-matrix). Comparing the coefficients of $z_i^4$ and $z_i^2z_j^2$ gives $A=P+N$. This proves the [sum of squares criterion for a biquadratic form](../../../polynomial.md#sum-of-squares-criterion-for-a-biquadratic-form).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [Horn copositive matrix](../../../linear-algebra.md#horn-copositive-matrix) is invariant under cyclic permutation of its five coordinates: its negative entries correspond precisely to neighboring indices on the five-cycle. For any $x\geq0$, cyclically relabel the coordinates so that $x_5$ is a smallest coordinate. In particular, $x_4-x_5\geq0$.

Using the stated identity in this coordinate order,

$$
x^THx=(x_1-x_2+x_3-x_4+x_5)^2+4x_2x_5+4x_1(x_4-x_5)\geq0.
$$

The square is nonnegative, and both remaining terms are nonnegative since $x_i\geq0$ and $x_4\geq x_5$. Cyclic invariance means the relabeling has not changed the [quadratic form](../../../linear-algebra.md#quadratic-form). Thus $H$ is a [copositive matrix](../../../linear-algebra.md#copositive-matrix) for every original ordering of $x$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $w=(1,2,1,0,0)^T$. Direct multiplication gives $Hw=(0,0,0,2,2)^T$, so $w^THw=0$.

Suppose $H=P+N$, where $P$ is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix) and $N$ is a symmetric [nonnegative matrix](../../../vector-space.md#nonnegative-matrix). Since $w\geq0$, both $w^TPw$ and $w^TNw$ are nonnegative. Their sum is zero, so both vanish. In particular,

$$
0=w^TNw=\sum_{i,j=1}^3 w_iw_jN_{ij}.
$$

Every coefficient $w_iw_j$ in this sum is strictly positive and every $N_{ij}$ is nonnegative, forcing $N_{ij}=0$ for $1\leq i,j\leq3$.

Now apply the same argument to all five cyclic shifts of $w$. The [Horn copositive matrix](../../../linear-algebra.md#horn-copositive-matrix) is cyclically invariant, so every shifted [vector](../../../vector-space.md#vector) also has zero [quadratic form](../../../linear-algebra.md#quadratic-form). It follows that the entries of $N$ vanish on every cyclic block of three consecutive indices. Every pair of indices on a five-cycle lies in such a block, hence $N=0$.

This would imply $P=H$. But the [zero quadratic form of a positive semidefinite matrix](../../../linear-algebra.md#zero-quadratic-form-of-a-positive-semidefinite-matrix) would then force $Hw=0$, contradicting $Hw=(0,0,0,2,2)^T$. Therefore $H$ lies outside the [positive-semidefinite-plus-nonnegative cone](../../../mathematical-optimization.md#positive-semidefinite-plus-nonnegative-cone). By the previous equivalence, its quartic form is a [nonnegative polynomial](../../../polynomial.md#nonnegative-polynomial) that is not a [sum of squares polynomial](../../../polynomial.md#polynomial-sos).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
