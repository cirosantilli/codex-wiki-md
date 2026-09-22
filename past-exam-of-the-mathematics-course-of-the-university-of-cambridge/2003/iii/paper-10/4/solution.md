<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The real [Grothendieck inequality](../../../../../grothendieck-inequality.md) asserts that a universal constant $K_G$ satisfies

$$
\left|\sum_{i,j}a_{ij}\langle u_i,v_j\rangle\right|
\le K_G\max_{\varepsilon_i,\delta_j\in\{-1,1\}}\left|\sum_{i,j}a_{ij}\varepsilon_i\delta_j\right|
$$

for every finite real scalar matrix and vectors of norm at most one in a real [Hilbert space](../../../../../hilbert-space-split.md). For complex scalars the corresponding scalar supremum is over phases of modulus at most one; a universal complex constant also exists. We prove both versions, without needing the optimal constant.

First, for unit vectors $u,v$ and a [standard Gaussian vector](../../../../../standard-gaussian-random-vector.md) $G$ on their finite-dimensional span,

$$
\mathbb E\bigl[\operatorname{sgn}\langle G,u\rangle\operatorname{sgn}\langle G,v\rangle\bigr]
=\frac2\pi\arcsin\langle u,v\rangle.
$$

To see this, rotational symmetry makes the angle of the [Gaussian vector](../../../../../gaussian-random-vector.md) uniform in the plane spanned by $u,v$. The two signs differ with probability $\arccos\langle u,v\rangle/\pi$. Subtracting twice this probability from one gives the identity; collinear cases follow directly. Zero Gaussian coordinates have probability zero.

Put $c=\log(1+\sqrt2)$, so $\sinh c=1$ and $0<c<\pi/2$. In the Hilbert [direct sum](../../../../../direct-sum.md) of odd [tensor powers](../../../../../tensor-power.md), formed with the [Hilbert tensor product](../../../../../hilbert-tensor-product.md) inner product, define

$$
U(u)=\bigoplus_{k\ge0}\sqrt{\frac{c^{2k+1}}{(2k+1)!}}\,u^{\otimes(2k+1)},\qquad
V(v)=\bigoplus_{k\ge0}(-1)^k\sqrt{\frac{c^{2k+1}}{(2k+1)!}}\,v^{\otimes(2k+1)}.
$$

The [Hilbert tensor product](../../../../../hilbert-tensor-product.md) satisfies $\langle u^{\otimes m},v^{\otimes m}\rangle=\langle u,v\rangle^m$. For unit $u,v$, both transformed vectors have squared norm $\sum_{k\ge0}c^{2k+1}/(2k+1)!=\sinh c=1$, and the [power series](../../../../../power-series.md) for sine gives

$$
\langle U(u),V(v)\rangle=\sin(c\langle u,v\rangle).
$$

For any finite collection of these transformed vectors, use a [standard Gaussian vector](../../../../../standard-gaussian-random-vector.md) on their finite-dimensional span. The sign identity and $|c\langle u,v\rangle|<\pi/2$ give

$$
\mathbb E\bigl[\operatorname{sgn}\langle G,U(u)\rangle\operatorname{sgn}\langle G,V(v)\rangle\bigr]
=\frac{2c}{\pi}\langle u,v\rangle.
$$

Consequently, writing $M$ for the scalar sign supremum,

$$
\left|\sum_{i,j}a_{ij}\langle u_i,v_j\rangle\right|
=\frac\pi{2c}\left|\mathbb E\sum_{i,j}a_{ij}\operatorname{sgn}\langle G,U(u_i)\rangle\operatorname{sgn}\langle G,V(v_j)\rangle\right|
\le\frac\pi{2c}M.
$$

Vectors of norm below one are padded to unit vectors in additional orthogonal directions, using separate directions for the two families so their cross inner products remain unchanged. This proves the real [Grothendieck inequality](../../../../../grothendieck-inequality.md) with $K_R=\pi/(2\log(1+\sqrt2))$.

For the complex [Grothendieck inequality](../../../../../grothendieck-inequality.md), rotate the total scalar sum to have nonnegative real part. Its real part is the sum of the two real bilinear expressions involving $\operatorname{Re}a_{ij}\operatorname{Re}\langle u_i,v_j\rangle$ and $-\operatorname{Im}a_{ij}\operatorname{Im}\langle u_i,v_j\rangle$. The real inner products are realized in the underlying real [Hilbert space](../../../../../hilbert-space-split.md), rotating one family by $i$ for the imaginary part. Each real coefficient matrix has real sign supremum at most the phase supremum of the original complex matrix. Applying the real inequality twice gives the valid constant **$K_C=2K_R$**. In what follows let $K_G$ denote the appropriate real or complex constant.

Now let $T:L^1(0,1)\to H$ be a [bounded linear operator](../../../../../continuous-linear-operator.md) into a [Hilbert space](../../../../../hilbert-space-split.md), and write $M=\|T\|$. If $M=0$ there is nothing to prove. Approximate a finite family of functions by simple functions on a common disjoint measurable partition. For such a family, write $f_j=\sum_k a_{jk}1_{A_k}$ and $m_k=|A_k|>0$. The vectors

$$
h_k=T(1_{A_k}/m_k)
$$

have norm at most $M$. Choose unit vectors $u_j$ with $\langle Tf_j,u_j\rangle=\|Tf_j\|$; zero images contribute zero and can be assigned any unit vector. With inner products linear in their first argument, the [Grothendieck inequality](../../../../../grothendieck-inequality.md) gives

$$
\sum_j\|Tf_j\|
= M\sum_{j,k}m_ka_{jk}\langle h_k/M,u_j\rangle
\le K_G M\sup_{|\alpha_j|\le1,\,|\beta_k|\le1}\left|\sum_{j,k}m_ka_{jk}\alpha_j\beta_k\right|
=K_G M\sup_{|\alpha_j|\le1}\left\|\sum_j\alpha_jf_j\right\|_1.
$$

Over the real field, phases here are signs. For any [Banach space](../../../../../banach-space-split.md) $E$, [operator norm duality](../../../../../operator-norm-duality.md) gives

$$
\sup_{|\alpha_j|\le1}\left\|\sum_j\alpha_jf_j\right\|_E
=\sup_{\phi\in B_{E^*}}\sum_j|\phi(f_j)|=w_1(f_1,\ldots,f_m).
$$

Indeed, interchange the two suprema and choose each phase to align the scalar values of the functional. Thus the required summing inequality holds for simple functions. Approximation in the [Lp space](../../../../../lp-space.md) $L^1$ passes it to arbitrary finite families, since both sides vary continuously under finite sums of $L^1$ errors. We obtain

$$
\boxed{\pi_1(T)\le K_G\|T\|;\quad T:L^1(0,1)\to H\text{ is absolutely summing}.}
$$

Finally let $R$ be the closed span of the [Rademacher functions](../../../../../rademacher-function.md) in $L^1(0,1)$. Independence, the scalar second moment, and Q2 give, for each finite scalar family,

$$
\frac1{\sqrt2}\left(\sum_j|a_j|^2\right)^{1/2}
\le\left\|\sum_ja_jr_j\right\|_1
\le\left(\sum_j|a_j|^2\right)^{1/2}.
$$

Completion therefore defines a [Banach space isomorphism](../../../../../banach-space-isomorphism.md) $S:\ell^2\to R$ with $\|S\|\le1$ and $\|S^{-1}\|\le\sqrt2$. If a bounded projection $P:L^1\to R$ existed, $S^{-1}P:L^1\to\ell^2$ would be an [absolutely summing operator](../../../../../absolutely-summing-operator.md) by the result just proved. The ideal property $\pi_1(BTA)\le\|B\|\pi_1(T)\|A\|$, obtained directly from the defining weak 1-norm, would make $I_{\ell^2}=(S^{-1}P)S$ absolutely summing. But its first $n$ coordinate vectors satisfy

$$
\sum_{j=1}^n\|e_j\|_2=n,\qquad
w_1(e_1,\ldots,e_n)=\sup_{\|h\|_2\le1}\sum_{j=1}^n|h_j|=\sqrt n.
$$

A single finite summing constant cannot dominate $\sqrt n$ for all $n$. Hence **the closed Rademacher span is not complemented in $L^1(0,1)$**.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
