# Paper 36

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_36.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_36.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [i](#3/i)
  - [ii](#3/ii)
  - [iii](#3/iii)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $S=\operatorname{supp}x$ be the [support of a vector](../../../numerical-analysis.md#support-of-a-vector) $x$, with $|S|\le s$. Suppose the [null space property](../../../numerical-analysis.md#nullspace-property) holds. Every other feasible [vector](../../../vector-space.md#vector) is $z=x+v$, where $0\ne v\in\ker A$. Splitting its [L1 norm](../../../functional-analysis.md#l1-norm) over $S$ and $S^c$ and using the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
\|x+v\|_1=\|x_S+v_S\|_1+\|v_{S^c}\|_1\ge\|x\|_1-\|v_S\|_1+\|v_{S^c}\|_1>\|x\|_1.
$$

Thus the [sparse vector](../../../numerical-analysis.md#sparse-vector) $x$ is the unique [minimizer](../../../analysis.md#global-minimizer) in [basis pursuit](../../../numerical-analysis.md#basis-pursuit). Notice that the argument works for complex coordinates: it uses the [absolute value](../../../real-analysis.md#absolute-value) inequality, rather than a real [sign function](../../../foundations-of-mathematics.md#sign-function).

Conversely, suppose [basis pursuit](../../../numerical-analysis.md#basis-pursuit) uniquely recovers every [sparse vector](../../../numerical-analysis.md#sparse-vector) of order $s$. Fix $0\ne v\in\ker A$ and any $S$ with $|S|\le s$. Take $x=-v_S$ and $z=v_{S^c}$. These [vectors](../../../vector-space.md#vector) have the same measurements, because $Av_S+Av_{S^c}=0$, and they are distinct since $z-x=v\ne0$. The [vector](../../../vector-space.md#vector) $x$ has at most $s$ nonzero coordinates, so uniqueness gives

$$
\|v_S\|_1=\|x\|_1<\|z\|_1=\|v_{S^c}\|_1.
$$

This is the [null space property](../../../numerical-analysis.md#nullspace-property) for every such $S$. **Uniform unique recovery by [basis pursuit](../../../numerical-analysis.md#basis-pursuit) is equivalent to the order-$s$ [null space property](../../../numerical-analysis.md#nullspace-property).**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

First the [null space property](../../../numerical-analysis.md#nullspace-property) implies [sparse injectivity](../../../numerical-analysis.md#sparse-injectivity). If a nonzero $v\in\ker A$ had at most $2s$ nonzero coordinates, partition its [support of a vector](../../../numerical-analysis.md#support-of-a-vector) into disjoint $S,T$ with $|S|,|T|\le s$. Applying the [null space property](../../../numerical-analysis.md#nullspace-property) to each of these sets yields

$$
\|v_S\|_1<\|v_T\|_1\quad\hbox{and}\quad\|v_T\|_1<\|v_S\|_1,
$$

which is impossible. Hence the [null space](../../../linear-algebra.md#kernel-of-a-linear-map) contains no nonzero [sparse vector](../../../numerical-analysis.md#sparse-vector) of order $2s$.

The feasible [vector](../../../vector-space.md#vector) $x$ has $\|x\|_0\le s$, where the [L0 sparsity count](../../../numerical-analysis.md#l0-sparsity-count) counts its nonzero coordinates. Any different feasible $z$ with $\|z\|_0\le\|x\|_0$ would give a nonzero [null space](../../../linear-algebra.md#kernel-of-a-linear-map) [vector](../../../vector-space.md#vector) $z-x$ with at most $2s$ nonzero coordinates, contrary to [sparse injectivity](../../../numerical-analysis.md#sparse-injectivity). Consequently every different feasible $z$ has strictly larger [L0 sparsity count](../../../numerical-analysis.md#l0-sparsity-count). **The unique sparsest feasible vector is $x$:**

$$
\boxed{\operatorname*{arg\,min}_{Az=Ax}\|z\|_0=\{x\}.}
$$

This proof does not treat the [L0 sparsity count](../../../numerical-analysis.md#l0-sparsity-count) as a genuine [norm](../../../functional-analysis.md#norm); no [triangle inequality](../../../topological-analysis.md#triangle-inequality) for it is needed.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use the stated characterization by the [Lq null space property](../../../numerical-analysis.md#lq-null-space-property). Raising an [Lq quasi-norm](../../../real-analysis.md#lq-quasi-norm) comparison to its positive exponent preserves its order, so the hypothesis at $q$ says that, for every nonzero $v\in\ker A$ and every $|S|\le s$,

$$
\sum_{j\in S}|v_j|^q<\sum_{j\notin S}|v_j|^q.
$$

We prove the corresponding $p$ inequality; this is [monotonicity of uniform sparse recovery in the exponent](../../../numerical-analysis.md#monotonicity-of-uniform-sparse-recovery-in-the-exponent).

Fix a nonzero [null space](../../../linear-algebra.md#kernel-of-a-linear-map) [vector](../../../vector-space.md#vector) and arrange its coordinate magnitudes as $a_1\ge\cdots\ge a_N\ge0$. Assume $s\ge1$. The [Lq null space property](../../../numerical-analysis.md#lq-null-space-property) rules out a nonzero [null space](../../../linear-algebra.md#kernel-of-a-linear-map) [vector](../../../vector-space.md#vector) supported on at most $s$ coordinates, so $s<N$ and $t=a_s>0$. Since $p-q<0$, the factors $a_j^{p-q}$ are at most $t^{p-q}$ for $j\le s$ and at least $t^{p-q}$ for $j>s$ with $a_j>0$. Terms with $a_j=0$ contribute zero and require no negative power of zero. Thus

$$
\sum_{j=1}^s a_j^p\le t^{p-q}\sum_{j=1}^s a_j^q<t^{p-q}\sum_{j=s+1}^N a_j^q\le\sum_{j=s+1}^N a_j^p.
$$

The largest $s$ coordinates maximize the $p$-power sum on any set of size at most $s$. Its complement therefore has the smallest complementary $p$-power sum. The displayed strict inequality proves the [Lq null space property](../../../numerical-analysis.md#lq-null-space-property) at exponent $p$ for every allowed [support of a vector](../../../numerical-analysis.md#support-of-a-vector). The stated recovery characterization now applies to the [Lq quasi-norm](../../../real-analysis.md#lq-quasi-norm) at $p$.

If $\ker A=\{0\}$, the measurement constraint already singles out $x$, for every objective; if $s=0$, only the zero [sparse vector](../../../numerical-analysis.md#sparse-vector) needs recovery. These cases do not need a positive threshold. **Uniform recovery at $q$ implies uniform recovery at every $0<p<q$:**

$$
\boxed{q\text{-recovery of order }s\ \Longrightarrow\ p\text{-recovery of order }s.}
$$

## 2

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Work in $\mathbb C^N$, the domain of the [matrix](../../../vector-space.md#matrix) $A$; the printed $\mathbb C^n$ in the introduction is a dimension typo. For a fixed nonempty [support of a vector](../../../numerical-analysis.md#support-of-a-vector) $S$, write $u$ for the coordinates of $x$ in $S$. Then

$$
\|Ax\|_2^2-\|x\|_2^2=u^*(A_S^*A_S-I_{|S|})u.
$$

The [Gram matrix](../../../linear-algebra.md#gram-matrix) $A_S^*A_S$ is a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator), so its difference from the [identity matrix](../../../vector-space.md#identity-matrix) is also a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator). By the [finite-dimensional spectral theorem](../../../linear-operator-theory.md#finite-dimensional-spectral-theorem), its [matrix 2-norm](../../../continuous-dual-space.md#matrix-2-norm) is the largest absolute [eigenvalue](../../../linear-operator-theory.md#eigenvalue), equivalently

$$
\sup_{u\ne0}\frac{|u^*(A_S^*A_S-I_{|S|})u|}{\|u\|_2^2}=\|A_S^*A_S-I_{|S|}\|_{2\to2}.
$$

Indeed, an expansion in an [orthonormal eigenbasis](../../../linear-operator-theory.md#orthonormal-eigenbasis) bounds every [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) by the largest absolute [eigenvalue](../../../linear-operator-theory.md#eigenvalue), and an appropriate [eigenvector](../../../linear-operator-theory.md#eigenvector) attains that bound. The [restricted isometry constant](../../../numerical-analysis.md#restricted-isometry-constant) must bound this quantity for every $S$ of size at most $s$, and the maximum of these quantities suffices for all [sparse vectors](../../../numerical-analysis.md#sparse-vector) of order $s$. There are finitely many sets, so the maximum exists. The empty set contributes zero. **Therefore**

$$
\boxed{\delta_s(A)=\max_{|S|\le s}\|A_S^*A_S-I_{|S|}\|_{2\to2}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use the natural empty-sum convention $\mu_1(0)=0$ for [cumulative coherence](../../../numerical-analysis.md#cumulative-coherence). This is needed for the printed case $s=1$. For $x=0$ the conclusion is immediate. Otherwise let $S$ be its [support of a vector](../../../numerical-analysis.md#support-of-a-vector), with $k=|S|\le s$. The [Gram matrix](../../../linear-algebra.md#gram-matrix) $G=A_S^*A_S$ has diagonal entries one because the columns have unit [Euclidean norm](../../../functional-analysis.md#euclidean-norm). Each off-diagonal row sum is bounded by

$$
\sum_{j\in S\setminus\{i\}}|\langle a_i,a_j\rangle|\le\mu_1(k-1)\le\mu_1(s-1).
$$

The last inequality uses monotonicity of [cumulative coherence](../../../numerical-analysis.md#cumulative-coherence): enlarging an index set only adds nonnegative summands. There are enough indices to enlarge it because $s\le N$.

The [Gershgorin circle theorem](../../../numerical-analysis.md#gershgorin-circle-theorem) places every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of $G$ within distance $\mu_1(s-1)$ of one. Since $G$ is a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator), its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are real, and the [finite-dimensional spectral theorem](../../../linear-operator-theory.md#finite-dimensional-spectral-theorem) gives

$$
(1-\mu_1(s-1))\|x\|_2^2\le x_S^*Gx_S=\|Ax\|_2^2\le(1+\mu_1(s-1))\|x\|_2^2.
$$

This is the [cumulative coherence bound for restricted isometry](../../../numerical-analysis.md#cumulative-coherence-bound-for-restricted-isometry). The lower bound remains valid when $\mu_1(s-1)>1$, although it is then nonpositive. No assumption that the [matrix](../../../vector-space.md#matrix) is already a near [isometry](../../../riemannian-geometry.md#isometry) is required. **The distortion is bounded by $\mu_1(s-1)$ on every order-$s$ sparse vector.**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For one-column [Gram matrices](../../../linear-algebra.md#gram-matrix), unit [Euclidean norm](../../../functional-analysis.md#euclidean-norm) of the columns gives $A_S^*A_S=1$. The [restricted isometry constant](../../../numerical-analysis.md#restricted-isometry-constant) formula therefore gives $\delta_1=0$. For a two-column [Gram matrix](../../../linear-algebra.md#gram-matrix), put $c=\langle a_i,a_j\rangle$. The difference from the [identity matrix](../../../vector-space.md#identity-matrix) has the form

$$
\begin{pmatrix}0&c\\\overline c&0\end{pmatrix},
$$

up to the convention for the complex [inner product](../../../linear-algebra.md#inner-product). Its characteristic polynomial is $\lambda^2-|c|^2$, so the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $\pm|c|$ and its [matrix 2-norm](../../../continuous-dual-space.md#matrix-2-norm) is $|c|$. Maximizing over pairs gives $\delta_2=\mu$, where $\mu$ is the [mutual coherence](../../../numerical-analysis.md#coherence-of-a-normalized-matrix).

Part (b), together with the minimality defining the [restricted isometry constant](../../../numerical-analysis.md#restricted-isometry-constant), gives $\delta_s\le\mu_1(s-1)$. Every summand defining [cumulative coherence](../../../numerical-analysis.md#cumulative-coherence) is at most the [mutual coherence](../../../numerical-analysis.md#coherence-of-a-normalized-matrix), so $\mu_1(s-1)\le(s-1)\mu$. **Thus, for normalized columns and $N\ge2$,**

$$
\boxed{\delta_1=0,\qquad\delta_2=\mu,\qquad\delta_s\le\mu_1(s-1)\le(s-1)\mu\quad(2\le s\le N).}
$$

The upper range $s\le N$ matters because the printed definition of [cumulative coherence](../../../numerical-analysis.md#cumulative-coherence) stops at $N-1$. For $N=1$, only $\delta_1=0$ is needed; the maximum over pairs defining [mutual coherence](../../../numerical-analysis.md#coherence-of-a-normalized-matrix) is otherwise empty.

## 3

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $\sigma=\operatorname{sgn}(x_S)$, using the real [sign function](../../../foundations-of-mathematics.md#sign-function) on the [support of a vector](../../../numerical-analysis.md#support-of-a-vector) $x$. The [fixed-sign null space condition](../../../numerical-analysis.md#fixed-sign-null-space-condition) in the PDF uses $S^c$ on its right-hand side. This complement is essential. For any real coordinate $x_j\ne0$, the supporting-line inequality for the [absolute value](../../../real-analysis.md#absolute-value) is

$$
|x_j+v_j|\ge|x_j|+\operatorname{sgn}(x_j)v_j.
$$

Every distinct feasible [vector](../../../vector-space.md#vector) is $x+v$ with $0\ne v\in\ker A$. Summing the coordinate inequalities on $S$ and adding the [L1 norm](../../../functional-analysis.md#l1-norm) on $S^c$ gives

$$
\|x+v\|_1-\|x\|_1\ge\langle\sigma,v_S\rangle+\|v_{S^c}\|_1\ge\|v_{S^c}\|_1-|\langle\sigma,v_S\rangle|>0.
$$

The strict final inequality is precisely the [fixed-sign null space condition](../../../numerical-analysis.md#fixed-sign-null-space-condition). **Hence $x$ is the unique [basis pursuit](../../../numerical-analysis.md#basis-pursuit) [minimizer](../../../analysis.md#global-minimizer).** Unlike the [null space property](../../../numerical-analysis.md#nullspace-property) of Question 1, this condition concerns the particular [sign function](../../../foundations-of-mathematics.md#sign-function) values of $x$, rather than every [vector](../../../vector-space.md#vector) supported in $S$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Assume $x$ is the unique [basis pursuit](../../../numerical-analysis.md#basis-pursuit) [minimizer](../../../analysis.md#global-minimizer). Fix $0\ne v\in\ker A$ and set

$$
\alpha=\langle\operatorname{sgn}(x_S),v_S\rangle,\qquad\beta=\|v_{S^c}\|_1.
$$

There is $\varepsilon>0$ such that the [sign function](../../../foundations-of-mathematics.md#sign-function) of $x_j+t v_j$ equals that of $x_j$ at every $j\in S$ whenever $|t|<\varepsilon$. To choose it, take less than the minimum of $|x_j|/|v_j|$ over the nonzero $v_j$ in $S$; if that set is empty, any positive $\varepsilon$ works. On this interval the [L1 norm](../../../functional-analysis.md#l1-norm) has the exact expression

$$
\|x+t v\|_1-\|x\|_1=t\alpha+|t|\beta.
$$

For $0<t<\varepsilon$, both $x+t v$ and $x-t v$ are distinct feasible [vectors](../../../vector-space.md#vector). Uniqueness forces their objective differences to be strictly positive, so $\alpha+\beta>0$ and $-\alpha+\beta>0$. Therefore

$$
\boxed{|\langle\operatorname{sgn}(x_S),v_S\rangle|<\|v_{S^c}\|_1\quad(0\ne v\in\ker A).}
$$

**The [fixed-sign null space condition](../../../numerical-analysis.md#fixed-sign-null-space-condition) is necessary as well as sufficient.** This argument also covers an empty [support of a vector](../../../numerical-analysis.md#support-of-a-vector): then $\alpha=0$ and the nonzero [null space](../../../linear-algebra.md#kernel-of-a-linear-map) [vector](../../../vector-space.md#vector) has $\beta>0$. Strictness is indispensable: equality would make a sufficiently short feasible segment have the same objective as $x$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $u=A^*h$ be the [strict dual certificate for basis pursuit](../../../numerical-analysis.md#strict-dual-certificate-for-basis-pursuit) supplied by condition (ii). For $0\ne v\in\ker A$, we have

$$
0=\langle h,Av\rangle=\langle A^*h,v\rangle=\langle\operatorname{sgn}(x_S),v_S\rangle+\sum_{l\in S^c}u_l v_l.
$$

Here the [adjoint operator](../../../hilbert-space.md#adjoint-operator) is the real transpose. The [injectivity](../../../algebra.md#injective-function) of $A_S$ ensures $v_{S^c}\ne0$: otherwise $A_Sv_S=0$ would force $v=0$. Thus at least one nonzero term lies outside the [support of a vector](../../../numerical-analysis.md#support-of-a-vector) $x$. Since $|u_l|<1$ at every such index,

$$
|\langle\operatorname{sgn}(x_S),v_S\rangle|=\left|\sum_{l\in S^c}u_l v_l\right|\le\sum_{l\in S^c}|u_l|\,|v_l|<\sum_{l\in S^c}|v_l|.
$$

This proves the [fixed-sign null space condition](../../../numerical-analysis.md#fixed-sign-null-space-condition), so part (a) gives uniqueness in [basis pursuit](../../../numerical-analysis.md#basis-pursuit). If $S^c$ is empty, the [injectivity](../../../algebra.md#injective-function) of $A_S=A$ instead means there is no nonzero [null space](../../../linear-algebra.md#kernel-of-a-linear-map) [vector](../../../vector-space.md#vector), and the feasible set is a singleton. **[Injective](../../../algebra.md#injective-function) active columns and a [strict dual certificate for basis pursuit](../../../numerical-analysis.md#strict-dual-certificate-for-basis-pursuit) ensure unique recovery.** Both ingredients matter: strictness outside $S$ cannot detect a nonzero [null space](../../../linear-algebra.md#kernel-of-a-linear-map) direction supported entirely inside $S$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Write $\sigma=\operatorname{sgn}(x_S)$ and $G=A_S^*A_S$. The [injectivity](../../../algebra.md#injective-function) of $A_S$ makes this [Gram matrix](../../../linear-algebra.md#gram-matrix) a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix), since $u^*Gu=\|A_Su\|_2^2>0$ for $u\ne0$. Thus its [matrix inverse](../../../linear-algebra.md#matrix-inverse) exists. Construct the [least-norm dual certificate](../../../numerical-analysis.md#least-norm-dual-certificate)

$$
\boxed{h=A_S(A_S^*A_S)^{-1}\sigma.}
$$

On the active coordinates, $A_S^*h=G G^{-1}\sigma=\sigma$. For $l\notin S$, symmetry of the real [Gram matrix](../../../linear-algebra.md#gram-matrix) and its [matrix inverse](../../../linear-algebra.md#matrix-inverse) gives

$$
(A^*h)_l=a_l^*A_SG^{-1}\sigma=\langle G^{-1}A_S^*a_l,\sigma\rangle.
$$

Condition (iii) makes the [absolute value](../../../real-analysis.md#absolute-value) of this coordinate strictly less than one. Consequently $h$ is a [strict dual certificate for basis pursuit](../../../numerical-analysis.md#strict-dual-certificate-for-basis-pursuit), and part (c) applies. If $S$ is empty, take $h=0$; the zero [vector](../../../vector-space.md#vector) uniquely minimizes the [L1 norm](../../../functional-analysis.md#l1-norm) on its feasible set. **Condition (iii) supplies an explicit certificate and therefore unique recovery.** There is no claim that this particular [least-norm dual certificate](../../../numerical-analysis.md#least-norm-dual-certificate) is necessary: other valid certificates may exist when this one fails.

## 4

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Interpret the angle as the [directed subspace angle](../../../hilbert-space.md#directed-subspace-angle) defined by the infimum of projected unit [vectors](../../../vector-space.md#vector); it is different from the [smallest angle between two subspaces](../../../hilbert-space.md#smallest-angle-between-two-subspaces). Write

$$
a=\cos\theta_{W,V^\perp}>0,\qquad b=\cos\theta_{V^\perp,W}>0.
$$

Consider the [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator) $T:W\longrightarrow V^\perp$ given by $Tw=P_{V^\perp}w$. Its [adjoint operator](../../../hilbert-space.md#adjoint-operator), between these two [Hilbert spaces](../../../hilbert-space.md), is $T^*u=P_Wu$: for $w\in W$ and $u\in V^\perp$, the [orthogonal projections](../../../hilbert-space.md#orthogonal-projection) give $\langle Tw,u\rangle=\langle w,u\rangle=\langle w,P_Wu\rangle$. The two positive [directed subspace angle](../../../hilbert-space.md#directed-subspace-angle) cosines yield

$$
\|Tw\|\ge a\|w\|,\qquad\|T^*u\|\ge b\|u\|.
$$

The first bound makes $T$ [injective](../../../algebra.md#injective-function) and gives a closed range. Explicitly, if $Tw_j$ converges, then $\|w_j-w_k\|\le a^{-1}\|Tw_j-Tw_k\|$, so $(w_j)$ is a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence). The [closed subspace of a Hilbert space](../../../hilbert-space.md#closed-subspace-of-a-hilbert-space) $W$ is complete, and its limit maps to the proposed range limit. The second bound gives $\ker T^*=\{0\}$. A [vector](../../../vector-space.md#vector) $u\in V^\perp$ orthogonal to the range has $T^*u=0$, so it must be zero. The range is therefore dense as well as closed in $V^\perp$, and $T$ is onto. This is the mechanism of [invertibility from lower bounds on an operator and its adjoint](../../../hilbert-space.md#invertibility-from-lower-bounds-on-an-operator-and-its-adjoint).

For any $f\in H$, choose the unique $w\in W$ with $Tw=P_{V^\perp}f$. Then $P_{V^\perp}(f-w)=0$, so $f-w\in V$. Moreover, if $w\in W\cap V$, then $Tw=0$ and hence $w=0$. **Every vector has a unique decomposition, and**

$$
\boxed{H=W\oplus V.}
$$

The [direct sum](../../../vector-space.md#direct-sum) is a topological one as well: the component $w=T^{-1}P_{V^\perp}f$ depends boundedly on $f$, with [operator norm](../../../continuous-dual-space.md#operator-norm) at most $a^{-1}$.

For precision, the quoted equality of the norms of complementary [oblique projections](../../../vector-space.md#oblique-projection) needs both summands nonzero. For example, with $H=\mathbb R$, $V=H$ and $W=\{0\}$, the [oblique projection](../../../vector-space.md#oblique-projection) is $I$, so $\|I\|=1$ but $\|I-I\|=0$. The [secant function](../../../geometry-and-topology.md#secant-trigonometry) has value one here, so the second equality in the quoted formula fails. With nonzero complementary summands its intended version is valid. The proof above does not use that formula. The angle itself is undefined on a zero source space because it has no unit [vectors](../../../vector-space.md#vector); expressing the hypotheses as the two lower bounds handles zero spaces without ambiguity.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use $T=P_{V^\perp}|_U:U\longrightarrow V^\perp$. Positivity of the [directed subspace angle](../../../hilbert-space.md#directed-subspace-angle) cosine gives

$$
\|Tu\|\ge\cos\theta_{U,V^\perp}\,\|u\|,
$$

so $T$ is [injective](../../../algebra.md#injective-function). The two [vector spaces](../../../vector-space.md) have the same finite [dimension](../../../vector-space.md#dimension-vector-space), $n$. By the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem), $T$ is also [surjective](../../../algebra.md#surjective-function). There is no need to assume a second positive [directed subspace angle](../../../hilbert-space.md#directed-subspace-angle) cosine in this finite-dimensional case.

For any $f\in H$, find $u\in U$ with $Tu=P_{V^\perp}f$. Then $f-u\in V$. If $u\in U\cap V$, then $Tu=0$, and [injectivity](../../../algebra.md#injective-function) gives $u=0$. **Hence**

$$
\boxed{H=U\oplus V.}
$$

The [direct sum](../../../vector-space.md#direct-sum) is again bounded: $u=T^{-1}P_{V^\perp}f$. If $n=0$, then $U=\{0\}$ and $V^\perp=\{0\}$, so closedness of $V$ gives $V=H$ and the conclusion directly; no angle of an empty unit sphere is needed. Equal finite [dimensions](../../../vector-space.md#dimension-vector-space) are essential to the surjectivity argument, whereas mere [injectivity](../../../algebra.md#injective-function) between infinite-dimensional [Hilbert spaces](../../../hilbert-space.md) is insufficient.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [linear independence](../../../vector-space.md#linear-independence) of the first $n$ elements of each [orthonormal system](../../../hilbert-space.md#orthonormal-sequence) shows that $T_n$ and $S_n$ have the same finite [dimension](../../../vector-space.md#dimension-vector-space) $n$ and are [closed subspaces of a Hilbert space](../../../hilbert-space.md#closed-subspace-of-a-hilbert-space). Apply part (b) with $U=T_n$ and $V=S_n^\perp$. Since $(S_n^\perp)^\perp=S_n$, the positive [directed subspace angle](../../../hilbert-space.md#directed-subspace-angle) cosine gives

$$
H=T_n\oplus S_n^\perp.
$$

Let $Q$ be the [oblique projection](../../../vector-space.md#oblique-projection) onto $T_n$ along $S_n^\perp$. Define $\widetilde f_n=Qf$. Its residual $f-Qf$ is orthogonal to every $\psi_j$ with $1\le j\le n$, so the required measurements agree. Conversely, if $g\in T_n$ has the same measurements, then $f-g\in S_n^\perp$; uniqueness of the [direct sum](../../../vector-space.md#direct-sum) decomposition gives $g=Qf$. Thus this is [finite-dimensional Hilbert sampling reconstruction](../../../vector-space.md#finite-dimensional-hilbert-sampling-reconstruction).

There is also an explicit coefficient description. Use the [inner product](../../../linear-algebra.md#inner-product) convention linear in its first entry and put

$$
C_{jk}=\langle\phi_k,\psi_j\rangle,\qquad b_j=\langle f,\psi_j\rangle,\qquad\widetilde f_n=\sum_{k=1}^n c_k\phi_k.
$$

Then $Cc=b$. The [orthonormal systems](../../../hilbert-space.md#orthonormal-sequence) show $\|P_{S_n}\sum_k c_k\phi_k\|=\|Cc\|_2$ and $\|\sum_k c_k\phi_k\|=\|c\|_2$, so the smallest [singular value](../../../linear-algebra.md#singular-value) of $C$ is $\cos\theta_{T_n,S_n}>0$. Hence $c=C^{-1}b$, another direct proof of existence and uniqueness.

For $n\ge1$, both summands of this [direct sum](../../../vector-space.md#direct-sum) are nonzero: the infinite [orthonormal system](../../../hilbert-space.md#orthonormal-sequence) $(\psi_j)$ contains $\psi_{n+1}\in S_n^\perp$. The permitted [oblique projection](../../../vector-space.md#oblique-projection) norm formula therefore applies without its degenerate exception, giving

$$
\|Q\|=\|I-Q\|=\sec\theta_{T_n,S_n}.
$$

The [operator norm](../../../continuous-dual-space.md#operator-norm) immediately yields the stability estimate $\|\widetilde f_n\|\le\sec\theta_{T_n,S_n}\|f\|$. For the approximation bounds, put $e=f-P_{T_n}f$. Because $Q$ fixes $T_n$, we have

$$
f-Qf=(I-Q)e,
$$

so the [operator norm](../../../continuous-dual-space.md#operator-norm) estimate gives $\|f-Qf\|\le\sec\theta_{T_n,S_n}\|e\|$. For the lower bound, $e\perp T_n$ while $P_{T_n}f-Qf\in T_n$. The [Pythagorean identity](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) gives

$$
\|f-Qf\|^2=\|e\|^2+\|P_{T_n}f-Qf\|^2\ge\|e\|^2.
$$

**The unique measurement-matching reconstruction is stable and within the [secant function](../../../geometry-and-topology.md#secant-trigonometry) factor of the best [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) approximation:**

$$
\boxed{\widetilde f_n=Qf,\quad\|\widetilde f_n\|\le\sec\theta_{T_n,S_n}\|f\|,\quad\|f-P_{T_n}f\|\le\|f-\widetilde f_n\|\le\sec\theta_{T_n,S_n}\|f-P_{T_n}f\|.}
$$

If a zero-dimensional reconstruction is admitted, it is simply $\widetilde f_0=0$ and its error equals the [norm](../../../functional-analysis.md#norm) of $f$; that case is best stated directly instead of using the angle of a zero space.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
