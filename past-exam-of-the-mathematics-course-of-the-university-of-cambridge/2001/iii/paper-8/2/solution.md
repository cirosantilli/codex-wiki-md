<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For genuine degrees three and two, the [resultant](../../../../../resultant.md) is the [Sylvester matrix](../../../../../sylvester-matrix.md) [determinant](../../../../../determinant.md)

$$
\boxed{R(p,q)=\det\begin{pmatrix}
a&b&c&d&0\\0&a&b&c&d\\
\alpha&\beta&\gamma&0&0\\0&\alpha&\beta&\gamma&0\\0&0&\alpha&\beta&\gamma
\end{pmatrix}}.
$$

Equivalently, if $r_1,r_2,r_3$ are the roots of $p$, counted with multiplicity, then $R(p,q)=a^2\prod_iq(r_i)$. Thus **$R(p,q)\ne0$ means that the [polynomials](../../../../../polynomial-split.md) have no common root**, or equivalently are coprime over $\mathbb C$. One can also see this from the matrix: its singularity gives a nonzero relation $Ap+Bq=0$ with $\deg A<2$, $\deg B<3$. If $p,q$ were coprime, $p\mid B$ would force $B=0$, then $A=0$, a contradiction. Conversely, a common factor supplies such a relation after dividing $p,q$ by that factor. When a leading coefficient is zero, use the [resultant](../../../../../resultant.md) for the actual [polynomial](../../../../../polynomial-split.md) degrees rather than assuming the displayed fixed-degree criterion unchanged.

An [algebraic addition theorem](../../../../../algebraic-addition-theorem.md) for a [meromorphic function](../../../../../meromorphic-function.md) $f$ means a nonzero [polynomial](../../../../../polynomial-split.md) $P(U,V,W)$ with

$$
P(f(z),f(w),f(z+w))=0
$$

identically where the values are finite. A local relation extends meromorphically to the other regular arguments.

For a [polynomial](../../../../../polynomial-split.md) $f$ of positive degree $d$, let $z_i$ be the $d$ roots of $f(z)-U$ and $w_j$ the $d$ roots of $f(w)-V$. Form

$$
P(U,V,W)=\prod_{i=1}^d\prod_{j=1}^d\bigl(W-f(z_i+w_j)\bigr).
$$

Its coefficients are separately [symmetric polynomials](../../../../../symmetric-polynomial.md) in the two sets of roots. The [Fundamental theorem of symmetric polynomials](../../../../../fundamental-theorem-of-symmetric-polynomials.md) and the fixed nonzero leading coefficient of $f$ show they are [polynomials](../../../../../polynomial-split.md) in $U,V$. The expression is monic of degree $d^2$ in $W$, so it is nonzero. If $U=f(z)$, $V=f(w)$, one factor vanishes at $W=f(z+w)$. This proves the addition relation, including at exceptional multiple-root values by [polynomial](../../../../../polynomial-split.md) identity. A constant [polynomial](../../../../../polynomial-split.md) instead has the relation $W-f(0)=0$.

For the elliptic case, let $E=\mathbb C/\Lambda$. A nonconstant [elliptic function](../../../../../elliptic-function.md) $f$ defines a [finite morphism](../../../../../finite-morphism.md) $E\to\mathbb P^1$, so the [function field](../../../../../function-field-of-an-algebraic-variety.md) of $E$ is a finite [algebraic extension](../../../../../algebraic-extension.md) of $\mathbb C(f)$. The [elliptic function-field decomposition](../../../../../elliptic-function-field-decomposition.md) expresses it as $\mathbb C(\wp,\wp')$, with

$$
(\wp')^2=4\wp^3-g_2\wp-g_3.
$$

The [Weierstrass addition formula](../../../../../weierstrass-addition-formula.md) makes translation algebraic:

$$
\wp(z+w)=-\wp(z)-\wp(w)+\frac14\left(\frac{\wp'(z)-\wp'(w)}{\wp(z)-\wp(w)}\right)^2.
$$

Differentiating and using the cubic differential equation also makes $\wp'(z+w)$ rational in the four separate values. Therefore $f(z+w)$ lies in a finite [algebraic extension](../../../../../algebraic-extension.md) of $\mathbb C(f(z),f(w))$. Its algebraic equation, after clearing denominators, is the required [polynomial](../../../../../polynomial-split.md) relation. This sketches why every [elliptic function](../../../../../elliptic-function.md), not only $\wp$, has an [algebraic addition theorem](../../../../../algebraic-addition-theorem.md). Constants are already covered.

For the final assertion, consider $f(z)=e^{e^z}$, an [entire function](../../../../../entire-function.md). If $c$ is a period, then $e^{e^z(e^c-1)}=1$ for every $z$. The continuous exponent must be a constant integer multiple of $2\pi i$; its [derivative](../../../../../derivative.md) forces $e^c=1$. Hence its periods are exactly $2\pi i\mathbb Z$, making it a [simply periodic function](../../../../../simply-periodic-function.md).

Suppose it had an [algebraic addition theorem](../../../../../algebraic-addition-theorem.md) $P$. There are only finitely many values $V_0$ for which $P(U,V_0,W)$ is identically zero: a nonzero coefficient [polynomial](../../../../../polynomial-split.md) in $V$ already bounds this exceptional set. Choose a positive irrational $\alpha$ with $e^\alpha$ outside this set, and set $c=\log\alpha$. Specializing $w=c$ gives a nonzero [polynomial](../../../../../polynomial-split.md) $Q(U,W)=P(U,e^\alpha,W)$ and, with $t=e^z$,

$$
0=Q(e^t,e^{\alpha t})=\sum_{m,n}q_{mn}e^{(m+\alpha n)t}.
$$

All exponents with nonzero coefficients are distinct, by irrationality of $\alpha$. Divide by the exponential with largest real exponent and let $t\to+\infty$; its nonzero coefficient would have to tend to zero. This contradiction proves that **simple periodicity does not imply an [algebraic addition theorem](../../../../../algebraic-addition-theorem.md)**. It is the [simply periodic entire function without an algebraic addition theorem](../../../../../simply-periodic-entire-function-without-an-algebraic-addition-theorem.md) example.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
