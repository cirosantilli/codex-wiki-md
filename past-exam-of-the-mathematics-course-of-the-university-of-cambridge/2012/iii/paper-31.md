# Paper 31

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_31.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_31.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)

## 1

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let $V_m=\det[x_i^{j-1}]_{i,j=1}^m$. It is an [alternating polynomial](../../../polynomial.md#alternating-polynomial): exchanging two variables exchanges two rows of the [Vandermonde matrix](../../../galois-theory.md#vandermonde-matrix) and reverses its [determinant](../../../linear-algebra.md#determinant). Hence $V_m$ vanishes whenever $x_k=x_l$, so each factor $x_l-x_k$ divides it. The distinct linear factors are pairwise [coprime polynomials](../../../polynomial.md#coprime-polynomials), and their product therefore divides $V_m$. Both have total degree $0+1+\cdots+(m-1)=m(m-1)/2$, so

$$
V_m=C_m\prod_{k<l}(x_l-x_k).
$$

The coefficient of $x_m^{m-1}$ in the [determinant](../../../linear-algebra.md#determinant) is $V_{m-1}$, by expansion along its last row. The same coefficient in the product is $\prod_{k<l<m}(x_l-x_k)$. Thus $C_m=C_{m-1}$, and $C_1=1$. Consequently the [Vandermonde determinant](../../../galois-theory.md#vandermonde-determinant) identity is

$$
\boxed{\det[x_i^{j-1}]_{i,j=1}^m=\prod_{1\leq k<l\leq m}(x_l-x_k).}
$$

This is a [polynomial](../../../polynomial.md) identity, including repeated coordinates; no division by a possibly zero numerical Vandermonde product is needed.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Write $\widetilde P_j(x)=x^{j-1}+\sum_{r=0}^{j-2}b_{rj}x^r$. The evaluation [matrix](../../../vector-space.md#matrix) $[\widetilde P_j(x_i)]$ is $V_m B$, where $B$ is upper triangular with diagonal entries $1$. Its [determinant](../../../linear-algebra.md#determinant) is therefore unchanged. This is [Vandermonde determinant invariance under monic basis change](../../../galois-theory.md#vandermonde-determinant-invariance-under-monic-basis-change):

$$
\det[\widetilde P_j(x_i)]_{i,j=1}^m=\prod_{k<l}(x_l-x_k).
$$

For $w(x)=x^a e^{-x}$ on $[0,\infty)$, multiply row $i$ by $\sqrt{w(x_i)}$. The requested weighted product becomes the [weighted Vandermonde determinant](../../../galois-theory.md#weighted-vandermonde-determinant) square

$$
\boxed{\prod_{j<k}(x_j-x_k)^2\prod_{i=1}^m w(x_i)=\left(\det[\sqrt{w(x_i)}\,\widetilde P_j(x_i)]_{i,j=1}^m\right)^2.}
$$

The sign difference between the two orientations of the Vandermonde product disappears on squaring. For $a=0$ interpret the weight at zero by continuity, so $w(0)=1$; for $a>0$, $w(0)=0$.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Choose real [monic orthogonal polynomials](../../../numerical-analysis.md#monic-orthogonal-polynomial) $p_j$ of degree $j$, $j=0,1,\ldots$, for $w(x)=x^a e^{-x}$ on $[0,\infty)$, and let

$$
h_j=\int_0^\infty p_j(x)^2w(x)\,dx,\qquad \phi_j(x)=h_j^{-1/2}p_j(x)\sqrt{w(x)}.
$$

Extend each $\phi_j$ by zero to negative $x$. The resulting [functions](../../../function.md) form an [orthonormal set](../../../linear-algebra.md#orthonormal-set) in $L^2(\mathbb R,dx)$. Define the [orthogonal polynomial projection kernel](../../../functional-analysis.md#orthogonal-polynomial-projection-kernel)

$$
\boxed{K_m(x,y)=\sum_{j=0}^{m-1}\phi_j(x)\phi_j(y)=\sqrt{w(x)w(y)}\sum_{j=0}^{m-1}\frac{p_j(x)p_j(y)}{h_j}.}
$$

The formula on the right is for nonnegative arguments; the kernel is zero when either argument is negative. With $\Phi_{ij}=\phi_{j-1}(x_i)$, the kernel evaluation [matrix](../../../vector-space.md#matrix) is $\Phi\Phi^T$. By the [determinant](../../../linear-algebra.md#determinant) multiplication identity and the preceding monic basis change,

$$
\det[K_m(x_i,x_j)]_{i,j=1}^m=\frac{\prod_{i<j}(x_j-x_i)^2\prod_iw(x_i)}{\prod_{j=0}^{m-1}h_j}.
$$

Thus initially $\widehat c_m=c_m\prod_jh_j$.

Use the symmetric labelled [joint probability density](../../../continuous-probability-distribution.md#joint-probability-density) on the full orthant. Expanding the two copies of $\det\Phi$ into [permutations](../../../combinatorics.md#permutation) and integrating all variables, [orthonormality](../../../linear-algebra.md#orthonormal-set) makes a term vanish unless the two [permutations](../../../combinatorics.md#permutation) agree. Each of the $m!$ surviving terms integrates to $1$. Hence

$$
\boxed{f_m(x_1,\ldots,x_m)=\frac1{m!}\det[K_m(x_i,x_j)]_{i,j=1}^m,\qquad c_m=\frac1{m!\prod_{j=0}^{m-1}h_j}.}
$$

If the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are instead listed in increasing order on a single ordered chamber, that chamber's density is $m!$ times this symmetric density. We keep the full-orthant convention throughout.

An explicit choice is $p_j(x)=(-1)^j j!L_j^{(a)}(x)$ in terms of the [Generalized Laguerre polynomials](../../../linear-operator-theory.md#generalized-laguerre-polynomial). To verify the normalization independently, their [Rodrigues' formula](../../../linear-operator-theory.md#rodrigues-formula) gives

$$
p_j(x)=(-1)^j w(x)^{-1}\frac{d^j}{dx^j}(x^{a+j}e^{-x}).
$$

Integrating by parts $j$ times proves orthogonality to every lower-degree [polynomial](../../../polynomial.md). The boundary terms vanish at zero and infinity for $a\geq0$. Taking the other factor to be $p_j$ and using $p_j^{(j)}=j!$ gives $h_j=j!\Gamma(a+j+1)$, where $\Gamma$ is the [Gamma function](../../../complex-analysis.md#gamma-function). The [Laguerre projection kernel](../../../functional-analysis.md#laguerre-projection-kernel) is therefore

$$
\boxed{K_m(x,y)=(xy)^{a/2}e^{-(x+y)/2}\sum_{j=0}^{m-1}\frac{j!}{\Gamma(a+j+1)}L_j^{(a)}(x)L_j^{(a)}(y)}
$$

for $x,y\geq0$.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Write $D_n=\det[K(x_i,x_j)]_{i,j=1}^n$ and expand it by [permutations](../../../combinatorics.md#permutation). The assumptions ensure that the indicated single-variable integrals exist; the [finite-rank projection kernel](../../../functional-analysis.md#finite-rank-projection-kernel) constructed above satisfies them with $r=m$. No symmetry of a general kernel is needed for the following argument.

If a [permutation](../../../combinatorics.md#permutation) fixes $n$, its product contains the separate factor $K(x_n,x_n)$. Integration gives $r$ times the term of the corresponding [permutation](../../../combinatorics.md#permutation) of $\{1,\ldots,n-1\}$. These terms contribute $rD_{n-1}$.

Otherwise $n$ belongs to a longer [permutation cycle](../../../finite-group-theory.md#permutation-cycle). Let $i$ precede $n$ and let $j$ follow it. The only factors containing $x_n$ are $K(x_i,x_n)K(x_n,x_j)$, whose integral is $K(x_i,x_j)$ by the reproducing assumption. Delete $n$ from the cycle to obtain a [permutation](../../../combinatorics.md#permutation) $\tau$ on $n-1$ letters. Inserting $n$ back after any of the $n-1$ possible letters reconstructs exactly one [permutation](../../../combinatorics.md#permutation); its [sign of a permutation](../../../finite-group-theory.md#sign-of-a-permutation) is $-\operatorname{sgn}(\tau)$, since increasing a cycle length by one reverses its sign. Thus the nonfixed terms contribute $-(n-1)D_{n-1}$.

Combining these two disjoint classes proves [projection kernel determinant integration](../../../functional-analysis.md#projection-kernel-determinant-integration):

$$
\boxed{\int_{\mathbb R}D_n\,dx_n=(r-n+1)D_{n-1}.}
$$

For $n=1$, use the empty [determinant](../../../linear-algebra.md#determinant) $D_0=1$, and the statement is precisely the assumed diagonal integral. For our kernel, [orthonormality](../../../linear-algebra.md#orthonormal-set) directly yields

$$
\int_{\mathbb R}K_m(x,y)K_m(y,z)\,dy=K_m(x,z),\qquad \int_{\mathbb R}K_m(x,x)\,dx=m,
$$

so every step of the marginal integration is justified.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

For $1\leq k\leq m$, the [correlation function of a point process](../../../probability-theory.md#correlation-function-of-a-point-process) associated with the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) is

$$
R_k(x_1,\ldots,x_k)=\frac{m!}{(m-k)!}\int_{\mathbb R^{m-k}}f_m(x_1,\ldots,x_m)\,dx_{k+1}\cdots dx_m.
$$

The [factorial](../../../combinatorics.md#factorial) factor counts ordered selections of $k$ distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue), so this is a [factorial](../../../combinatorics.md#factorial) moment density, rather than the ordinary probability density of $k$ particular labels. Equivalently, for a nonnegative measurable test [function](../../../function.md) $F$,

$$
\mathbb E\sum_{i_1,\ldots,i_k\text{ distinct}}F(\lambda_{i_1},\ldots,\lambda_{i_k})=\int_{\mathbb R^k}F(x_1,\ldots,x_k)R_k(x_1,\ldots,x_k)\,d\mathbf x.
$$

Repeated [projection kernel determinant integration](../../../functional-analysis.md#projection-kernel-determinant-integration), with $r=m$, gives a factor $(m-k)!$ on integrating an $m$-by-$m$ kernel [determinant](../../../linear-algebra.md#determinant) down to size $k$. Together with the normalizing $1/m!$ in $f_m$, the factors cancel:

$$
\boxed{R_k(x_1,\ldots,x_k)=\det[K_m(x_i,x_j)]_{i,j=1}^k.}
$$

In particular $R_1(x)=K_m(x,x)$ and $\int R_k\,d\mathbf x=m!/(m-k)!$. Set $R_0=1$ and $R_k=0$ for $k>m$. The [eigenvalue](../../../linear-operator-theory.md#eigenvalue) configuration is thus a [determinantal point process](../../../probability-theory.md#determinantal-point-process) with a rank-$m$ [finite-rank projection kernel](../../../functional-analysis.md#finite-rank-projection-kernel).

## 2

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A [function](../../../function.md) $f:\mathbb R\to\mathbb R$ satisfies [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) with bound $L\geq0$ if

$$
\boxed{|f(x)-f(y)|\leq L|x-y|\quad\text{for every }x,y\in\mathbb R.}
$$

Here $L$ is an admissible [Lipschitz bound](../../../real-analysis.md#lipschitz-bound); the least admissible value is the [Lipschitz constant](../../../real-analysis.md#lipschitz-constant). The later parts use the admissible bound $1$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [empirical spectral measures](../../../probability-theory.md#empirical-spectral-measure) of the two real [symmetric matrices](../../../linear-algebra.md#symmetric-matrix) are

$$
L_N=\frac1N\sum_{i=1}^N\delta_{\lambda_i},\qquad \widehat L_N=\frac1N\sum_{i=1}^N\delta_{\widehat\lambda_i},
$$

where $\delta_t$ is the [Dirac measure](../../../measure-theory.md#dirac-measure) at $t$. Thus $\langle L_N,f\rangle=N^{-1}\sum_i f(\lambda_i)$. Pair the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) in the specified increasing order and apply the [triangle inequality](../../../topological-analysis.md#triangle-inequality) followed by [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) with bound $1$:

$$
\boxed{\left|\langle L_N,f\rangle-\langle\widehat L_N,f\rangle\right|\leq\frac1N\sum_{i=1}^N|f(\lambda_i)-f(\widehat\lambda_i)|\leq\frac1N\sum_{i=1}^N|\lambda_i-\widehat\lambda_i|.}
$$

This deterministic estimate uses only the [Lipschitz bound](../../../real-analysis.md#lipschitz-bound); no entry independence or distributional hypothesis is needed here.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The [Hoffman–Wielandt inequality](../../../linear-operator-theory.md#hoffman-wielandt-inequality) says that for [normal matrices](../../../linear-operator-theory.md#normal-matrix) $A,B$ with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\alpha_i,\beta_i$, there is a [permutation](../../../combinatorics.md#permutation) $\pi$ such that

$$
\sum_{i=1}^N|\alpha_i-\beta_{\pi(i)}|^2\leq\|A-B\|_F^2=\operatorname{Tr}[(A-B)^*(A-B)],
$$

where $\|\cdot\|_F$ is the [Frobenius norm](../../../compact-operator.md#frobenius-norm) and $*$ denotes the [conjugate transpose](../../../linear-operator-theory.md#conjugate-transpose). For [Hermitian matrices](../../../hilbert-space.md#hermitian-operator), the increasingly ordered real [eigenvalues](../../../linear-operator-theory.md#eigenvalue) may be paired directly: this ordering minimizes the sum of squared distances over all [permutations](../../../combinatorics.md#permutation), by removing crossed pairs. In particular, for the real [symmetric matrices](../../../linear-algebra.md#symmetric-matrix) in this question,

$$
\boxed{\sum_{i=1}^N|\lambda_i-\widehat\lambda_i|^2\leq\operatorname{Tr}[(X_N-\widehat X_N)^2].}
$$

The square on the right is justified by symmetry. For arbitrary [matrices](../../../vector-space.md#matrix), the appropriate expression is the conjugate-transpose product, not the ordinary square.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Put $D=|\langle L_N,f\rangle-\langle\widehat L_N,f\rangle|$. Apply the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) to the average of the nonnegative [eigenvalue](../../../linear-operator-theory.md#eigenvalue) differences, and then the [Hoffman–Wielandt inequality](../../../linear-operator-theory.md#hoffman-wielandt-inequality):

$$
D^2\leq\left(\frac1N\sum_i|\lambda_i-\widehat\lambda_i|\right)^2\leq\frac1N\sum_i|\lambda_i-\widehat\lambda_i|^2\leq\frac1N\operatorname{Tr}[(X_N-\widehat X_N)^2].
$$

Taking nonnegative square roots gives the [spectral Lipschitz bound from Frobenius distance](../../../linear-operator-theory.md#spectral-lipschitz-bound-from-frobenius-distance)

$$
\boxed{D\leq\left(\frac1N\operatorname{Tr}[(X_N-\widehat X_N)^2]\right)^{1/2}=\frac{\|X_N-\widehat X_N\|_F}{\sqrt N}.}
$$

The factor $N^{-1/2}$ is essential: the [empirical spectral measure](../../../probability-theory.md#empirical-spectral-measure) has total mass $1$, not $N$.

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

Use the fixed common entry law from the printed setup: $Y=\sqrt N X_{ij}$ has mean zero and [second moment](../../../probability-theory.md#second-moment) $1$ for each upper-triangular entry, including the diagonal. Let

$$
Z_C=Y\mathbf1_{\{|Y|\geq C\}},\qquad t(C)=\mathbb E[Y^2\mathbf1_{\{|Y|\geq C\}}].
$$

Since $\mathbb EY=0$, the removed part after [centered truncation of a Wigner matrix](../../../probability-theory.md#centered-truncation-of-a-wigner-matrix) is

$$
\Delta_{ij}=X_{ij}-\widehat X_{ij}=N^{-1/2}(Z_{C,ij}-\mathbb EZ_C).
$$

Consequently $\mathbb E\Delta_{ij}^2=N^{-1}\operatorname{Var}(Z_C)\leq N^{-1}t(C)$. Symmetry gives $\operatorname{Tr}\Delta^2=\sum_{i,j}\Delta_{ij}^2$. There are $N$ diagonal terms and $N(N-1)$ off-diagonal terms in this sum, so

$$
\mathbb E\left[\frac1N\operatorname{Tr}\Delta^2\right]=\operatorname{Var}(Z_C)\leq t(C).
$$

Mirrored entries are counted twice, as they must be; independence of those mirrored entries is neither true nor needed for this [expectation](../../../probability-theory.md#expected-value) calculation.

By the preceding bound and the [Markov inequality](../../../probability-inequality.md#markov-inequality),

$$
\mathbb P\{D>\varepsilon\}\leq\mathbb P\left\{\frac1N\operatorname{Tr}\Delta^2>\varepsilon^2\right\}\leq\frac{t(C)}{\varepsilon^2}.
$$

The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) applies to $Y^2\mathbf1_{\{|Y|\geq C\}}\leq Y^2$, so $t(C)\to0$. Choose $C$ with $t(C)<\varepsilon^3$. Then

$$
\boxed{\mathbb P\{|\langle L_N,f\rangle-\langle\widehat L_N,f\rangle|>\varepsilon\}<\varepsilon\quad\text{for every }N.}
$$

This [second moment bound for spectral truncation](../../../probability-theory.md#second-moment-bound-for-spectral-truncation) depends only on $\varepsilon$ and the common law of $Y$, and is uniform over [functions](../../../function.md) with [Lipschitz bound](../../../real-analysis.md#lipschitz-bound) $1$. No fourth-moment hypothesis is required. If the scaled entry law were allowed to vary arbitrarily with $N$, a uniform choice would instead require uniform decay of its second-moment tails; the intended fixed-law setting supplies exactly that condition.

## 3

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Use [block matrix](../../../vector-space.md#block-matrix) elimination with the invertible square block $A$:

$$
\begin{pmatrix}I&0\\-CA^{-1}&I\end{pmatrix}\begin{pmatrix}A&B\\C&D\end{pmatrix}=\begin{pmatrix}A&B\\0&D-CA^{-1}B\end{pmatrix}.
$$

The left multiplier is block triangular with identity diagonal blocks, so its [determinant](../../../linear-algebra.md#determinant) is $1$. Taking the [determinant](../../../linear-algebra.md#determinant) of the block-triangular product proves

$$
\boxed{\det M=\det A\,\det(D-CA^{-1}B).}
$$

The [matrix](../../../vector-space.md#matrix) $D-CA^{-1}B$ is the [Schur complement](../../../linear-algebra.md#schur-complement) of $A$. The proof needs $A$ invertible, but does not assume the [Schur complement](../../../linear-algebra.md#schur-complement) or the full [matrix](../../../vector-space.md#matrix) is invertible.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Take $z$ off the real axis, or more generally require both $X-zI$ and $X^{(i)}-zI$ to be invertible. The [spectral theorem for real symmetric matrices](../../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) guarantees these inverses for nonreal $z$. Move coordinate $i$ to the first position by a simultaneous row and column [permutation](../../../combinatorics.md#permutation). With $H=X^{(i)}-zI$, the permuted [matrix](../../../vector-space.md#matrix) is

$$
\begin{pmatrix}X_{ii}-z&x_i^T\\x_i&H\end{pmatrix}.
$$

Solve its equation against the first coordinate vector: if its solution is $(u,v)^T$, then the lower block equation gives $v=-H^{-1}x_i u$. Substitution into the first equation gives $(X_{ii}-z-x_i^TH^{-1}x_i)u=1$. The component $u$ is the requested diagonal entry of the [matrix inverse](../../../linear-algebra.md#matrix-inverse), proving the [Schur complement formula for a diagonal resolvent entry](../../../linear-algebra.md#schur-complement-formula-for-a-diagonal-resolvent-entry):

$$
\boxed{[(X-zI)^{-1}]_{ii}=\frac1{X_{ii}-z-x_i^T(X^{(i)}-zI)^{-1}x_i}.}
$$

The product is bilinear, with transpose, because $x_i$ is real and $X$ is real symmetric, even when the inverse is complex. In a complex [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) version the row is $x_i^*$ instead. The final $x_i$ belongs inside the denominator, as in the original PDF; the converted TeX misplaces it outside the fraction.

The inverse hypotheses matter if $z$ is real: $X=\begin{pmatrix}0&1\\1&0\end{pmatrix}$ is invertible at $z=0$, while its one-by-one principal minor is not. Thus existence of the full inverse alone is not sufficient to use this formula.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Work with $z$ in the upper half-plane. Write the [Stieltjes matrix resolvents](../../../functional-analysis.md#stieltjes-matrix-resolvent) and their normalized [matrix traces](../../../linear-algebra.md#matrix-trace) as

$$
G=(X_N-zI)^{-1},\quad G^{(i)}=(X_N^{(i)}-zI)^{-1},\quad g=\frac1N\operatorname{Tr}G,\quad g^{(i)}=\frac1N\operatorname{Tr}G^{(i)},\quad q_i=x_i^TG^{(i)}x_i.
$$

The minor trace is normalized by $N$, not by $N-1$. This sign convention is the negative of the convention $(zI-X_N)^{-1}$ used in the general [resolvent of an operator](../../../functional-analysis.md#resolvent-of-an-operator) article. Here $g$ is the [Stieltjes transform of a measure](../../../measure-theory.md#stieltjes-transform-of-a-measure) of the [empirical spectral measure](../../../probability-theory.md#empirical-spectral-measure), with kernel $(x-z)^{-1}$.

The diagonal entries of $X_N$ are zero, so the preceding [Schur complement](../../../linear-algebra.md#schur-complement) formula gives $G_{ii}=-1/(z+q_i)$. Taking the [matrix trace](../../../linear-algebra.md#matrix-trace), subtracting the comparison value $-1/(z+g)$, and combining fractions gives the [resolvent self-consistency defect](../../../functional-analysis.md#resolvent-self-consistency-defect)

$$
\begin{aligned}\varepsilon_N(z)&=g+\frac1{z+g}\\&=\frac1N\sum_{i=1}^N\left(\frac1{z+g}-\frac1{z+q_i}\right)\\&=\boxed{\frac1N\sum_{i=1}^N\frac{q_i-g}{(z+g)(z+q_i)}}.\end{aligned}
$$

The positive numerator sign is fixed by this subtraction. All denominators are nonzero in the upper half-plane, as the imaginary-part estimate in the next part shows. The identity is deterministic and does not use entry independence or moment assumptions.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Put $\eta=\operatorname{Im}z>0$. For a real [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$,

$$
\operatorname{Im}\frac1{\lambda-z}=\frac{\eta}{(\lambda-\operatorname{Re}z)^2+\eta^2}>0.
$$

The [spectral theorem for real symmetric matrices](../../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) therefore gives $\operatorname{Im}g>0$ and $\operatorname{Im}q_i\geq0$, since $q_i$ is a sum of $(\lambda-z)^{-1}$ with nonnegative coefficients given by squared eigenvector coordinates of $x_i$. This is the [positive imaginary part of a Stieltjes matrix resolvent](../../../functional-analysis.md#positive-imaginary-part-of-a-stieltjes-matrix-resolvent). Hence

$$
|z+g|\geq\eta,\qquad |z+q_i|\geq\eta.
$$

Apply the [triangle inequality](../../../topological-analysis.md#triangle-inequality) to the identity above, and add and subtract the minor trace:

$$
\begin{aligned}|\varepsilon_N(z)|&\leq\frac1{\eta^2N}\sum_{i=1}^N|q_i-g|\\&\leq\frac1{\eta^2N}\sum_{i=1}^N|q_i-g^{(i)}|+\frac1{\eta^2N}\sum_{i=1}^N|g^{(i)}-g|.
\end{aligned}
$$

The allowed [principal minor resolvent trace bound](../../../functional-analysis.md#principal-minor-resolvent-trace-bound), with the printed $N$ normalization, bounds the second average by $c/(\eta N)$. Thus the explicit conclusion is

$$
\boxed{|\varepsilon_N(z)|\leq\frac1{(\operatorname{Im}z)^2N}\sum_{i=1}^N\left|x_i^T(X_N^{(i)}-zI)^{-1}x_i-g_N^{(i)}(z)\right|+\frac{c}{(\operatorname{Im}z)^3N}.}
$$

In particular, the final term is $O((\operatorname{Im}z)^{-3}N^{-1})$ with a constant independent of $N$. The upper-half-plane restriction gives the displayed positive denominators; in the lower half-plane the analogous bound uses $|\operatorname{Im}z|$.

The chosen centering also has a probabilistic meaning. The column vector $x_i$ is independent of the minor, has mean zero and coordinate [variance](../../../variance.md) $1/N$, so its [conditional expectation](../../../measure-theory.md#conditional-expectation) satisfies

$$
\mathbb E[q_i\mid X_N^{(i)}]=\frac1N\operatorname{Tr}G^{(i)}=g_N^{(i)}.
$$

This explains why the bound isolates fluctuations of a [quadratic form](../../../linear-algebra.md#quadratic-form) around the minor trace. Mean centering alone is not a concentration estimate; no unrequested limiting assertion is being assumed.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
