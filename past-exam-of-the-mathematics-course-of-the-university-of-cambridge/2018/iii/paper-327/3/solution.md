<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take $D_j=-i\partial_{x_j}$ and the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat f(\lambda)=\int e^{-ix\cdot\lambda}f(x)\,dx$. Write the scalar [polynomial](../../../../../polynomial-split.md) as $P=P_N+P_{N-1}+\cdots+P_0$, with $P_j$ homogeneous of degree $j$. The [principal symbol](../../../../../principal-symbol-of-a-partial-differential-equation.md) of the constant-coefficient [linear partial differential operator](../../../../../linear-partial-differential-operator.md) $P(D)$ is $P_N$. It is an [elliptic differential operator](../../../../../elliptic-differential-operator.md) exactly when

$$
\boxed{P_N(\lambda)\ne0\quad\text{for every real }\lambda\ne0.}
$$

Complex coefficients are allowed, but the frequency $\lambda$ is real.

By compactness of the unit [sphere](../../../../../sphere.md), $c=\min_{|\omega|=1}|P_N(\omega)|>0$. Homogeneity gives $|P_N(\lambda)|\geq c|\lambda|^N$, whereas the lower-degree terms are bounded by $C|\lambda|^{N-1}$ for $|\lambda|\geq1$. The [triangle inequality](../../../../../triangle-inequality.md) then gives the [high-frequency lower bound for an elliptic polynomial](../../../../../high-frequency-lower-bound-for-an-elliptic-polynomial.md):

$$
|P(\lambda)|\geq c|\lambda|^N-C|\lambda|^{N-1}
\geq\frac c2|\lambda|^N\geq c'\langle\lambda\rangle^N
$$

for sufficiently large $|\lambda|$. Thus

$$
\boxed{|P(\lambda)|\gtrsim\langle\lambda\rangle^N\quad(|\lambda|\geq R).}
$$

The [Japanese bracket](../../../../../japanese-bracket.md) is $\langle\lambda\rangle=(1+|\lambda|^2)^{1/2}$. If $N=0$, a nonzero constant $P$ satisfies the same assertion directly.

For real $s$, the [Sobolev space](../../../../../sobolev-space-split.md) is the [tempered distribution](../../../../../tempered-distribution.md) space

$$
H^s(\mathbb R^n)=\left\{u\in\mathcal S'(\mathbb R^n):
\widehat u\text{ is a function and }
\int_{\mathbb R^n}\langle\lambda\rangle^{2s}|\widehat u(\lambda)|^2\,d\lambda<\infty\right\}.
$$

One may include $(2\pi)^{-n}$ in the squared norm for this [Fourier transform](../../../../../fourier-transform.md) normalization; it does not change the space. The [Local Sobolev space](../../../../../local-sobolev-space.md) is

$$
H^s_{\mathrm{loc}}(X)=\{u\in\mathcal D'(X):\chi u\in H^s(\mathbb R^n)
\text{ for every }\chi\in C_c^\infty(X)\},
$$

where [multiplication of a distribution by a smooth function](../../../../../multiplication-of-a-distribution-by-a-smooth-function.md) is followed by extension by zero.

If $u$ is a [compactly supported distribution](../../../../../compactly-supported-distribution.md), choose a [cutoff function](../../../../../cutoff-function.md) $\chi$ equal to one near its [compact support](../../../../../compact-support.md). The finite [order of a distribution](../../../../../order-of-a-distribution.md) gives an integer $M$ and a bound

$$
|\langle u,\psi\rangle|\leq C\max_{|\alpha|\leq M}
\sup_{x\in K}|\partial^\alpha\psi(x)|
$$

for a fixed [compact set](../../../../../compact-space.md) $K$. This also makes $u$ a [tempered distribution](../../../../../tempered-distribution.md). Its [Fourier transform of a compactly supported distribution](../../../../../fourier-transform-of-a-compactly-supported-distribution.md) is the [smooth function](../../../../../smooth-function.md)

$$
\widehat u(\lambda)=\langle u,\chi(x)e^{-ix\cdot\lambda}\rangle,
\qquad |\widehat u(\lambda)|\leq C'\langle\lambda\rangle^M.
$$

The [Leibniz rule](../../../../../leibniz-rule.md) gives the last estimate, and parameter differentiation under the finite-order pairing proves smoothness of this [Fourier transform](../../../../../fourier-transform.md). Therefore the [negative Sobolev regularity of a compactly supported distribution](../../../../../negative-sobolev-regularity-of-a-compactly-supported-distribution.md) is

$$
\boxed{u\in H^s(\mathbb R^n)\quad\text{for every }s<-M-\frac n2.}
$$

Indeed $\langle\lambda\rangle^{2(s+M)}$ is integrable precisely when $2(s+M)<-n$. This proves the claimed existence of a sufficiently negative [Sobolev space](../../../../../sobolev-space-split.md) index.

We use three elementary [Sobolev space](../../../../../sobolev-space-split.md) facts: differentiation of order $q$ maps $H^t$ continuously into $H^{t-q}$; $H^a\subseteq H^b$ for $a\geq b$; and [Sobolev multiplication by a smooth cutoff](../../../../../sobolev-multiplication-by-a-smooth-cutoff.md) is bounded on $H^t$ for every real $t$. The first two follow directly from the frequency weights. For the third, [multiplication of a distribution by a smooth function](../../../../../multiplication-of-a-distribution-by-a-smooth-function.md) becomes convolution with the rapidly decaying $\widehat\chi$, and

$$
\langle\lambda\rangle^t\leq C_t\langle\lambda-\eta\rangle^{|t|}\langle\eta\rangle^t
$$

together with [Young's convolution inequality](../../../../../young-s-convolution-inequality.md) gives the bound. These facts apply after localization as well.

The [high-frequency lower bound for an elliptic polynomial](../../../../../high-frequency-lower-bound-for-an-elliptic-polynomial.md) gives a useful global implication. If $w\in H^r(\mathbb R^n)$ and $P(D)w\in H^t(\mathbb R^n)$, split its [Fourier transform](../../../../../fourier-transform.md) into $|\lambda|\leq R$ and $|\lambda|>R$. The low-frequency part is controlled by $\|w\|_{H^r}$, while the high-frequency part is controlled by $\|P(D)w\|_{H^t}$. Thus, for arbitrary real $r,t$,

$$
\boxed{\|w\|_{H^{t+N}}\leq C_{r,t}\left(\|P(D)w\|_{H^t}+\|w\|_{H^r}\right).}
$$

The conclusion that $w\in H^{t+N}$ is obtained directly by integrating these frequency bounds; it is not an assumption made to state the estimate.

For the [cutoff bootstrap for local elliptic regularity](../../../../../cutoff-bootstrap-for-local-elliptic-regularity.md), fix $U\Subset X$. A [cutoff function](../../../../../cutoff-function.md) equal to one near $\overline U$ makes $u$ a [compactly supported distribution](../../../../../compactly-supported-distribution.md) after multiplication, so the preceding negative-index argument gives $u\in H^r_{\mathrm{loc}}(U)$ for some finite $r$. Suppose inductively that $u\in H^q_{\mathrm{loc}}(U)$. For any [test function](../../../../../test-function.md) $\chi\in C_c^\infty(U)$,

$$
P(D)(\chi u)=\chi P(D)u+[P(D),\chi]u.
$$

The [Leibniz rule](../../../../../leibniz-rule.md) shows that this [commutator](../../../../../commutator.md) has order at most $N-1$, with [smooth functions](../../../../../smooth-function.md) as coefficients, all with [compact support](../../../../../compact-support.md):

$$
[P(D),\chi]=\sum_{|\alpha|\leq N}p_\alpha
\sum_{0<\beta\leq\alpha}\binom\alpha\beta
(D^\beta\chi)D^{\alpha-\beta}.
$$

A second [cutoff function](../../../../../cutoff-function.md) equal to one near $\operatorname{supp}\chi$ lets us apply the stated [Sobolev space](../../../../../sobolev-space-split.md) bounds to every term. Hence $[P(D),\chi]u\in H^{q-N+1}(\mathbb R^n)$, while $\chi P(D)u\in H^s(\mathbb R^n)$. For $N\geq1$, the global estimate yields

$$
\chi u\in H^{\min(s,q-N+1)+N}
=H^{\min(s+N,q+1)}.
$$

This holds for every such $\chi$, so it improves the [Local Sobolev space](../../../../../local-sobolev-space.md) index by one until $s+N$ is reached. A finite number of iterations starting at $r$ proves

$$
\boxed{P(D)u\in H^s_{\mathrm{loc}}(X)\quad\Longrightarrow\quad
u\in H^{s+N}_{\mathrm{loc}}(X).}
$$

Since $U\Subset X$ was arbitrary, the conclusion holds throughout $X$. For $N=0$, division by the nonzero constant $P$ proves it immediately. This is the asserted [elliptic regularity](../../../../../elliptic-regularity.md), proved without assuming an initial nonnegative [Sobolev space](../../../../../sobolev-space-split.md) index.

A first-order example on $\mathbb R^2$ is the [first-order Cauchy-Riemann operator](../../../../../first-order-cauchy-riemann-operator.md)

$$
\boxed{P(D)=D_1+iD_2=-2i\,\partial_{\bar z},\qquad
P_1(\lambda)=\lambda_1+i\lambda_2,\qquad |P_1(\lambda)|=|\lambda|.}
$$

It is an [elliptic differential operator](../../../../../elliptic-differential-operator.md) with complex coefficients. In one real variable, $D=-i\,d/dx$ is already a first-order [elliptic differential operator](../../../../../elliptic-differential-operator.md).

**There is no scalar [elliptic differential operator](../../../../../elliptic-differential-operator.md) of odd order in three variables.** If its order $N$ were odd, its [principal symbol](../../../../../principal-symbol-of-a-partial-differential-equation.md) would satisfy $P_N(-\omega)=-P_N(\omega)$ on $S^2$. Regard the [continuous map](../../../../../continuous-map.md)

$$
f:S^2\longrightarrow\mathbb R^2,\qquad
f(\omega)=(\operatorname{Re}P_N(\omega),\operatorname{Im}P_N(\omega)).
$$

The [Borsuk-Ulam theorem](../../../../../borsuk-ulam-theorem.md) gives $f(\omega)=f(-\omega)$ for some $\omega$. Oddness then gives $f(\omega)=0$, contradicting ellipticity. This is the [odd-order obstruction for scalar elliptic operators in at least three dimensions](../../../../../odd-order-obstruction-for-scalar-elliptic-operators-in-at-least-three-dimensions.md); restricting to a three-dimensional subspace proves the higher-dimensional case too. For real coefficients alone, the same obstruction follows from the [intermediate value theorem](../../../../../intermediate-value-theorem.md) along a path between antipodal points.

The scalar qualification matters. An [elliptic system of differential equations](../../../../../elliptic-system-of-differential-equations.md) can be first order in three variables: with the [Pauli matrices](../../../../../pauli-matrices.md), the matrix symbol $A(\lambda)=\sum_{j=1}^3\sigma_j\lambda_j$ satisfies $A(\lambda)^2=|\lambda|^2\mathbf1$ and is invertible for $\lambda\ne0$. This does not contradict the scalar [polynomial](../../../../../polynomial-split.md) obstruction.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 327](../../paper-327-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
