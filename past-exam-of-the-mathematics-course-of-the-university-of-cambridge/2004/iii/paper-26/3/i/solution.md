<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix an even weight and use the determinant-normalized [slash operator for modular forms](../../../../../../slash-operator-for-modular-forms.md)

$$
(f|_kA)(\tau)=\det(A)^{k/2}(c\tau+d)^{-k}f(A\tau),\qquad A\in GL_2^+(\mathbb Q).
$$

It is unchanged by positive scalar multiples of $A$ and satisfies $(f|A)|B=f|AB$. The [determinant-n matrix representatives for Hecke operators](../../../../../../determinant-n-matrix-representatives-for-hecke-operators.md) are

$$
\Pi_n=\left\{\begin{pmatrix}a&b\\0&d\end{pmatrix}:a,d>0,\ ad=n,\ 0\leq b<d\right\}.
$$

Indeed, integer row operations with determinant one send the first column of an integral determinant-$n$ matrix to $(a,0)^t$, with $a>0$; the second diagonal entry is $d=n/a>0$, and a row shear reduces $b$ modulo $d$. This gives unique representatives of the left modular-group orbits.

Define the [Hecke operator](../../../../../../hecke-operator.md) by

$$
\boxed{T_nf=n^{k/2-1}\sum_{A\in\Pi_n}f|_kA
=n^{k-1}\sum_{ad=n}d^{-k}\sum_{b=0}^{d-1}f\left(\frac{a\tau+b}{d}\right).}
$$

The set of integral matrices of determinant $n$ is stable under right multiplication by the modular group. Right multiplication therefore permutes its left orbits, proving the modular transformation law for $T_nf$. Each summand is holomorphic in the upper half-plane. Its imaginary argument tends to infinity at the cusp, so the formula preserves cusp holomorphy and maps $M_k$ to itself and $S_k$ to itself.

Expand each summand in q. The finite sum over $b$ vanishes unless the Fourier index is divisible by $d$, when it equals $d$. The coefficient at $q^m$ then receives a contribution for each $a\mid\gcd(m,n)$, giving the [Fourier coefficients of a composite-index Hecke operator](../../../../../../fourier-coefficients-of-a-composite-index-hecke-operator.md) formula

$$
\boxed{a_m(T_nf)=\sum_{a\mid\gcd(m,n)}a^{k-1}a_{mn/a^2}(f).}
$$

For $m=0$ interpret the sum over all divisors of $n$, so the constant coefficient is $\sigma_{k-1}(n)a_0(f)$. In particular $a_1(T_nf)=a_n(f)$ and integral coefficients are preserved.

Here is a useful direct derivation of the [Hecke multiplication relations](../../../../../../hecke-multiplication-relations.md). On formal Fourier series put $U_pf=\sum_ma_{pm}q^m$ and $V_pf=f(q^p)$. They obey $U_pV_p=1$, although $V_pU_p$ is generally not the identity. The coefficient formula gives

$$
T_{p^r}=\sum_{j=0}^rp^{j(k-1)}V_p^jU_p^{r-j}.
$$

Multiplying by $T_p=U_p+p^{k-1}V_p$ and using $U_pV_p=1$ separates the terms with $j=0$ from the others and yields

$$
T_pT_{p^r}=T_{p^{r+1}}+p^{k-1}T_{p^{r-1}}\qquad(r\geq1).
$$

For distinct primes, all the relevant shift operators commute. Thus $T_mT_n=T_{mn}$ when $\gcd(m,n)=1$, and each prime-power operator is a polynomial in its prime operator. This proves commutativity. Induction on the smaller of two prime exponents, using the displayed recurrence, gives $T_{p^r}T_{p^s}=\sum_{j=0}^{\min(r,s)}p^{j(k-1)}T_{p^{r+s-2j}}$. Factoring general indices into primes then proves

$$
\boxed{T_mT_n=\sum_{a\mid\gcd(m,n)}a^{k-1}T_{mn/a^2}.}
$$

The auxiliary shifts need not themselves preserve the level-one form space; they are used only to prove identities of coefficient sequences.

For cusp forms, the [Petersson inner product](../../../../../../petersson-inner-product.md) is

$$
\langle f,g\rangle=\int_{\Gamma\backslash\mathbb H}f(\tau)\overline{g(\tau)}y^k\frac{dxdy}{y^2}.
$$

It converges by exponential cusp decay, is positive-definite, and makes the Hecke operators self-adjoint. For the change-of-variable argument, the determinant-normalized slash action compensates exactly for the change in $y^k$, while hyperbolic area is invariant. Integrating a correspondence term in the opposite direction replaces its matrix by its inverse. The adjugate $A^\#=nA^{-1}$ is again an integral matrix of determinant $n$; it has the same slash action as $A^{-1}$, because scalar matrices act trivially. Summing over the two sets of representatives, equivalently over the common finite covering domains of the correspondence, interchanges $f$ and $g$ and proves $\langle T_nf,g\rangle=\langle f,T_ng\rangle$. This explains [Hecke operators are self-adjoint for the Petersson inner product](../../../../../../hecke-operators-are-self-adjoint-for-the-petersson-inner-product.md) with the present normalization.

Commuting self-adjoint operators on the finite-dimensional cusp space have a common orthonormal eigenbasis: diagonalize one, restrict the others to its invariant eigenspaces and repeat. If $f$ is a nonzero common [Hecke eigenform](../../../../../../hecke-eigenform.md), $a_n(f)=a_1(T_nf)=\lambda_na_1(f)$. The first coefficient cannot vanish, since then every coefficient would vanish. Normalize it to one. The eigenvalue is then $\lambda_n=a_n(f)$, and the common eigenspace is one-dimensional because all its normalized Fourier coefficients are fixed. The eigenvalues are real by self-adjointness and are [algebraic integers](../../../../../../algebraic-integer.md), since the Hecke operators act by integer matrices on the integral cusp-form lattice from Question 1. The integral echelon basis and the operator identity there also show that $T_1,\ldots,T_{d-1}$ are an integral basis of the [integral Hecke algebra of level-one cusp forms](../../../../../../integral-hecke-algebra-of-level-one-cusp-forms.md); independence follows by evaluating their first-coefficient functionals on $g_1,\ldots,g_{d-1}$.

The eigenform's coefficient relations are

$$
a_ma_n=\sum_{a\mid\gcd(m,n)}a^{k-1}a_{mn/a^2},\qquad
a_{p^{r+1}}=a_pa_{p^r}-p^{k-1}a_{p^{r-1}}.
$$

They give the [Euler product of a Hecke eigenform](../../../../../../euler-product-of-a-hecke-eigenform.md)

$$
L(f,s)=\sum_{n\geq1}\frac{a_n}{n^s}=\prod_p\left(1-a_pp^{-s}+p^{k-1-2s}\right)^{-1}
$$

in a sufficiently far right half-plane. The [Mellin transform of a cusp-form L-function](../../../../../../mellin-transform-of-a-cusp-form-l-function.md) completes this to $\Lambda(f,s)=(2\pi)^{-s}\Gamma(s)L(f,s)=\int_0^\infty f(iy)y^{s-1}dy$. Splitting at one and using $f(i/y)=i^ky^kf(iy)$ gives

$$
\Lambda(f,s)=\int_1^\infty f(iy)\bigl(y^{s-1}+i^ky^{k-s-1}\bigr)dy.
$$

Exponential decay makes this an entire function of $s$, and the formula proves **$\Lambda(f,s)=i^k\Lambda(f,k-s)$**.

On the noncuspidal line in positive even weights $k\geq4$, the normalized [Eisenstein series](../../../../../../eisenstein-series.md) has eigenvalues $\sigma_{k-1}(n)$, as follows from the same divisor formula for its coefficients; $M_k=\mathbb CE_k\oplus S_k$. As a cuspidal example, $S_{12}$ is spanned by the normalized [modular discriminant](../../../../../../modular-discriminant.md). Its coefficients $\tau(n)$ are the Hecke eigenvalues, and the recurrence gives $\tau(4)=\tau(2)^2-2^{11}=-1472$ from $\tau(2)=-24$. Thus the Hecke theory converts analytic forms into multiplicative arithmetic data.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
