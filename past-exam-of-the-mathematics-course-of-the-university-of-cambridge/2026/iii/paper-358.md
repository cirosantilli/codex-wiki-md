# Paper 358

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20358.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20358.pdf)

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
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 358](paper-358.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $R_z=(A-zI)^{-1}$ be compact and let $w$ be another resolvent point. The resolvent identity gives

$$
R_w-R_z=(w-z)R_wR_z,
$$

or

$$
\boxed{R_w=[I+(w-z)R_w]R_z}.
$$

The bracket is bounded and the product of a bounded operator with a [compact operator](../../../compact-operator.md) is compact. Thus compactness at one resolvent point implies compactness at every resolvent point.

Fix such a $z$. Spectral mapping for the bounded compact operator $R_z$ gives

$$
\lambda\in\sigma(A)
\quad\Longleftrightarrow\quad
(\lambda-z)^{-1}\in\sigma(R_z)\setminus\{0\}.
$$

Every nonzero spectral point of a compact operator is an isolated eigenvalue of finite multiplicity, and zero is its only possible accumulation point. Hence a [compact resolvent](../../../compact-operator.md#compact-resolvent) operator has only isolated eigenvalues of finite multiplicity, with no finite accumulation point. The spectrum is allowed to be empty.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For $f\in C_c^\infty(\mathbb R)$, integration by parts gives

$$
\|Tf\|^2=\|f''\|^2+\|xf\|^2
+2\operatorname{Re}\langle-f'',ixf\rangle.
$$

Another integration by parts removes the factor $x$ from the real cross term and yields the bound

$$
|2\operatorname{Re}\langle-f'',ixf\rangle|
\leq2\|f'\|\|f\|.
$$

The Sobolev interpolation estimate $\|f'\|^2\leq\varepsilon\|f''\|^2+C_\varepsilon\|f\|^2$ therefore implies

$$
\boxed{\|f''\|^2+\|xf\|^2
\leq C(\|Tf\|^2+\|f\|^2)}.
$$

Thus convergence in the graph norm of the closure forces convergence in $H^2$ and of $xf$ in $L^2$. Conversely, $f\in H^2$ and $xf\in L^2$ clearly makes $-f''+ixf\in L^2$, and cutoff followed by mollification approximates it in this graph norm. Hence

$$
\boxed{D(T)=\{f\in H^2(\mathbb R):xf\in L^2(\mathbb R)\}}.
$$

The operator is accretive because

$$
\operatorname{Re}\langle Tf,f\rangle=\|f'\|^2.
$$

Consequently $T+I$ and its adjoint $T^*+I=-d^2/dx^2-ix+I$ are bounded below by one. The range of $T+I$ is both closed and dense, hence all of $L^2$, so $-1$ is a resolvent point. If $f=(T+I)^{-1}g$ with $\|g\|\leq1$, then $\|f\|\leq1$, and the graph estimate bounds $\|f''\|$ and $\|xf\|$. The compactness criterion in the question shows that $(T+I)^{-1}$ is compact. Thus the [Imaginary Airy operator](../../../compact-operator.md#imaginary-airy-operator) has compact resolvent.

For the unitary translation $(U_af)(x)=f(x-a)$,

$$
U_a^{-1}TU_a=T+iaI.
$$

Therefore

$$
\boxed{\|(T-(z+ia)I)^{-1}\|
=\|(T-zI)^{-1}\|},
$$

so the inverse resolvent norm is constant on every vertical line. The same unitary equivalence gives $\sigma(T)=\sigma(T)+ia$ for every real $a$. If the spectrum contained one point, it would contain its entire vertical line, contradicting the isolated-point spectrum forced by compact resolvent. Hence

$$
\boxed{\sigma(T)=\varnothing}.
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

On $L^2(\mathbb R^2)=L^2(\mathbb R_x)\otimes L^2(\mathbb R_y)$, take

$$
\boxed{\mathcal A=-\partial_x^2+ix=T\otimes I_y},
$$

with its natural tensor-product domain. For every $z\in\mathbb C$,

$$
(\mathcal A-zI)^{-1}=(T-zI)^{-1}\otimes I_y,
$$

so $\sigma(\mathcal A)=\varnothing$. It is not compact: for fixed nonzero $f$ and any orthonormal sequence $(e_n)$ in $L^2(\mathbb R_y)$, the resolvent images

$$
(T-zI)^{-1}f\otimes e_n
$$

are nonzero, mutually orthogonal, and have equal norm, so no subsequence converges.

## 2

↑ **Parent:** [Paper 358](paper-358.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Choose normalized eigenvectors $u_n$ of the finite compressions and embed them as $v_n=P_n^*u_n\in H$. Then

$$
\langle Av_n,v_n\rangle=\lambda_n.
$$

The bounded sequence $(v_n)$ has weakly convergent subsequences. If $v_{n_j}\rightharpoonup v$, then for every $y\in H$, strong convergence $P_n^*P_ny\to y$ and the compressed eigenvalue equation give

$$
\langle(A-\lambda I)v,y\rangle
=\lim_j\langle(A-\lambda_{n_j}I)v_{n_j},P_{n_j}^*P_{n_j}y\rangle=0.
$$

Because $\lambda\notin\sigma(A)$, this forces $v=0$. Every weak cluster point is zero, so $v_n\rightharpoonup0$. Since $\langle Av_n,v_n\rangle=\lambda_n\to\lambda$, the weak-null characterization gives

$$
\boxed{\lambda\in W_e(A)}.
$$

**Thus finite-section [spectral pollution](../../../functional-analysis.md#spectral-pollution) of a bounded operator can occur only in its [essential numerical range](../../../functional-analysis.md#essential-numerical-range).**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let

$$
C_n=\overline{W(Q_nAQ_n^*)}.
$$

The tail spaces decrease, so $C_{n+1}\subseteq C_n$. If $\lambda\in\bigcap_nC_n$, choose a unit vector $v_n$ supported after coordinate $n$ with $|\langle Av_n,v_n\rangle-\lambda|<1/n$. Such vectors converge weakly to zero, hence $\lambda\in W_e(A)$.

Conversely, if $v_j\rightharpoonup0$ and $\langle Av_j,v_j\rangle\to\lambda$, then for every fixed $n$ the first $n$ coordinates of $v_j$ tend to zero. After normalizing $Q_nv_j$, its numerical values still tend to $\lambda$, so $\lambda\in C_n$. Therefore

$$
\boxed{\bigcap_{n=1}^\infty C_n=W_e(A)}.
$$

When the intersection is nonempty, decreasing closed sets have distance functions increasing pointwise to the distance from their intersection; on each compact set this convergence is uniform. This is precisely

$$
\boxed{C_n\downarrow W_e(A)
\quad\text{in the <Attouch--Wets topology>}}.
$$

If $W_e(A)=\varnothing$ and a compact $K$ met every $C_n$, nestedness and compactness would supply a convergent sequence whose limit belongs to all $C_n$, a contradiction. Hence $K\cap C_n=\varnothing$ for all sufficiently large $n$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $H_0=-d^2/dx^2+x^2$. The Hermite expansion gives

$$
\langle H_0f,f\rangle
=\sum_{m=n+1}^\infty(2m+1)|c_m|^2
=\|f'\|^2+\|xf\|^2.
$$

Since $T=-d^2/dx^2+ix^2$,

$$
\langle Tf,f\rangle=\|f'\|^2+i\|xf\|^2,
$$

and therefore

$$
\boxed{\langle Tf,f\rangle
=(i-1)\|xf\|^2
+\sum_{m=n+1}^\infty(2m+1)|c_m|^2}.
$$

Write $X=\|xf\|^2$ and $S=\sum_{m=n+1}^\infty(2m+1)|c_m|^2$. Then $\operatorname{Re}\langle Tf,f\rangle=S-X$, $\operatorname{Im}\langle Tf,f\rangle=X$, and

$$
\operatorname{Re}\langle Tf,f\rangle
+\operatorname{Im}\langle Tf,f\rangle=S\geq2n+3.
$$

If $|z|\leq n$, then $|\operatorname{Re}z+\operatorname{Im}z|\leq\sqrt2n<2n+3$, so

$$
\boxed{|z|\leq n\Longrightarrow z\notin W(Q_nTQ_n^*)}.
$$

Every fixed compact set is eventually excluded from the tail numerical ranges. Part (b) therefore implies

$$
\boxed{W_e(T)=\varnothing}.
$$

## 3

↑ **Parent:** [Paper 358](paper-358.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [spectral theorem for normal operators on a separable Hilbert space](../../../hilbert-space.md#spectral-theorem-for-normal-operators-on-a-separable-hilbert-space) states that a normal operator $A$ has a unique projection-valued measure $E$ on its spectrum such that

$$
\boxed{A=\int_{\sigma(A)}z\,dE(z)}.
$$

For bounded $A$ this integral acts on all of $H$. For an unbounded normal operator,

$$
D(A)=\left\{v:\int|z|^2\,d\langle E(z)v,v\rangle<\infty\right\}.
$$

Equivalently, $A$ is unitarily equivalent to multiplication by a measurable function on a direct sum of $L^2$ spaces.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

By the spectral theorem, the operator in parentheses acts at spectral value $t\in\mathbb R$ by

$$
\frac1{2\pi i}\int_a^b
\left[\frac1{t-x-i\epsilon}
-\frac1{t-x+i\epsilon}\right]dx
=\frac1\pi\int_a^b
\frac\epsilon{(t-x)^2+\epsilon^2}\,dx.
$$

The Poisson kernel converges to $1$ for $t\in(a,b)$, to $1/2$ at $t=a,b$, and to $0$ outside $[a,b]$. It is uniformly bounded, so dominated convergence in the [spectral measure of a normal operator](../../../hilbert-space.md#spectral-measure-of-a-normal-operator) gives the strong limit

$$
E((a,b))+\frac12E(\{a\})+\frac12E(\{b\})
=\boxed{\frac12[E((a,b))+E([a,b])]}.
$$

Applying this operator to $v$ proves the claimed [Stone formula](../../../hilbert-space.md#stone-formula).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $p(x)=x^3-x$. Since $A$ is multiplication by $p$, its spectral projection is multiplication by $\mathbf1_{p^{-1}(S)}$. Hence

$$
\mu_{f,g}(S)=\int_{p^{-1}(S)}f(x)\overline{g(x)}\,dx.
$$

Split $[-1,1]$ at the two critical points $\pm1/\sqrt3$. On each resulting interval, $p$ is monotone, so one-dimensional change of variables shows that the measure is absolutely continuous. For almost every $t$,

$$
\boxed{
\frac{d\mu_{f,g}}{dt}(t)
=\sum_{\substack{x\in[-1,1]\\x^3-x=t}}
\frac{f(x)\overline{g(x)}}{|3x^2-1|}}.
$$

The density vanishes outside

$$
\left[-\frac{2}{3\sqrt3},\frac{2}{3\sqrt3}\right].
$$

Its inverse-square-root singularities at the two critical values are locally integrable, so they do not create singular spectral measure.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
